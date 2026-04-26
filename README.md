# Nomad World Map

- **Contributors:** urban1702
- **Stable tag:** 1.4
- **License:** GPLv2 or later
- **License URI:** http://www.gnu.org/licenses/gpl-2.0.html

Create your own custom travel map. Link locations on the map to blog posts and share your travel plans.

## Description

For each location that is added to the map you can set the type of content you want to show. Either the excerpt of a blog post, a short custom description or only the travel dates.

The location content itself is shown in a carousel underneath the map. When you slide through the carousel the map will automatically zoom to the location that is linked to the visible content.

### Features include

- Create multiple independent maps
- Add multiple maps to the same page
- Style your map
- A sidebar widget that can show your last location
- Show a list of visited locations with optional arrival and departure dates
- Set custom thumbnails for each location
- Set custom line colors for the past and future travel routes
- Rearrange the order of the travel route by dragging the items up or down in the route list
- Specify if you want the map to zoom to the first or last location of your travel route
- Choose from three different content types for each location: link to a blog post, write a custom description or show the travel dates

If you want to contribute to the development of this plugin, you can do so through [GitHub](https://github.com/nomadworldmap/nomad-world-map).

## Installation

1. Upload the `nomad-world-map` folder to the `/wp-content/plugins/` directory.
2. Activate the plugin through the `Plugins` menu in WordPress.
3. Create your route on the map under `Nomad Map`.
4. Add the map to a page with this shortcode: `[nwm_map]`.

## Frequently Asked Questions

### How do I add the map to a page?

Add this shortcode `[nwm_map]` to the page where you want to display the map.

### How do I add multiple maps to a page?

You add the shortcode like you normally would, only this time you also need to define the map ID.
So if you want to show the maps with ids 1, 4 and 5 you would add the following shortcodes:

- `[nwm_map id="1"]`
- `[nwm_map id="4"]`
- `[nwm_map id="5"]`

### Can I specify the dimensions of the map?

Yes, just add the width and height as an attribute to the shortcode: `[nwm_map height="500" width="500"]`.

### How do I specify which map is shown?

You can add the `id` attribute to the shortcode `[nwm_map id="3"]`. This will show the map with ID 3 on your page.

### I created a route and added the shortcode to a page, but when I view the page in the browser it only shows a blank map?

Make sure your theme does not use AJAX to navigate between pages; if so, try to disable it. Also make sure there are no [JavaScript](http://codex.wordpress.org/Using_Your_Browser_to_Diagnose_JavaScript_Errors) errors on your site. Last thing you can try is to switch to another theme and disable other plugins and see if that fixes it.

### What other shortcode options exist for individual maps?

- Set zoom level: `[nwm_map zoom="6"]`
- Set content type (`tooltip` or `slider`): `[nwm_map content="tooltip"]`
- Disable lines between markers: `[nwm_map lines="0"]`
- Set map type: `[nwm_map maptype="roadmap"]` (other values: `satellite`, `hybrid`, `terrain`)

If the zoom level, content type, lines or map type are not set in the shortcode, the values from the general settings page are used.

### Can I show a list of all the destinations on the map?

Yes, this shortcode `[nwm_list id="1"]` will show the destination list for the map with id 1. If no id is set, it will default to 1.

Other shortcode options for the list:

- `[nwm_list id="1" dates="all"]` Show both arrival and departure dates
- `[nwm_list id="1" dates="arrival"]` Only show arrival dates
- `[nwm_list id="1" dates="departure"]` Only show departure dates
- `[nwm_list order="asc"]` or `[nwm_list order="desc"]` Change the sort order of the destination list

### When I search for a blog post title it returns no results?

Make sure the blog post you search for is published, and that it matches exactly with the title you see in the blog post editor. Otherwise please open a support request in the support form.

## Screenshots

1. Front-end of the plugin
2. Settings screen
3. The route editor

## Changelog

See [CHANGELOG.md](./CHANGELOG.md).
Nomad World Map
===============

This repository is intended for developers to browse the code and to contribute to 
the development of Nomad World Map. 

Support
-------
If you need support, then please don't post it here but use the
[support forums](http://wordpress.org/support/plugin/nomad-world-map) instead. 

The documentation can be found [here](http://wordpress.org/plugins/nomad-world-map/faq/).
