# SWTNDX

A lightweight* update for the look of your Apache directory listings (as 
generated by mod_autoindex).

**Examples**: [files.einserver.de](http://files.einserver.de) and [hsa.einserver.de](http://hsa.einserver.de/)



## Features

- Adds a breadcrumb based on the path segments
- Renders Readme files found in the current folder into a box at the beginning of the page
- Makes it easy to use your own CSS (or icons)



## Included Stylesheets

- Minimal
- Bootstrap (Based on Twitter Bootstrap)
- Apple OS (Mimics Finder / iOS table view) *early beta, may not work in every browser!*
- Uberspace (Inspired by <http://uberspace.de>) *beta*

To use the alternate stylesheets adjust the <code>$css</code> variable in <code>header.uihtml</code>



## Requirements

1. Apache with mod_autoindex installed
2. PHP > 5.2 (< 5 is should work, but who would recommend anything below 5.2?)
3. Support for .htaccess including allow_override



## Simple Installation

1. Upload the swtndx folder to the folder you want to make public (Attention: it contains a .htaccess file which might be invisble depending on your and the servers OS)
2. Also upload the **_.htaccess** and rename it to **.htaccess** (If you already have an .htaccess in your folder, please append the contents of _.htaccess to yours)
3. *Optional, but recommened* upload the robots.txt to lock out search engine spiders
4. Done.

If it doesn't work check everything (the file that was named 1_.htaccess might contain more information for you). 

If it still doesn't work get mad, throw things around. Then sit down and try again. Read the Apache docs: http://httpd.apache.org/docs/ 

Don't give up!



## Advanced Installation

If you consider yourself ready for the advanced installation, you should know what to do, but here are some tipps anyway.

- Upload the swtndx folder to any location on your server and use symlinks to add it to the folders you want to make public - Makes it easy to update.
- Don't upload. Use git and clone the repository, *then* use symlinks. Makes it even easier to update.
- Don't forget to check if your Apache has follow-symlinks enabled. If it doesn't, you can uncomment a line in the .htaccess that came with swtndx, it might be able to enable it for you.



## Version History

* v1.2 (20120229) Added a new default style sheet (Minimal) which is closer to the pre 1.0 default stylesheet and is smaller than the Bootstrap based one.
* v1.1 (20120106) Added early draft for new stylesheet which mimics the Mac OS X Finder and iOS
* v1.0 (20120104) re-release under new name, updated pretty much everything
* v0.5 Intermezzo, rewrote most of it
* v0.3 (20100201) bugfix: weird php error
* v0.2 (20100201) bugfixes: favicon, colours, copyright, robots.txt
* v0.1 (20100130) initial release



## Legal

This is provided 'as is' and I'm not responsible for anything you do with it. 
Thanks.

swtndx is licensed under the Creative Commons Attribution-Share Alike 3.0 Unported license http://creativecommons.org/licenses/by-sa/3.0/

### Icons 

The default icons are custom made by @kinaj exclusively for swtndx.
You are not allowed to use them elsewhere.
Contact @kinaj for your very own custom icons, he makes amazing things.
http://janikbaumgartner.com/

This script includes the Chalkwork icons set made by Dave Shea and available at http://chalkwork.com/ and are licenced under Creative Commons Attribution-NonCommercial-ShareAlike 3.0

### CSS

The bootstrap style uses http://twitter.github.com/bootstrap/


----

Thanks for reading. Florian Pichler, http://einserver.de