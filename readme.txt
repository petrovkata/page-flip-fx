=== Page Flip FX ===
Contributors: flashxml
Tags: images, photos, widget, post, plugin, posts, sidebar, page, flip, flipper, pageflipper, free, flash, as3, image, effect, animation, effects, text, xml, photo, slideshow, auto, scroll, scrollbar, tween
Requires at least: 2.8.0
Tested up to: 3.0
Stable tag: trunk

== Description ==

One of the most advanced Page Flip. Completely XML customizable, without using Flash. And it's free!

= Main features =

You can integrate it in any website for free without even using Flash. It's a fully skinnable and customizable page flipper with different shadow gradients, alpha and colors. It has a completely skinnable control bar through the skin.xml file. Supports SWFs and multiple types of images (JPG, PNG, BMP, GIF). You can have additional animated text with lots of animation and positioning properties and the text is CSS customizable. Slideshow can be enabled (auto flipping) with different page flipping types and durations. Flipping sounds can be optionally added through external mp3. You can enter in zoom mode or you can go to an URL when clicking on a page.

== Installation ==

Make sure your Wordpress version is greater than 2.8 and your hosting provider is using PHP5.

1. [Download](http://www.flashxml.net/free/download/page-flip.zip "Page Flip FX") or [purchase](http://www.flashxml.net/page-flip.html#swmi-license "Page Flip FX") the Page Flip FX Flash component
2. Create a new folder inside your `/wp-content/` directory called `flashxml/page-flip-fx` and copy the content of the archive to this folder
3. Install [the plugin](http://downloads.wordpress.org/plugin/page-flip-fx.zip "Page Flip FX Plugin") or upload the `page-flip-fx` folder along with all its files to `/wp-content/plugins/` directory
4. Activate the plugin from the **Plugins** tab in **WordPress Dashboard**
5. Go to **Page Flip FX** from the **Settings** tab and update the path in case you used a different one
6. In the post editor use the following tag to embed the Page Flip FX: `[page-flip-fx][/page-flip-fx]`. You could also add `<?php pageflipfx_echo_embed_code(); ?>` in the PHP file of your theme
7. Go to [FlashXML.net](http://www.flashxml.net/ "Free Flash Components") and [customize your Page Flip FX](http://www.flashxml.net/page-flip.html "Page Flip FX") using the Live Demo. Generate the `settings.xml` text and use it to overwrite `flashxml/pageflipfx/settings.xml`
8. To use your own images, upload them to the `flashxml/pageflipfx/images` folder and update the `flashxml/pageflipfx/images.xml` file accordingly

= Additional settings file =

To embed the Page Flip FX more than once, you will need another settings file and (probably) another set of images. Let's assume your new file is called **settings2.xml**. From the post editor, use the following code: `[page-flip-fx settings="settings2.xml"][/page-flip-fx]`. From the PHP files of your theme, add the file name as *the first argument* of the `pageflipfx_echo_embed_code()` function call. If you use a separate set of images, don't forget to create a new XML file for that and update the value in the settings file.

= No Flash support text =

To support visitors without Adobe Flash, you can provide alternative textual content. From the post editor, add the text between `[page-flip-fx]` and `[/page-flip-fx]`. From the PHP files of your theme, add the text as *the second argument* of the `pageflipfx_echo_embed_code()` function call.

= If you have PHP4 =

To make it work if you're using PHP4, add the following code `[page-flip-fx width="600" height="300"][/page-flip-fx]` in the post editor. From the PHP files of your theme, add the width and height as *the third and fourth argument* of the `pageflipfx_echo_embed_code()` function call. Don't forget to provide your own width and height values, since 600 and 300 are just examples.

== Screenshots ==

1. The Live Demo on [FlashXML.net](http://www.flashxml.net/page-flip.html "Page Flip FX") is the utility that helps easily customize your Page Flip FX to fit all your needs.