=== Contact Form FX ===
Contributors: flashxml
Tags: images, photos, widget, post, plugin, posts, sidebar, contact, form, as3, text, free, flash, xml, label, customization, layout, button, background, shade
Requires at least: 2.8.0
Tested up to: 3.0.1
Stable tag: trunk

One of the most advanced Contact Forms on the web. Completely XML customizable, without any Flash knowledge. And it's free!

== Description ==

You can integrate it in any website for free without any Flash knowledge. It has customizable width and height for the whole application. You can create your own custom fields, indicate which ones are required or not. There are multiple options for labels customization, many background and shade properties along with properties for the layout personalization. Other features are present in the Live Demo.

== Installation ==

Make sure your Wordpress version is greater than 2.8 and your hosting provider is using PHP5.

1. There are two files to download: [WordPress Plugin](http://downloads.wordpress.org/plugin/contact-form-fx.zip "Contact Form FX Plugin") (that you have to install and activate) & [Free package](http://www.flashxml.net/free/download/contact-form.zip "Contact Form FX")
2. Create a new folder inside your **wp-content** folder called **flashxml**, inside this folder create a new one called **contact-form-fx** and copy the content of the **free package** there
3. If you copied the **free package** to a location different than the one above, go to **Contact Form FX** from the **Settings** tab in your **WordPress Dashboard** and update the path accordingly
4. Add `[contact-form-fx][/contact-form-fx]` where you want the Flash to show up in your post/page
5. If you want to make the Contact Form FX part of your theme, edit the template files and add `<?php contactformfx_echo_embed_code(); ?>` where you want it to show up
6. Go to [FlashXML.net](http://www.flashxml.net/ "Free Flash Components") and [customize your Contact Form FX](http://www.flashxml.net/contact-form.html "Contact Form FX") using the Live Demo. Generate the `settings.xml` text and use it to overwrite `wp-content/flashxml/contact-form-fx/settings.xml`

= Additional settings file =

To embed the Contact Form FX more than once, you will need another settings file. Let's assume your new file is called `settings2.xml`. Add `[contact-form-fx settings="settings2.xml"][/contact-form-fx]` where you want the Flash to show up in your post/page. If you made the Flash part of your theme, add the file name as **the first argument** of the `contactformfx_echo_embed_code()` function call (for example `<?php contactformfx_echo_embed_code("settings2.xml"); ?>`).

= No Flash support text =

To support visitors without Adobe Flash Player, you can provide alternative content by adding the text between `[contact-form-fx]` and `[/contact-form-fx]`. If you made the Flash part of your theme, add the text as **the second argument** of the `contactformfx_echo_embed_code()` function call (for example `<?php contactformfx_echo_embed_code("","Alternative content"); ?>`).

= If you have PHP4 =

To make it work with PHP4, add `[contact-form-fx width="600" height="300"][/contact-form-fx]` where you want the Flash to show up in your post/page. If you made the Flash part of your theme, add the width and height as **the third and fourth argument** of the `contactformfx_echo_embed_code()` function call. Don't forget to provide your own width and height values, since 600 and 300 are just examples.

= Getting rid of the FlashXML.net label =

To remove the FlashXML.net label from the top-left corner you'll need to buy the [paid package](http://www.flashxml.net/contact-form.html "Contact Form FX"). Once you'll do that, simply use the SWF file from the paid package to overwrite the SWF file from the `wp-content/flashxml/contact-form-fx/` folder.

== Screenshots ==

1. The Live Demo on [FlashXML.net](http://www.flashxml.net/contact-form.html "Contact Form FX") is the utility that helps easily customize your Contact Form FX to fit all your needs.