---
layout: page
title: "JavaScript vsprintf function"
comments: true
sharing: true
footer: true
alias:
- /functions/view/vsprintf:580
- /functions/view/vsprintf
- /functions/view/580
- /functions/vsprintf:580
- /functions/580
---
<!-- Generated by Rakefile:build -->
A JavaScript equivalent of PHP's vsprintf

{% codeblock strings/vsprintf.js lang:js https://raw.github.com/kvz/phpjs/master/functions/strings/vsprintf.js raw on github %}
function vsprintf(format, args) {
  //  discuss at: http://phpjs.org/functions/vsprintf/
  // original by: ejsanders
  //  depends on: sprintf
  //   example 1: vsprintf('%04d-%02d-%02d', [1988, 8, 1]);
  //   returns 1: '1988-08-01'

  return this.sprintf.apply(this, [format].concat(args));
}
{% endcodeblock %}

 - [Raw function on GitHub](https://github.com/kvz/phpjs/blob/master/functions/strings/vsprintf.js)

Please note that php.js uses JavaScript objects as substitutes for PHP arrays, they are 
the closest match to this hashtable-like data structure. 

Please also note that php.js offers community built functions and goes by the 
[McDonald's Theory](https://medium.com/what-i-learned-building/9216e1c9da7d). We'll put online 
functions that are far from perfect, in the hopes to spark better contributions. 
Do you have one? Then please just: 

 - [Edit on GitHub](https://github.com/kvz/phpjs/edit/master/functions/strings/vsprintf.js)


### Other PHP functions in the strings extension
{% render_partial _includes/custom/strings.html %}
