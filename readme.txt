=== Page Flip FX ===
Contributors: flashxml
Tags: images, photos, widget, post, plugin, posts, sidebar, page, flip, flipper, pageflipper, free, flash, as3, image, effect, animation, effects, text, xml, photo, slideshow, auto, scroll, scrollbar, tween
Requires at least: 2.8.0
Tested up to: 3.0.1
Stable tag: trunk

An advanced Page Flip. Completely XML customizable without any Flash knowledge. And it's free!

== Description ==

You can integrate it in any website for free without even using Flash. It's a fully skinnable and customizable page flipper with different shadow gradients, alpha and colors. It has a completely skinnable control bar through the skin.xml file. Supports SWFs and multiple types of images (JPG, PNG, BMP, GIF). You can have additional animated text with lots of animation and positioning properties and the text is CSS customizable. Slideshow can be enabled (auto flipping) with different page flipping types and durations. Flipping sounds can be optionally added through external mp3. You can enter in zoom mode or you can go to an URL when clicking on a page.

== Installation ==

Make sure your Wordpress version is greater than 2.8 and your hosting provider is using PHP5.

1. There are two files to download: [WordPress Plugin](http://downloads.wordpress.org/plugin/page-flip-fx.zip "Page Flip FX Plugin") (that you have to install and activate) & [Free archive](http://www.flashxml.net/free/download/page-flip.zip "Page Flip FX")
2. Create a new folder inside your **wp-content** folder called **flashxml**, inside this folder create a new one called **page-flip-fx** and copy the content of the **free archive** there
3. If you copied the **free archive** to a location different than the one above, go to **Page Flip FX** from the **Settings** tab in your **WordPress Dashboard** and update the path accordingly
4. Add `[page-flip-fx][/page-flip-fx]` where you want the Flash to show up in your post/page
5. If you want to make the Page Flip FX part of your theme, edit the template files and add `<?php pageflipfx_echo_embed_code(); ?>` where you want it to show up
6. Go to [FlashXML.net](http://www.flashxml.net/ "Free Flash Components") and [customize your Page Flip FX](http://www.flashxml.net/page-flip.html "Page Flip FX") using the Live Demo. Generate the `settings.xml` text and use it to overwrite `wp-content/flashxml/page-flip-fx/settings.xml`
7. To use your own images, upload them to `wp-content/flashxml/page-flip-fx/images/` and update the `wp-content/flashxml/page-flip-fx/images.xml` file accordingly

= Additional settings file =

To embed the Page Flip FX more than once, you will need another settings file and (probably) another set of images. Let's assume your new file is called `settings2.xml`. Add `[page-flip-fx settings="settings2.xml"][/page-flip-fx]` where you want the Flash to show up in your post/page. If you made the Flash part of your theme, add the file name as **the first argument** of the `pageflipfx_echo_embed_code()` function call (for example `<?php pageflipfx_echo_embed_code("settings2.xml"); ?>`).

= No Flash support text =

To support visitors without Adobe Flash Player, you can provide alternative content by adding the text between `[page-flip-fx]` and `[/page-flip-fx]`. If you made the Flash part of your theme, add the text as **the second argument** of the `pageflipfx_echo_embed_code()` function call (for example `<?php pageflipfx_echo_embed_code("","Alternative content"); ?>`).

= If you have PHP4 =

To make it work with PHP4, add `[page-flip-fx width="600" height="300"][/page-flip-fx]` where you want the Flash to show up in your post/page. If you made the Flash part of your theme, add the width and height as **the third and fourth argument** of the `pageflipfx_echo_embed_code()` function call. Don't forget to provide your own width and height values, since 600 and 300 are just examples.

= Getting rid of the FlashXML.net label =

To remove the FlashXML.net label from the top-left corner you'll need to buy the [paid package](http://www.flashxml.net/page-flip.html "Page Flip FX"). Once you'll do that, simply use the SWF file from the paid package to overwrite the SWF file from the `wp-content/flashxml/page-flip-fx/` folder.

== Screenshots ==

1. The Live Demo on [FlashXML.net](http://www.flashxml.net/page-flip.html "Page Flip FX") is the utility that helps easily customize your Page Flip FX to fit all your needs.