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

Make sure your Wordpress version is equal or greater than 2.8 and your hosting provider is using PHP5.

1. Upload the `page-flip-fx` folder along with all its subfolders and files to the `/wp-content/plugins/` folder
2. Activate the plugin from the **Plugins** menu in WordPress Dashboard
3. In the post editor use the following tag to embed the Page Flip: `[page-flip-fx][/page-flip-fx]`. Or add `<?php pageflipfx_echo_embed_code(); ?>` in your templates
4. Go to [FlashXML.net](http://www.flashxml.net/ "Free Flash Components") and [customize your Page Flip](http://www.flashxml.net/page-flip.html "Page Flip") using the Live Demo. Generate the `settings.xml` text and use it to overwrite `page-flip-fx/component/settings.xml`
5. To use your own images, upload them to the `page-flip-fx/component/images` folder and update the `page-flip-fx/component/images.xml` file accordingly

= Additional settings file =

To embed the Page Flip more than once, you will need another settings file and (probably) another set of images. Let's assume your new file is called **settings2.xml**. From the post editor, use the following code: `[page-flip-fx settings="settings2.xml"][/page-flip-fx]`. From the PHP files of your theme, add the file name as *the first argument* of the `pageflipfx_echo_embed_code()` function call. If you use a separate set of images, don't forget to create a new XML file for that and update the `imagesXML` value in the settings file.

= No Flash support text =

To support visitors without Adobe Flash, you can provide alternative textual content. From the post editor, add the text between `[page-flip-fx]` and `[/page-flip-fx]`. From the PHP files of your theme, add the text as *the second argument* of the `pageflipfx_echo_embed_code()` function call.

== Screenshots ==

1. The Live Demo on [FlashXML.net](http://www.flashxml.net/page-flip.html "Page Flip") is the utility that helps easily customize your Page Flip to fit all of your needs.