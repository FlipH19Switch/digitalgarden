---
{"dg-publish":true,"permalink":"/public-scripts/obsidian-scripts/linked-assumptions-js/"}
---

// Grab all outlinks from the current page
let pageLinks = dv.array(dv.current().file.path).flatMap(p => dv.page(p).file.outlinks);

// Filter out specific links
let linkedAssumptions = Array.from(pageLinks.filter(pageLinks => pageLinks.path.includes("Assumptions")));


// Create list
dv.list(linkedAssumptions);