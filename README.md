# banners-with-manners
Responsive, Object-orientated e-commerce banners.

This is a simple framework for generating fast, responsive e-commerce banners (or banners of any type for that matter - it just so happens that I was working on an e-commerce project at the time!).

How To Use

- Incorporate the CSS and JS into your workflow
- Ensure you also link to JQuery 
- Generate a banner by instantiating a new object, feeding it a DOM node and creating a settings file.

Example: http://codepen.io/Goodson/pen/GppNjB

var bannersettings = {
  promoNumber:1,
  url:'http://www.bbc.co.uk',
  header1:"<span>I am a </span><em>60 / 40</em> split banner with a headline on the left",
  header2:"<span>This is </span><em>a test</em> headline 2",
  header3:"<span>This is </span><em>a test</em> headline 3",
  preheader:"Online Only ",
  subtitle:"Enter Code <span>AW14ZEDRT</span> At Checkout",
  background:"rgba(20,20,60,1)"
};

var banner1 = createBanner('generated',bannersettings); //assumes you have a class of '.generated' in your markup.

Customisation Options

- promoNumber //this determines which layout will be used.  1 - 60 / 40 split, 2 - 50 / 50 split, 3 - 100% wide, 4 - 33% split
- url //the link wrapper
- header1, header2, header3 //header titles for the banner
- preheader //preheader banner title
- subtitle //subtitle for the banner
- background //can be an RGBA value, a URL or hash reference.  Can set multiple CSS properties in one string.

More Information

This framework is intended to be light and fast.  It mostly (apart from the background) separates out presentation from the data layer for ultimate flexability.  The CSS file includes a few defaults but it's just a base for more detailed customisation.


