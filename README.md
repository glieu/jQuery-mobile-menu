# jQuery Mobile Menu v1.0

###[jQuery Mobile Menu Examples](http://www.pixelademo.com/mobile-menu/)

### Features
* Multi-level menu support (3 levels max)
* Flexible, lightweight and easy to setup
* Cross-browser compatibility
* Very clean corporate style

* * *
### Usage

####Include the CSS & JS
jquery.mobile-menu.css can be modified to fit website design

    <link rel="stylesheet" href="jquery.mobile-menu.css" />
    <script src="jquery.mobile-menu.min.js"></script>

####Menu Markup
	<div id="mobile-menu">
	    <ul>
	        <li><a href="#">item 1</a>
				<ul>
                    <li><a href="#">sub item 1a</a></li>
                    <li><a href="#">sub item 1b</a></li>
                    <li><a href="#">sub item 1c</a></li>
                </ul>
			</li>
	        <li><a href="#">item 2</a></li>
	        <li><a href="#">item 3</a></li>
	        <li><a href="#">item 4</a></li>
	    </ul>
	</div>
####Initialize

    <script>
        jQuery(document).ready(function($){		
            $("#mobile-menu").mobileMenu({
                MenuWidth: 250,
                SlideSpeed : 300,
                WindowsMaxWidth : 767,
                PagePush : true,
                FromLeft : true,
                Overlay : true,
                CollapseMenu : true,
                ClassName : "mobile-menu"
            });
        });        
    </script>

### Options
    MenuWidth : 250, // menu width, default to 250px
    SlideSpeed: 300, // slide in speed, default to 300ms
    WindowsMaxWidth: 767, // Max window width to display menu, default to 767px. When change this, be sure to the media query in jquery.mobile-menu.css file
    PagePush: true, // default true for push menu, false for overlay
    FromLeft: true, // default true for slide in from left, false for right
    Overlay: true, // default true for darken the page, false no overlay
	CollapseMenu : true, // default true, menu will not collapse whenfalse
    ClassName : "mobile-menu" // if changed, please change jquery.mobile-menu.css file to your class name

### Browser Support
jQuery v1.11.1

### Browser Support
* Chrome
* Firefox
* Safari
* Opera
* IE8+
* Android Browser
* iOS Safari