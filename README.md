# json-tree-view
this is my improved version from https://www.cssscript.com/json-data-tree-view/


Yet another JSON viewer library that renders your JSON data as a collapsible and expandable tree structure for better readability.

How to use it:\
Download and import the json-view’s files into the document.

<link rel="stylesheet" href="/path/to/jsonview.css" />\
The library uses Font Awesome for the collapse/expand icons.

<link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.2.0/css/all.css" integrity="sha384-hWVjflwFxL6sNzntih27bfxkr27PmbbK/iSvJ+a4+0owXq79v+lsFkW54bOGbiDQ" crossorigin="anonymous">\
<script src="/path/to/jsonview.js"></script>\
Create a container to place the JSON viewer.

<div class="root"></div>\
Format and render your JSON data in the container.

let data = '{}';\
let target = '.root';\
jsonView.format(data, target);\


API methods.

// expand tree\
jsonView.expandChildren(tree);

// collapse tree\
jsonView.collapseChildren(tree);

// treverse tree object\
jsonView.traverseTree(tree, function(node) {\
  console.log(node);\
});\
