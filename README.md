Apache/Javascript Site Redirector
=================================

As a sysadmin, I've had to redirect site X to site Y because
of some merger or aquisition more times than I can count.

Here's the latest incantation of this sysadmin magic:

1. Create an Apache config that uses [mod_rewrite](http://httpd.apache.org/docs/current/mod/mod_rewrite.html) to funnel all requests into a single HTML page.

2. Have the javascript in that page extract the URI and redirect it to the new sitename.

Included is [redir.conf](redir.conf) which is a sample Apache config and [redirect/index.html](redirect/index.html) with basic javascript that will do the job. If you want to put images in the HTML, place them in the redirect directory as well and use absolute references to them in the IMG tags.

Notes
-----
This method is not "SEO friendly", but it will get you to clean up your old bookmarks.
