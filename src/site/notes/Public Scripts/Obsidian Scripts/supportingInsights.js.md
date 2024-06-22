---
{"dg-publish":true,"permalink":"/public-scripts/obsidian-scripts/supporting-insights-js/"}
---

// Grab all inlinks to the current page
let pageLinks = dv.array(dv.current().file.path).flatMap(p => dv.page(p).file.inlinks);

// Filter out specific links
let supportingInsights = Array.from(pageLinks.filter(pageLinks => pageLinks.path.includes("Insights")));


// Create list
dv.list(supportingInsights);