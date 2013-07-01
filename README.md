iG:MU-Plugins Loader
====================

This is a mu-plugin for WordPress which allows to keep your mu-plugins in their own directories for better organization. WordPress on its own loads only single files from mu-plugins root and ignores all files inside directories.

This mu-plugin allows plugin organization just like regular WordPress plugins where each mu-plugin can be inside its own directory and still be loaded into WordPress.

This has only one requirement to work; the plugin bootstrap file should have the same name as its directory and should have a ``` .php ``` extension. So if your plugin directory name is ``` my-uber-cool-plugin ``` then your directory structure would be like:

```
mu-plugins
	|_ ig-mu-plugins-loader.php
	|_ my-uber-cool-plugin				<- plugin directory
		|_ my-uber-cool-plugin.php		<- plugin bootstrap
		|_ some-other-file.php
```

