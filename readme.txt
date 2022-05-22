========
Go to git repo https://github.com/alialaa/wp-blocks-course-boilerplate
Terminal go to plugins folder and clone above repo.
Name of file must match main plugin file textblock textblock.php
Create a block
Rename and Update the comments in the main plugin file in this case boilerplate.php
Index.js change the register block function
create-block/boilerplate to block-course/text-blcok
git clone https://github.com/alialaa/wp-blocks-course-boilerplate.git nameofblock text-block
git remote -v will show the git repo above but we cannot push to it bc it is not ours and we want to keep it for a great beginning.
git remote rename origin upstream basically renaming the origin branch to upstream strange I know
git remote add origin https://github.com/melissaspiegel/jule.git
Open up block.json update info
* Change register block function in index.js change 
    * create-block/boilerplate
    * To 
    * Block-course/text-block
    * mwm-text/text-block
    * Rename boilerplate.php file which is the main plugin file to text-block.php
    * Change the info in the comment of text-block.php
    * Change function to match our new prefix and block name 
        * Change from create_block_boilerplate_block_init
        * Change to 
            * mwm_text_text_block_block_init
            * BAD NAMING ON MY PART
*         npm install 
* npm run start to compile 
* Got to WordPress admin and activate plugin - YAY!




origin    https://github.com/melissaspiegel/jule.git (fetch)
origin    https://github.com/melissaspiegel/jule.git (push)
upstream    https://github.com/alialaa/wp-blocks-course-boilerplate.git (fetch)
upstream    https://github.com/alialaa/wp-blocks-course-boilerplate.git (push)
IT-USA-B00704:text-block mspiegel$ git add -A
IT-USA-B00704:text-block mspiegel$ git commit -m"added vscod confi"
On branch main
Your branch is up to date with 'upstream/main'.
nothing to commit, working tree clean
IT-USA-B00704:text-block mspiegel$ git push -u origin main
Enumerating objects: 92, done.
Counting objects: 100% (92/92), done.
Delta compression using up to 16 threads
Compressing objects: 100% (44/44), done.
Writing objects: 100% (92/92), 718.03 KiB | 718.03 MiB/s, done.
Total 92 (delta 43), reused 92 (delta 43), pack-reused 0
remote: Resolving deltas: 100% (43/43), done.
To https://github.com/melissaspiegel/jule.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.
IT-USA-B00704:text-block mspiegel$ 



=== Boilerplate ===
Contributors:      The WordPress Contributors
Tags:              block
Tested up to:      5.7.0
Stable tag:        0.1.0
License:           GPL-2.0-or-later
License URI:       https://www.gnu.org/licenses/gpl-2.0.html

Example block written with ESNext standard and JSX support – build step required.

== Description ==

This is the long description. No limit, and you can use Markdown (as well as in the following sections).

For backwards compatibility, if this section is missing, the full length of the short description will be used, and
Markdown parsed.

== Installation ==

This section describes how to install the plugin and get it working.

e.g.

1. Upload the plugin files to the `/wp-content/plugins/boilerplate` directory, or install the plugin through the WordPress plugins screen directly.
1. Activate the plugin through the 'Plugins' screen in WordPress


== Frequently Asked Questions ==

= A question that someone might have =

An answer to that question.

= What about foo bar? =

Answer to foo bar dilemma.

== Screenshots ==

1. This screen shot description corresponds to screenshot-1.(png|jpg|jpeg|gif). Note that the screenshot is taken from
the /assets directory or the directory that contains the stable readme.txt (tags or trunk). Screenshots in the /assets
directory take precedence. For example, `/assets/screenshot-1.png` would win over `/tags/4.3/screenshot-1.png`
(or jpg, jpeg, gif).
2. This is the second screen shot

== Changelog ==

= 0.1.0 =
* Release

== Arbitrary section ==

You may provide arbitrary sections, in the same format as the ones above. This may be of use for extremely complicated
plugins where more information needs to be conveyed that doesn't fit into the categories of "description" or
"installation." Arbitrary sections will be shown below the built-in sections outlined above.
