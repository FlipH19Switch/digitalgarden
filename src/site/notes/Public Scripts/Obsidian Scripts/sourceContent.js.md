---
{"dg-publish":true,"permalink":"/public-scripts/obsidian-scripts/source-content-js/","created":"2025-06-14T23:55:14.726-04:00","updated":"2025-06-14T23:55:14.726-04:00"}
---

// Grab all inlinks to the current page
let pageLinks = dv.array(dv.current().file.path).flatMap(p => dv.page(p).file.inlinks);

// Filter out specific links
let sourceContent = Array.from(pageLinks.filter(pageLinks => pageLinks.path.includes("Source Content")));


// Create list
dv.list(sourceContent);