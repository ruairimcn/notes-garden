A [[WordPress]] Plugin Deactivation Debug is a process where you deactivate some or all plugins on a WordPress website in order to debug an issue.

In general, plugins work well together, but sometimes conflicts can arise. You can avoid conflicts by only instal plugins that have some or all of these traits: 
1. Are made by a reputable developer
2. Have a high rating
3. Have a high number of installations


# Doing the debug
## 1: Turn on wp-debug
Edit wp.config and turn on/off the options as needed

wp-debug
This can be true or false. Turning this on is a prerequisite to the following two working.
This starts the debug feature of WordPress where errors are recorded.

wp-debug-log
This can be true of false. Turning this on causes WordPress to create a file in
/wp-content/wp-debug.txt
where all debug errors are recorded

wp-debug-display
This can be true or false. Turning this on causes WordPress to display errors on the front-end of the website. i.e. not good to turn on for a live website.


## 2: Look for clues in the debug log
Turn on wp-config-debug and look through the error log for clues, i.e. the name of the plugin's folder in the error log line. If you disable the plugin in question by simply renaming its folder to something else, this will often fix the issue in question, and you'll have to either fix the issue by updating various plugins and hoping that fixes it, or having to replace this plugin with a different one. 


## 3: Mass disable all plugins
If step 2 doesn't work for you, try disabling all plugins. 
1. First, make a note of what plugins are enabled so you can revert to your previous setup easily.
2. Disable all plugins.
3. Re-enable plugins one by one, checking to see if the error has returned each time. Make sure all kinds of caching are disabled (you can specify caching to be disabled at the browser level from inside the Inspector of most modern browsers)

If the problem persists:
- Revert to a default WordPress theme to see if the theme is the issue
- Re-install WordPress
- Open a support ticket with your hosting company
- Continue to look for clues in the debug log
- [[Google the problem]]


---
**Links**:: 
**Tags**:: 

**Sources**::

**Date created**:: 2021-07-10  
**Time created**:: 11:51