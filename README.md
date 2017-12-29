# Clear Page Cache
Simple Drupal 7 module to clear page cache only.

Useful when Drupal core caching is turned on, and you'd like to show your node edits immediately to anonymous visitors, but don't want to clear the entire cache.

The module adds a menu link (admin/clearpagecache "Clear Page Cache") and a role permission (use clear page cache).

The module is quite fast even for sites with many pages (1000+). Of course you empty the page cache entirely, so be mindful when using this module - all your pages will need to be cached again sometimes at the expense of page speed for the first anonymous visitor. TIP: Use a spider/crawler app to hit all pages (eg. "prime the cache") after emptying the page cache.

An alternative is the 'Clear Cache' module https://www.drupal.org/project/clear_cache, but I think it clears the entire cache as opposed to just the page cache.

## Installation
0. Download zip or git clone
1. Add module folder to "sites/all/modules"
2. Enable "clear_page_cache" module
3. Add "use clear page cache" permissions to any role you want (not "anonymous"!)
4. A menu link "Clear Page Cache" will appear in the administrative toolbar
