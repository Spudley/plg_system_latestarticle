LatestArticle
=============

This plugin allows you to create a 'latest article' URL for each of your categories.

It works by intercepting page requests to addresses matching the specified pattern, and re-routing them to the newest article in the requested category.

Note that it only enables the URL; it does not actually place the links to the latest article URLs on your site; it is up to you to do that separately, eg as menu entries.

Version History
----------------

* 1.0.0


Installation
----------------

This is a standard Joomla plugin. Installation is via Joomla's extension manager. As with all plugins, remember that it must also be activated after being installed.


Usage
----------------

Firstly, set the URL pattern you want for the latest article links. The default value for this is `[category]/latest`, which should be a good starting point. You may change it though if you wish.

Now simply navigating to `http://yoursite.com/mycategory/latest/` will result in the request being redirected to the newest article in the `mycategory` category.

You may now add menu entries or other links pointing to this URL in order to use your random links.


Motivation
----------------

This plugin was written after searching for an existing one to do the job proved fruitless. The functionality to load the latest article is in Joomla already, but I couldn't find an easy way to create a fixed URL that always goes to the newest article, so I wrote the plugin. It helped that it is similar to another plugin I'd already written for random links.


Todo List and Known Issues
--------------------------

* Todo: Add caching to the DB query so we don't have to query the content table every time.
* Todo: I've not tested it with nested categories; I doubt it will work correctly.
* Todo: Add more options; eg only featured articles, or a choice of sort orders.
* Caveat: If you have an actual article with a title like `latest` that matches the redirect URL in this plugin, then they may clash. Try to avoid this.


License
----------------
As with all Joomla extensions and Joomla itself, this plugin is licensed under the GPL. The full license document should have been included with the source code.
