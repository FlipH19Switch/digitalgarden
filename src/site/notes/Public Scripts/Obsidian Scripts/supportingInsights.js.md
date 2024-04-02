---
{"dg-publish":true,"permalink":"/public-scripts/obsidian-scripts/supporting-insights-js/"}
---


<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">

<div class="markdown-embed-title">

# supportingInsights.js

</div>


// Grab all inlinks to the current page
let pageLinks = dv.array(dv.current().file.path).flatMap(p => dv.page(p).file.inlinks);

// Filter out specific links
let supportingInsights = Array.from(pageLinks.filter(pageLinks => pageLinks.path.includes("Insights")));


// Create list
dv.list(supportingInsights);

</div></div>
