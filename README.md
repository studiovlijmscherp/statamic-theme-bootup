# Bootup: Statamic starter Theme
Minimalistic Bootstrap theme for use with Statamic

## Why should I use this theme instead of the default included (CDN) version?
Simple; this theme uses the latest Bootstrap version (4.1.1), installed locally and ready for your own customizations :-)
It includes up-to-date Bootstrap 4 partials, and more.

## Installing
- Drop the theme folder 'bootup' into your site/themes directory
- Go to the /site/themes/bootup folder in your terminal
- Run *npm install* or *yarn install*
- Run *gulp init*
- Run *gulp* (this starts a watcher which re-generates JS and CSS on-the-fly)
- Change the active theme by heading to Theming settings in the Control Panel, or by changing theme in settings/theming.yaml.
- Refresh your site and you should see the new theme.

## Included
- latest Bootstrap (4.1.1)
- Gulp build-process concatenates all SCSS to one minified CSS file
- Gulp build-process concatenates all JS to one minified JS file
- Bootstrap 4 navigation bar Partial
- More partials to come!

## What does this 'build proces' do?
It generates new CSS (bootup.css) + JS (bootup.js) everytime you modify files in the *bootup/src* folder. In de *bootup/src* you will find the following folders and files:

- js/vendor.js (this file is generated by Gulp and contains bootstrap.js and slick.js)
- js/site_scripts.js (place your own JS in here)
Any .js file added to the src/js/ folder will be included in the bootup.js file
- scss/bootup.scss (this is the only file used for generation of the bootup.css file. Add any @imports you like into this file)
- scss/modules/_variables.scss (this is the Bootstrap variables file. Modify anything you like. This file is copied once when running *gulp init*)
- scss/vendor/_external.scss (add your vendor @imports in here)