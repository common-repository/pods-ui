=== Pods UI ===
Contributors: sc0ttkclark
Donate link: http://podsfoundation.org/donate/
Tags: pods, ui
Requires at least: 3.1
Tested up to: 3.2.1
Stable tag: 0.7.5

Please use the Pods plugin instead, Pods UI was integrated within it as of Pods 1.10.

== Description ==

*NOTICE: Pods UI is included in Pods core as of Pods 1.10, you don't need a separate plugin anymore! Look for future features and bug fixes within Pods core*

Information about Pods UI can be found at http://podsframework.org/codex/pods_ui_manage/

== Changelog ==

= 0.7.5 - July 27, 2011 =
* Minor Bug fixes - this will be the LAST separate release of Pods UI, it is now included in Pods core as of Pods 1.10!

= 0.7.4.1 - July 24, 2011 =
* FIXED: Duplication feature updated to fit code update in publicForm (pod_id + tbl_row_id)
* FIXED: Fixed action links to apply_filters before checking if it's empty
* FIXED: Fixed heading / value handling
* FIXED: 'bool' now accepted as coltype in addition to 'boolean' to match Pods
* FIXED: Fixed validate notice reference in demo.php plugin

= 0.7.4 - June 23, 2011 =
* ADDED: Added support for filters besides PICK - bool (checkbox), txt / num / slug / desc / code (text box) for additional filtering
* FIXED: Fixed filters
* FIXED: Demo plugin updated with better plugin validation (checking to see if Pods and Pods UI are activated)

= 0.7.3.1 - April 5, 2011 =
* FIXED: Fixing sorting

= 0.7.3 - April 5, 2011 =
* FIXED: Fixing sorting

= 0.7.2 - April 1, 2011 =
* FIXED: Fixing filters

= 0.7.1 - March 8, 2011 =
* FIXED: Reordering bug fixed
* FIXED: Reset Sort link now shown to the left of 'Show per page' when Usermeta-based Sort is enabled

= 0.7.0 - March 4, 2011 =
* ADDED: For Management screens, Searching now searches across all non-pick fields by default (you can enable pick field search by setting search_across_picks=true in the Pods UI options, or disable searching across fields by setting search_across=false)
* ADDED: Session-based Persistence for Searching and Filtering (by specific Management panel)
* ADDED: User-based Persistence for Sorting and Show Per Page
* ADDED: Searching / Filtering / Pagination now available for the Reorder panel of Pods UI

= 0.6.8.14 - September 9, 2010 =
* FIXED: URLs became overly complex when using filters and other links

= 0.6.8.13 - August 26, 2010 =
* ADDED: Multi-access check in edit_where

= 0.6.8.12 - August 23, 2010 =
* ADDED: On Add, two new links show up (Add another + Add another based on this)
* FIXED: On Save, redirected to the wrong URL (missing ID)
* FIXED: Display Helpers used in 'columns' were doubled, causing issues with display of value

= 0.6.8.11 - August 13, 2010 =
* FIXED: Fixed form, was display "; instead of the actual form

= 0.6.8.10 - August 13, 2010 =
* ADDED: Support for Multisite Environment URLs
* ADDED: action_after_save option to customize which action is used after save (set to 'manage' to go back to the Manage screen on add / save / duplicate)
* ADDED: delete_where option to customize when a user can delete an item based on the item's value
* FIXED: edit_where / duplicate_where / delete_where now check before showing their corresponding URLs in Manage screen
* FIXED: Column display_helper now runs during $object->fetchRecord() loop instead of after

= 0.6.8.9 - August 8, 2010 =
* ADDED: Duplication (enabled by default)
* ADDED: View links, now you can View Pod Items (if detail_url is defined in the Pod settings)
* FIXED: demo.php activation issues
* FIXED: Delete this item now only appears when Editing
* FIXED: Enhanced action link building, added some parameters to allow for more customization

= 0.6.8.8 - July 30, 2010 =
* FIXED: Bug fix release

= 0.6.8.6 - July 29, 2010 =
* ADDED: Delete this item link now added to the form save button (on Edit only, and only if 'delete' is not disabled)
* ADDED: Full API integration with Pods API (delete, reorder), removed pods_ui_save_rel()
* ADDED: Standardized demo.php Validation and Activation processes
* FIXED: Full support for Pods 1.9.0 (Pods UI no longer supports versions previous to Pods 1.9.0)
* FIXED: Moved reordering into Pods API in core
* FIXED: Bug fixes on 'updated' and 'search' to work on multi-level ('num')
* FIXED: Bug fixes for 'updated' and 'search' to remove them from appearing in the URLs outside of 'manage'

= 0.6.8.7 - July 29, 2010 =
* FIXED: Bug fix release

= 0.6.8.5 - July 16, 2010 =
* ADDED: 'icon' option added for defining custom icon for page headings
* FIXED: move.png location updated for Pods 1.8.9

= 0.6.8.4 - July 8, 2010 =
* FIXED: api.php sanitization using pods_sanitize() and cleaned up code
* FIXED: Updated demo.php package to ensure compatibility with Pods 1.8.9
* FIXED: 'updated' and 'search' no longer persist in the URL when navigating between Add / Edit / Manage
* FIXED: 'browse' changed to 'manage' in integration with Pods 1.8.9 changes

= 0.6.8.3 - April 28, 2010 =
* FIXED: pods_ui_coltype now properly supports columns with . in it (like pick columns)

= 0.6.8.2 - March 17, 2010 =
* FIXED: UI option 'item' now defaults to "Item" to avoid weird naming from a Pod name
* FIXED: Error messages now appear in Red instead of Yellow
* ADDED: $object->data is now set, so you can reference other fields within your Display Helper
* ADDED: Message now appears in Yellow at top when an item is successfully saved in Add / Edit forms

= 0.6.8.1 - February 18, 2010 =
* FIXED: Formatting of Pagination for when there are no records
* FIXED: Formatting of Pagination area, the html tags weren't placed normally
* FIXED: findRecords() now uses the LIMIT fix
* ADDED: Updated Compatability, works in WP 3.0

= 0.6.8 - February 1, 2010 =
* ADDED: Pods UI will now take over the default Edit / Add New pages of Pods when the Pod is set to Top Level Navigation
* ADDED: Error Reporting if pods_ui_manage() / pods_ui_form() doesn't have an object to work with
* FIXED: Add New button needed to reset current num id
* FIXED: Sanitized sort and limit parameters in findRecords()
* FIXED: Reorder API now checks if user has access to Pod
* FIXED: pods_ui_save_rel() needed small tweaks to avoid errors when not enough info was passed

= 0.6.7 - January 8, 2010 =
* ADDED: Drag and Drop Reordering of items
* ADDED: Show per page option

= 0.6.6 - January 2, 2010 =
* ADDED: Reset Filters option when 'filters' / 'search' are active
* ADDED: You can now enable 'filters' / 'custom_filters' but disable the search box by setting 'search' to false
* ADDED: pods_ui_var now supports arrays for bulk checking
* FIXED: Activation requirements removed as they caused too many issues across multiple PHP configurations; replaced within main functions themselves
* FIXED: Added 'item' reference in Demo UI variables to give a better example
* FIXED: Filters to not all be selected, leaving the default value to be the correct field label
* FIXED: Filters that have no data will not be shown
* FIXED: Filters now compatible with updated get_dropdown_values from the Pod class (as of Pods 1.7.9)
* FIXED: Name / Created / Modified now support the display_helper option

= 0.6.5 - - December 7, 2009 =
* FIXED: Filters not working because $val was being used instead of $value
* FIXED: Made sure the Filters option could be provided as a string separated by comma (for those using the query string method)

= 0.6.4 - - December 2, 2009 =
* FIXED: Filter now filters correctly based on field_name instead of key from array (thx to patrickheeney)
* FIXED: Removed Pods UI long internal documentation from header of pods-ui.php file, this is now all within the User Guide
* FIXED: Updated demo.php to have Latest Pods Version in Package

= 0.6.3 - November 24, 2009 =
* ADDED: Pods UI now checks to see if the Pods CMS plugin is installed
* ADDED: demo.php now checks to see if the Pods CMS / Pods UI plugins are installed

= 0.6.2 - November 14, 2009 =
* ADDED: SQL Option for customizing findRecords() on Manage screen
* ADDED: "Back to Manage" link on Add / Edit form pages