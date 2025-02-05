=== Plugin Name ===
Contributors: nomadcoder
Donate link: https://www.paypal.com/paypalme/nomadnewyork
Tags: featured image, thumbnail grid
Tested up to: 6.4
Stable Tag: 6.4
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html


Display a post Thumbnail Grid using Featured Images

== Description ==

Visit the web site for detailed examples. Click on Shortcodes for examples
https://www.plugins.shooflysolutions.com/thumbnail-grid/

This plugin gives you access to a simple shortcodes that displays post thumbnails in a grid. The plugin uses the featured image thumbnail if one exists. If one does not exist, the default thumbnail (if it exists) or title will be displayed instead. Use the category feature to ensure that all of the posts that you want to display in this manner have thumbnails.

For instructions, shortcode descriptions & examples please visit the <a href="https://www.shooflysolutions.com/featured-image-thumbnail-grid-for-wordpress//">plugin web page</a>.


Please be kind and rate this plugin. Please do not rate if there is an issue without going through support first. 

Everything helps!


== Description ==


For quicker support, please visit our website, read the faqs and email us at support@shooflysolutions.com.

Donations for extended support are appreciated but are never required!

This plugin gives you access to two a simple shortcake to display post thumbnails in a grid. The plugin uses the featured image thumbnail if one exists. If one does not exist, the title will be displayed instead. Use the category feature to ensure that all of the posts that you want to display in this manner have thumbnails.

This plugin is not designed to show several pages of thumbnails, rather it is designed to allow you to embed thumbnails into any page or to display a subset of thumbnails on a page. To show more thumbnails on a page than the default value Blog pages show at most, use a fixed value for posts_per_page or try setting the posts_per_page value to ’999′.

Your theme must be enabled for post thumbnails.

POSTS & PAGES

You can use any of the parameters listed in the wordpress codex.
Click here to see the WordPress Codex for Posts

Here are some of the most common paramaters:

cat = (*Use cat instead of category for posts if category does not work) category id. To view the category id, go to your post categories, edit the category and look in the browser address bar for the category id. If you don’t see it, click your mouse in the address bar.
It should look something like this. The category id is 7:

[[your site goes here]]/wp-admin/edit-tags.php?action=edit&taxonomy=category&tag_ID=7&post_type=post

posts_per_page - the number of posts to display. The default is -1. This causes the post count to default to the value in Blog pages show at most.

post_type – the type of posts to display. The default is ‘post”.  Enter any type that supports thumbnails. Obviously, you want to have featured images set for all of the posts that you are displaying in this grid. You can use ‘page’ here if your theme supports thumbnails on pages. You can enter custom post types, like ‘events’ in this section too.

orderby - Sort retrieved posts by parameter. The default is none.

order – ‘DESC’ or ‘ASC’

tag - use the tag name, not the tag id.

[thumbnailgrid cat='1' posts='5' type='post' order_by='author' order='ASC']”

Will display the thumbnails for the 5 most recent posts from the category with the id of 1 sorted by the author name in ascending order

[thumbnailgrid]
Will display the thumbnails using the default value in the Reading settings Blog pages show at most.



Examples:

[bkthumbnailgrid category="4" limit="5"]
displays the thumbnails for the first 5 bookmarks where the link category is 4.

[bkthumbnailgrid orderby="owner" order="DESC"]
displays all thumbnails for all bookmarks ordered descending by the name of the owner.

Shortcodes
Most properties can be set in the style sheet or in the custom css module for your theme. The following settings are shortcode settings that apply to individual grids. Note that for width and height values you may use any valid unit of height: px, cm, %, etc. Note: Media Image sizes are configured in the wordpress admin panel under Settings/Media. The default thumbnail size is 150px by 150px. The style sheet is configured to handle the default thumbnail size. To properly display your images, you must modify the height and witdth in the thumbanil shortcode or the style sheet.

Visit  <a href="http://www.shooflysolutions.com/software/featured-image-thumbnail-grid-for-wordpress/">ShooflySolutions</a> for demos.

height
The height of thumbnail image. This value defaults to the height of the thumbnail or the setting in the style sheet.

width
The width of the thumbnail image. This value defaults to the width of the thumbnail or the setting in the style sheet. To display an image proportionately, set this value to ‘auto’;

gridwidth
The width of the grid. this value defaults to the width of the grid area or to the setting in the style sheet.

maxgridwidth
The maximum width of the grid. This is the better option to use when aligning grid left/right/center if you want the grid to wrap

showcaption
Set showcaption=FALSE to hide the captions showcaption defaults to TRUE

captionheight
This value sets the caption height and hides the overflow (if there is more text than can fit into the caption area, it will not be visible). The display defaults to one line of text or the value in the style sheet.

captionwidth
The caption width. This value defaults to the width variable above or to the setting in the style sheet.

wraptext
Wrap the text in the caption. Normally the text is limited to one line and overflow is indicated by an elipses. Please note that, to avoid a misaligned grid, you should set a caption height when wrapping text in a grid that has more than one row. wraptext defaults to FALSE

aligngrid
When the gridwidth value is set, set this value to left, right,  center or autocenter (uses jQuery)

imagesize
Media Image sizes are configured in the wordpress admin panel under Settings/Media. You can use any size in the plugin. The default value is ‘thumb’. thumb thumbnail medium large post-thumbnail (To proportionately size images, try setting the height="100%" width="auto")

Added support for codex features that were not loading through the shortcode:

before
show posts before a specific date. As a feature of this plugin, you can set this field to before="today"

after
show posts after a specific date. As a feature of this plugin, you can set this field to after="today"

inclusive
include the before and/or after date in the query

post__not_in
exclude posts (comma delimited id's) in this list

post__in
include posts (comma delimited id's) in this list

post_parent__in
include posts (comma delimited id's) with parent id's in this list.  Would be handy for post_type="page"
post_parent__not_in
exclude posts (comma delimited id's) with parent id's in this list.  Would be handy for post_type="page"

tag_slug__and
include posts (comma delimited strings) with tags that match all of the tag slugs in this list.

tag_slug__in
exclude posts (comma delimited strings) that have a tag that matches any of the tags in this list

debug_query
for advanced users or upon request for support purposes, set debug_query=true to view the SQL query.

== Installation ==

Download the Thumbnail Grid Plugin

How to install this plugin

Method 1:
Install this plugin using the built-in plugin installer:
Go to Plugins > Add New.
Under Search, type “Thumbnail Grid”
Click Install Now.
A popup window will ask you to confirm your wish to install the Plugin.
Click Proceed to continue with the installation. The resulting installation screen will list the installation as successful or note any problems during the install.
If successful, click Activate Plugin to activate it, or Return to Plugin Installer for further actions.

Method 2:
Download the plugin. In the WordPress admin panel, click on Plugins. Select Add New to get to the “Install Plugins” page. Click on browse and choose the downloaded file.

Click on the “Install Now” button to install the plugin. Once the plugin is installed, select “Activate Plugin”.

Method 3: (Advanced Users):

Unzip the file. Using FTP, upload the thumbnailgrid folder to the contents/plugins folder in your wordpress directory.



== Frequently Asked Questions ==

Please visit the FAQ page on our site at <a href="http://www.shooflysolutions.com/faq/">http://www.shooflysolutions.com/faq/</a>

- Only 10 thumbnails display at once no matter what I do

WordPress uses posts per page to control how many posts show up (In "Readings Settings", look at "Blog pages show at most". You will see that it is set to 10.

To override this in the thumbnail plugin, use a fixed value for posts_per_page or try setting the posts_per_page value to ’999′. All of the thumbnails for your posts (as long as you do not have more than 999 posts), should display.

This should work:

[thumbnailgrid posts_per_page ='999']
- How do I control the number of thumbnails that appear? -
This plugin is not designed to show several pages of thumbnails, rather it is designed to allow you to embed thumbnails into any page or to display a subset of thumbnails on a page. To show more thumbnails on a page than the default value "Blog pages show at most" (See the second screenshot on the screenshot tab), use a fixed value for posts_per_page or try setting the posts_per_page value to ’999′.

- I can't add a thumbnail to my posts.-
Your theme must be enabled for post thumbnails.

- How do I change the Height & Width on a single post or page?
You can now change the height and width in the short code, allowing you to override the style sheet width and height. Use auto to retain proportional sizing in the grid.

[thumbnailgrid height="200px" width="auto"]

- How do I change the Height & Width of the thumbnails for all posts and pages?


You can install a custom css plugin (do a search for the plugin Simple Custom CSS). Once installed, it should show up in your Appearance menu. Using the Custom CSS plugin:

Copy & Paste the styles below. Replace the width and height with the width and height that you would like to use. You can also change the space around the thumbnail by changing the padding. !important ensures that your custom style will have priority over the default style.

Start Copy & Paste Below this line

.postimage,
.postimage img {
width: 150px!important;
height: 150px!important;
}
.griditemleft {
width: 150px!important;
padding: 10px!important;
}

End Copy & Paste Above this line
Save this change. When you are testing your view, make sure that you refresh the page. If you mess it up, just delete it and start over.

- How do I center the grid on individual posts or pages?

You must set the width of the grid in order to center it. You can set the grid width in the shortcode by using the gridwidth in the shortcode.

[thumbnailgrid gridwidth="500px"]

How do I center the grid on all pages?

If your theme does not have a custom css module, you can install a custom css plugin (do a search for the plugin Simple Custom CSS). Once installed, it should show up in your Appearance menu. Using the Custom CSS plugin:

Using custom CSS, you must add a width to thumbnailgridcontainer. This can be a percentage.

Example 1:

.thumbnailgridcontainer {

width: 500px!important;
}

Example 2:
.thumbnailgridcontaner
{

    width:80%!important;
}
End Copy & Paste Above this line
Save this change. When you are testing your view, make sure that you refresh the page. If you mess it up, just delete it and start over.

Visit the Web Site (and the Support page on Wordpress) for more tips: http://www.shooflysolutions.com/software/featured-image-thumbnail-grid-for-wordpress/

== Screenshots ==

1. This is a screenshot taken from our old web site. Please visit http://www.shooflysolutions.com to see the thumbnail demos.

2. To view or modify "Blog Pages Show at most, go to the reading section of your Wordpress Settings

3. Settings page - Settings for the Thumbnail Grid can be found under the Settings Menu

== Changelog ==
* =Version 6.6.1
= Update tested through date
* =Version 6.6
* =Add option to use the alternate text as the title.
* =Version 6.5
* =Update version information
* =Tell users about our new plugin
* =Version 6.4
* =Fix introduced bug
* =Version 6.3
* =Use taxonomy for the category instead of cat for posts
* =Version 6.2
* =Allow category as alternative to cat
* =Allow debug as alternative to debug_query
* =6.1
* Fix description
* add script kiddies control
* =6.0
* Added post id data to thumbnail for javascript
* Fix default values
* Fix missing id for thumbnail grid
* Fix processing of boolean values
* Add has_thumbnails setting
* Remove support for bookmarks
* Better script loading
* =5.5
* Add ability to open links in new page, target shortcode (target ="_blank")
* Fill in missing alt from links
* =5.4
* Add missing javascript for autocenter
* Fix autocenter when number of items in grid is less than can fit in content
* Fix some of the __not_in code, not working natively
* =5.3
* Grid now has a class for the page. This is only unique if there is only one grid on the page.
* Add new filter to modify the title
* Fix filter for text under the title
* New param maxgridwidth. You can now set maxgridwidth instead (or with) width. This will enable grid to wrap when using aligngrid.
* Fix post_parent__not_in
* New param aligngrid="autocenter" - Uses jQuery to keep the grid centered for themes where centering is not working.
* Another fix for empty settings
* =5.2
* Fix broken settings
* = 5.1
* Fix thumbnail grid with no paramaters does not display with defaults.
* Default thumbnail (wp-includes/media/default.png) now displays for posts created without a featured image media id. * = 5.0
* Add support for codex features that were not functional (page__in, before, after, tag_slug__and, tag_slug__in, post_parent__in, post_parent__not_in )
* Add ability to display posts created before or after a today.
* Add code to enable dump of query (debug_query)* = 4.0
* Add settings & setting page for loading style sheets in header or footer - option to load compressed style sheet.
* = 3.1.1
* Remove nags.
* = 3.1
* Another Version number change to try to get plugin back onto wordpress repository?
* = 3.0.1 -
* Remove update checker
* = 3.0.0 -
* Added filters to plugin for Extensions.
* New shortcodes aligngrid, gridwidth, captionheight, displaycaption and imagesize.
* = 2.1.2 - Remove comments that (we think) wordpress is changing to <p>carriage returns.</p>
* = 2.1.1 - Fix to style sheet
= 2.1 =
* Fixes for height & width, minor modifications
* Add gridwidth attribute to shortcode
= 2.0 =
* Add functionality that enables users to center grid. See instructions.
* Add height & width attributes to shortcode for individual thumbnail grid.
= 1.2 =
* Fix incorrect thumbnail image loading
= 1.1 =
* Remove extra quote after link title
= 1.0 =
* Original Release



== Arbitrary section ==

Need more? Customization is available. Contact sales@shooflysolutions.com for more information.