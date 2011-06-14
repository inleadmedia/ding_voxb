VoxB module
==========
This module provides capability for the user to review, tag and rate on an item in Ding! through the VoxB service.

Installation
-----------------
1. Include the module in `ting/ting_object_details.tpl.php`.
2. Activate the module.
3. Configure the module with the values given as examples.

Improvements
----------------------------------
In order to make the item landing page look & feel nice, content types for showing VoxB is needed ([Chaos tool suite] [ctools]?).

At this moment the module is included in `ting/ting_object_details.tpl.php`.
This is not the right solution.

* Replace the SOAP client with [NanoSOAP] [nanosoap].
* Integrate the possibility of logging requests.
* Refactoring of CSS class names to not use camelCase.
* Model the pagination over [theme_pager] [theme_pager].
* Refactor the JavaScript to the behavior of drupal.js.
* Major template changes.
* Various fixes (AJAX, naming, spaces, etc.).

VoxB related issues
-----------------------------
### Current deficiencies in the service:
* `updateMyRequest` needs all former posts in the request.
* The VoxB-service is slow.
* Reviews and tags are not sorted after date of creation.

### Current features to the service:
* Expand error messages, eventually with error codes (only 2 messages exist at the moment).
* More documentation.
* Abolish several user profiles.
* Lists and user lists (highest rated items, mostly reviewed items, popular items, etc.).
* Rating of reviews in order to hide inappropriate reviews.

[ctools]: http://drupal.org/project/ctools
[nanosoap]: http://drupal.org/project/nanosoap
[theme_pager]: http://api.drupal.org/api/drupal/includes--pager.inc/function/theme_pager/5
