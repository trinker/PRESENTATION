---
title      : slidify_test
subtitle   : 
author     : Tyler Rinker
job        : 
logo       : 
biglogo    : 
license    : 
framework  : io2012
highlighter: highlight.js
hitheme    : tomorrow
mode       : selfcontained
widgets    : [mathjax, quiz, bootstrap]
---



## Animation

	<div class="scianimator"><div id="Rplot" style="display: inline-block;"></div></div>
	<script src="js/Rplot.js"></script>
<!-- highlight R code -->
<script type="text/javascript">
	SyntaxHighlighter.autoloader(
	  "r    js/shBrushR.js"
	);
	SyntaxHighlighter.defaults["toolbar"] = false;
	SyntaxHighlighter.all();
</script>

--- 

## googleVis

<!-- MotionChart generated in R 3.0.1 by googleVis 0.4.5 package -->
<!-- Tue Sep 10 21:41:44 2013 -->


<!-- jsHeader -->
<script type="text/javascript">
 
// jsData 
function gvisDataMotionChartID2cdc3ccf278d () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
 "Apples",
2008,
"West",
98,
78,
20,
"2008-12-31" 
],
[
 "Apples",
2009,
"West",
111,
79,
32,
"2009-12-31" 
],
[
 "Apples",
2010,
"West",
89,
76,
13,
"2010-12-31" 
],
[
 "Oranges",
2008,
"East",
96,
81,
15,
"2008-12-31" 
],
[
 "Bananas",
2008,
"East",
85,
76,
9,
"2008-12-31" 
],
[
 "Oranges",
2009,
"East",
93,
80,
13,
"2009-12-31" 
],
[
 "Bananas",
2009,
"East",
94,
78,
16,
"2009-12-31" 
],
[
 "Oranges",
2010,
"East",
98,
91,
7,
"2010-12-31" 
],
[
 "Bananas",
2010,
"East",
81,
71,
10,
"2010-12-31" 
] 
];
data.addColumn('string','Fruit');
data.addColumn('number','Year');
data.addColumn('string','Location');
data.addColumn('number','Sales');
data.addColumn('number','Expenses');
data.addColumn('number','Profit');
data.addColumn('string','Date');
data.addRows(datajson);
return(data);
}
 
// jsDrawChart
function drawChartMotionChartID2cdc3ccf278d() {
var data = gvisDataMotionChartID2cdc3ccf278d();
var options = {};
options["width"] =    500;
options["height"] =    350;

    var chart = new google.visualization.MotionChart(
    document.getElementById('MotionChartID2cdc3ccf278d')
    );
    chart.draw(data,options);
    

}
  
 
// jsDisplayChart
(function() {
var pkgs = window.__gvisPackages = window.__gvisPackages || [];
var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
var chartid = "motionchart";
  
// Manually see if chartid is in pkgs (not all browsers support Array.indexOf)
var i, newPackage = true;
for (i = 0; newPackage && i < pkgs.length; i++) {
if (pkgs[i] === chartid)
newPackage = false;
}
if (newPackage)
  pkgs.push(chartid);
  
// Add the drawChart function to the global list of callbacks
callbacks.push(drawChartMotionChartID2cdc3ccf278d);
})();
function displayChartMotionChartID2cdc3ccf278d() {
  var pkgs = window.__gvisPackages = window.__gvisPackages || [];
  var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
  window.clearTimeout(window.__gvisLoad);
  // The timeout is set to 100 because otherwise the container div we are
  // targeting might not be part of the document yet
  window.__gvisLoad = setTimeout(function() {
  var pkgCount = pkgs.length;
  google.load("visualization", "1", { packages:pkgs, callback: function() {
  if (pkgCount != pkgs.length) {
  // Race condition where another setTimeout call snuck in after us; if
  // that call added a package, we must not shift its callback
  return;
}
while (callbacks.length > 0)
callbacks.shift()();
} });
}, 100);
}
 
// jsFooter
</script>
 
<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartMotionChartID2cdc3ccf278d"></script>
 
<!-- divChart -->
  
<div id="MotionChartID2cdc3ccf278d"
  style="width: 500px; height: 350px;">
</div>


--- 


```r
sessionInfo()
```

```
## R version 3.0.1 (2013-05-16)
## Platform: i386-w64-mingw32/i386 (32-bit)
## 
## locale:
## [1] LC_COLLATE=English_United States.1252 
## [2] LC_CTYPE=English_United States.1252   
## [3] LC_MONETARY=English_United States.1252
## [4] LC_NUMERIC=C                          
## [5] LC_TIME=English_United States.1252    
## 
## attached base packages:
## [1] stats     graphics  grDevices utils     datasets  methods   base     
## 
## other attached packages:
## [1] googleVis_0.4.5      knitcitations_0.5-0  bibtex_0.3-6        
## [4] slidifyLibraries_0.3 slidify_0.3.52       reports_0.2.0       
## [7] knitr_1.4.1         
## 
## loaded via a namespace (and not attached):
##  [1] digest_0.6.3   evaluate_0.4.7 formatR_0.9    httr_0.2      
##  [5] markdown_0.6.3 RCurl_1.95-4.1 rJava_0.9-4    RJSONIO_1.0-3 
##  [9] stringr_0.6.2  tools_3.0.1    whisker_0.3-2  xlsx_0.5.1    
## [13] xlsxjars_0.5.0 XML_3.98-1.1   xtable_1.7-1   yaml_2.1.7
```

