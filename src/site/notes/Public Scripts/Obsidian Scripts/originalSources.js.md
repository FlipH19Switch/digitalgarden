---
{"dg-publish":true,"permalink":"/public-scripts/obsidian-scripts/original-sources-js/"}
---

// Similar to code in [Dataview documentation](https://blacksmithgu.github.io/obsidian-dataview/api/code-examples/#find-all-direct-and-indirectly-linked-pages)

// Grab all unique links
let page = dv.current().file.path;
let pages = new Set();
let stack = [page];
while (stack.length > 0) {
    let elem = stack.pop();
    let meta = dv.page(elem);
    if (!meta) continue;

    for (let inlink of meta.file.inlinks.array()) {
        if (pages.has(inlink.path)) continue;

        if (
        inlink.path.includes("Insights") ||
        inlink.path.includes("Source Content") ||
        inlink.path.includes("Studies") ||
        inlink.path.includes("Patents") ||
        inlink.path.includes("Reviews")    
        ) {
        pages.add(inlink.path);
        stack.push(inlink.path);
        }
    }
}

let data = dv.array(Array.from(pages)).map(p => dv.page(p));


// FIlter out relevant links
data = data.filter(data => 
	data.file.path.split('/').includes("Studies") ||
	data.file.path.split('/').includes("Patents") ||
	data.file.path.split('/').includes("Reviews")
	);


// Create table
dv.table(["Source", "Citation Key"], data.map(p => [p.file.frontmatter.Citation, p.file.link]));