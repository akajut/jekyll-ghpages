---
layout: post
title:  "Jekyll Code Highlighting"
date:   2015-12-04 13:19:48
categories: jekyll 
---
Testing out Jekyll Code Highlighting

{% highlight js %} 

// Define spreadsheet URL.
//var mySpreadsheet = 'https://docs.google.com/spreadsheet/ccc?key=0AowHVemz7IvedElrNHVTb2dzZm9TX0x5ckViVWx5bXc#gid=0';

var mySpreadsheet = 'https://docs.google.com/spreadsheets/d/1dXMZdCVkP9cqw9e6u-YbhcEy4AsJmuacsUuPOEFOhII#gid=0';

// Load an entire sheet.
$('#statistics').sheetrock({
  url: mySpreadsheet,
  query: "select A,B,D,E,F,G order by F, G",
  labels: ['Trip', 'Start', 'Number of Days', 'Miles', 'St/Pr', 'Area']
});

{% endhighlight %}