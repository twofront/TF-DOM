# TF DOM

TF DOM provides very simple shorthands to help you modify the DOM. Use it with or without browserify.

# Create
  
	var $ = require('tfdom');
  
	var myDiv = $.create('div', {
  	id: 'mydiv', innerHTML: 'My Div', style: 'color: red', parent: document.body, 
    children: [
			$.create('div', {innerText: 'This <br> tag will display as text.'})
		]
   });

# Get

	var someDiv = $.get('divId');
