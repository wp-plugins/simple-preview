=== Simple Preview ===
Contributors: Gabriel Nagmay
Tags: simple-preview, draft, anonymous, public, post, preview, posts
Requires at least: 2.7
Tested up to: 2.9
Stable tag: 0.1.4

Enables you to give a link to anonymous users for public preview of a post before it is published.

== Description ==

Have you ever been writing a post with the help of someone who does not have access to your blog and needed to give them the ability to preview it before publishing? This plugin takes care of that by generating a simple URL that can be given out for public preview.

Where credit is due: This plugin is a updated/modified/simplified version of Public Post Preview 1.3 by Matt Martz and Jonathan Dingman
	
Core Changes: 
1. Completely removed the use of "nonce" variable. Posts marked preview are now accessible by multiple anonymous users. There is no longer a 24hr time limit.
1. Public_Post_Preview used the option variable as an array to store preview state - genius! However, it's use seemed backwards with an empty item == preview true. This logic was reversed so: simple_array[,,true,,true] now means that p=1 and p=4 have previews. This also allows for the preview to be turned off by default. 		
1. Removed extra variables for a cleaner URI: http://www.yourblog.com/?p=1502&preview=true

== Installation ==

1. Upload the `simple-preview` folder to the `/wp-content/plugins/` directory or install directly through the plugin installer.
1. Activate the plugin through the 'Plugins' menu in WordPress or by using the link provided by the plugin installer

NOTE: See "Other Notes" for Upgrade and Usage Instructions as well as other pertinent topics.

== Upgrade ==

1. Use the plugin updater in WordPress or...
1. Delete the previous `public-post-preview` folder from the `/wp-content/plugins/` directory
1. Upload the new `public-post-preview` folder to the `/wp-content/plugins/` directory

== Usage ==

1. Unlike public post preview, simple preview is not turned on by default. 
1. To enable simple preview for a specific post, check 'Allow Anonymous Preview' and save the post. A simple URL will be created.
1. To disable, uncheck the box and save the post again

== Change Log ==

= 0.1.4 (2009-10-28): =
* Initial Public Release