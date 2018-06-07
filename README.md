# 🖼 Image Slider 🖼 
![CDNJS](https://img.shields.io/cdnjs/v/jquery.svg)
[![GitHub license](https://img.shields.io/github/license/ArslanAmeer/Ui-Component-Minimal-Slider.svg)](https://github.com/ArslanAmeer/Ui-Component-Minimal-Slider/blob/master/LICENSE)
![GitHub repo documentation](https://img.shields.io/badge/Documentation-Proper-brightgreen.svg)
[![Open Source Love](https://badges.frapsoft.com/os/v1/open-source.png?v=103)](https://github.com/ellerbrock/open-source-badges/)
[![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)

[![forthebadge](https://forthebadge.com/images/badges/built-with-love.svg)](https://forthebadge.com)
![Author](https://img.shields.io/badge/Author-Arslan_Ameer-lightgrey.svg)

### A Simple 👌 Elegent 💎 and Minimal  ( ⛏ Customized) Slider Made with HTML CSS &amp; JQuery. 
#### Many Thanks To 🙏 ( https://github.com/viljamis/ResponsiveSlides.js ) 🙇‍♂️
---
### DEMO 

![Slider Demo](assets/images/demo.gif "Responsive Slider")

👉 **[Try Live Demo](https://arslanameer.github.io/Ui-Component-Minimal-Slider/)**

---
## ✏ About 💡:

This slider is made with html css and js. It uses jquery to fade between images automatically and through navigation buttons
or through pagination bullets.
This Slider is Made/Customized for standard use, as a banner or ad slider. 

**NOTE:** I set slider's css and settings for Demo purpose.

Try & modify it as you need.

## 💡 How To Use 🔬 :

➕ Add CSS (styling File) and JS (script File) links inside `<head>` tag of your html file.
These files can be found in `assets/css` and `assets/js` folders.

```html
<link rel="stylesheet" href="assets/css/slider.css">
<link rel="stylesheet" href="assets/css/main.css">
```
And because this slider is JQuery dependent. You can either download [Jquery](https://jquery.com/) from website or use bellow cdn link.

(JQuery minified javascript file is included in `asstes/js`)

Add this link inside of `<head>` tag.
```html
<!-- Main Slider Script Linking -->
<script src="assets/js/slider.min.js"></script>

<!-- Jquery Script Linking -->
<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
  OR
<script src="assets/js/jquery-3.3.1.min.js"></script>
```

➕ Add Markup in your body:
```html
<body>
  <div class="container"><!-- This is Main Container for My Page. U may need it or not. Creat or Modify as per your Need -->
     <div class="rslides_container">
       <ul class="rslides" id="slider">
         <li><img src="assets/images/demoimage (1).jpg" alt="1"></li>
         <li><img src="assets/images/demoimage (2).jpg" alt="2"></li>
         <li><img src="assets/images/demoimage (3).jpg" alt="3"></li>
         <li><img src="assets/images/demoimage (4).jpg" alt="4"></li>
         <!-- Add many Images As you need -->
       </ul>
     </div>
  </div>
  <script>
    // Will Add Slider Initializing Script Here
  </script>
</body>
```

**Finally**
➕ Add this script to your file within seperate `<script>...</script>` tag to initialize your Image Slider.
```js
$(function () {    
    // Slideshow
    $("#slider").responsiveSlides({
        auto: true,                     // Auto Slide Start
        pager: true,                    // Bullets on Bottom
        nav: true,                      // Prev & Next Button 
        speed: 700,                     // Slide Tranistion Speed (ms)
        timeout: 2700,                  // Time INterval Between Eac Slider (ms)
        maxwidth: 800,                  // Slider Width Max
        namespace: "centered-btns"      // Navigation button Location
    });
});
```

  ## YOU'RE DONE! 🎆🎇🎉👏👏
---

### Additional Settings 😎

You can add or modify slider settings in script file. following are complete list of settings you can apply.
```js
$(".rslides").responsiveSlides({
  auto: true,             // Boolean: Animate automatically, true or false
  speed: 500,            // Integer: Speed of the transition, in milliseconds
  timeout: 4000,          // Integer: Time between slide transitions, in milliseconds
  pager: false,           // Boolean: Show pager, true or false
  nav: false,             // Boolean: Show navigation, true or false
  random: false,          // Boolean: Randomize the order of the slides, true or false
  pause: false,           // Boolean: Pause on hover, true or false
  pauseControls: true,    // Boolean: Pause when hovering controls, true or false
  prevText: "Previous",   // String: Text for the "previous" button
  nextText: "Next",       // String: Text for the "next" button
  maxwidth: "",           // Integer: Max-width of the slideshow, in pixels
  navContainer: "",       // Selector: Where controls should be appended to, default is after the 'ul'
  manualControls: "",     // Selector: Declare custom pager navigation
  namespace: "rslides",   // String: Change the default namespace used
  before: function(){},   // Function: Before callback
  after: function(){}     // Function: After callback
});
```

For Further Guidance and Information Please Visit:  http://responsiveslides.com/


## 📄 License  🔐

Ui-Component-Minimal-Slider (Image Slider)
Copyright (C) 2018  - Arslan Ameer

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <http://www.gnu.org/licenses/>.
