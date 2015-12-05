---
layout: post
title:  "Jekyll Code Highlighting"
date:   2015-12-04 13:19:48
categories: jekyll 
---
Testing out Jekyll Code Highlighting

{% highlight js %} 

// Define spreadsheet URL.
var mySpreadsheet = 'https://docs.google.com/spreadsheets/d/1dXMZdCVkP9cqw9e6u-YbhcEy4AsJmuacsUuPOEFOhII/edit?usp=sharing';
mySpreadsheet += '#gid=0' // Pulling data from sheet 1

// Load an entire sheet.
$('#trips').sheetrock({
  url: mySpreadsheet,
  query: "select A,B,D,E,F,G order by F, G",
  labels: ['Trip', 'Start', 'Number of Days', 'Miles', 'St/Pr', 'Area']
});

{% endhighlight %}