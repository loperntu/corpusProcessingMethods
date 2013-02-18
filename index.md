---
title       : Corpus Processing Methods
subtitle    : An R-chitecture
author      : Shu-Kai Hsieh 謝舒凱
job         : Assitant Prof. at GIL, NTU
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
github:
  user: loperntu
  repo: corpusProcessingMethods
---

## Read-And-Delete

1. Edit YAML front matter
2. Write using R Markdown
3. Use an empty line followed by three dashes to separate slides!

--- .class #id 

## Slide 1

CPM, 到底有什麼特別?

> 1. Linguistics: a data-intensive discipline? 
> 2. Corpus data science
> 3. Pre-processing
> 4. (Corpus-based) Exploratory Data Analysis 
> 5. Hypothesis and Testing
> 6. Statistical Modeling
> 7. Demo: Shiny-LexicoR 

---

## Motion Chart

<!-- MotionChart generated in R 2.15.1 by googleVis 0.2.17 package -->
<!-- Mon Feb 18 17:29:35 2013 -->


<!-- jsHeader -->
<script type="text/javascript" src="http://www.google.com/jsapi">
</script>
<script type="text/javascript">
 
// jsData 
function gvisDataMotionChartIDea77ce696fb ()
{
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
function drawChartMotionChartIDea77ce696fb() {
  var data = gvisDataMotionChartIDea77ce696fb();
  var options = {};
options["width"] =    600;
options["height"] =    500;

     var chart = new google.visualization.MotionChart(
       document.getElementById('MotionChartIDea77ce696fb')
     );
     chart.draw(data,options);
    

}
  
 
// jsDisplayChart 
function displayChartMotionChartIDea77ce696fb()
{
  google.load("visualization", "1", { packages:["motionchart"] }); 
  google.setOnLoadCallback(drawChartMotionChartIDea77ce696fb);
}
 
// jsChart 
displayChartMotionChartIDea77ce696fb()
 
<!-- jsFooter -->  
//-->
</script>
 
<!-- divChart -->
  
<div id="MotionChartIDea77ce696fb"
  style="width: 600px; height: 500px;">
</div>



---

## ggplot2

  carat       cut color clarity depth table price    x    y    z
1  0.23     Ideal     E     SI2  61.5    55   326 3.95 3.98 2.43
2  0.21   Premium     E     SI1  59.8    61   326 3.89 3.84 2.31
3  0.23      Good     E     VS1  56.9    65   327 4.05 4.07 2.31
4  0.29   Premium     I     VS2  62.4    58   334 4.20 4.23 2.63
5  0.31      Good     J     SI2  63.3    58   335 4.34 4.35 2.75
6  0.24 Very Good     J    VVS2  62.8    57   336 3.94 3.96 2.48
![plot of chunk unnamed-chunk-2](figure/unnamed-chunk-2.png) 


---
