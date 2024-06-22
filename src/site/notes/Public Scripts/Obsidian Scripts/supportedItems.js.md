---
{"dg-publish":true,"permalink":"/public-scripts/obsidian-scripts/supported-items-js/"}
---

// Grab all inlinks to the current page
let pageLinks = dv.array(dv.current().file.path).flatMap(p => dv.page(p).file.inlinks);

// Filter out specific links
let insights = Array.from(pageLinks.filter(pageLinks => pageLinks.path.includes("Insights")));

let sourceContent = Array.from(pageLinks.filter(pageLinks => pageLinks.path.includes("Source Content")));

let studies = Array.from(pageLinks.filter(pageLinks => pageLinks.path.includes("Studies")));

let patents = Array.from(pageLinks.filter(pageLinks => pageLinks.path.includes("Patents")));

let reviews = Array.from(pageLinks.filter(pageLinks => pageLinks.path.includes("Reviews")));

let takeaways = Array.from(pageLinks.filter(pageLinks => pageLinks.path.includes("Takeaways")));

// Prepare arrays for tables
insights = dv.array(Array.from(insights)).map(p => dv.page(p));

sourceContent = dv.array(Array.from(sourceContent)).map(p => dv.page(p));

studies = dv.array(Array.from(studies)).map(p => dv.page(p));

patents = dv.array(Array.from(patents)).map(p => dv.page(p));

reviews = dv.array(Array.from(reviews)).map(p => dv.page(p));

takeaways = dv.array(Array.from(takeaways)).map(p => dv.page(p));

// Tables
dv.table(["Insights"], insights.map(p => [p.file.link]));

dv.table(["Source Content"], sourceContent.map(p => [p.file.link]));

dv.table(["Studies", "Citation Key"], studies.map(p => [p.file.frontmatter.Citation, p.file.link]));

dv.table(["Patents", "Citation Key"], patents.map(p => [p.file.frontmatter.Citation, p.file.link]));

dv.table(["Reviews", "Citation Key"], reviews.map(p => [p.file.frontmatter.Citation, p.file.link]));

dv.table(["Takeaways"], takeaways.map(p => [p.file.link]));