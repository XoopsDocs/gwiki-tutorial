# Blocks

**New Page**

This block allows the user to quickly enter a page name and invoke the editor, mainly useful as way to create a new page. This block is aware of the wiki permissions for the current user, and will only be displayed if the user has some edit permissions. The block is also sensitive to namespaces, and will display a selection list of namespaces the user has permissions for. Options \(none\)

**Page Display Block**

This block displays a page in a block. Any wiki links in the block will follow the default linking as established in **Help - Preferences**.

Options

* Show Full Page - If set to No, only the first portion of the page \(a teaser\) will be displayed. The page author can explicitly indicate where the teaser portion should end by including a {more} directive.
* Wiki Page to Load - The name of the page to show. It the random option is selected, this is used as a matching prefix to limit which pages can be chosen for display.
* Show a Random Page - If set to Yes, the page to load will be chosen randomly. The Page to Load option will be used as a prefix pattern to limit selections. This can be used, for example, to show only pages in a specific namespace.
* Show Default Image - If set to Yes, the image specified to represent the page, if any, will be shown. For pages with images in the teaser portion, it might be desirable to turn off the represent image.

**Recent Pages**

This block shows a list of recently modified pages. Options

* Number of Pages - Maximum number of changed pages to list.
* Namespace - Optional, if specified it is used to limit the list to a single namespace.
* Maximum age - Optional, leave blank to disable. Otherwise, this is used as an age limit. The option is used as an argument to the PHP strtotime\(\) function. An example would be "-30 days" to limit the display to changes within the last 30 days.

**Related Pages**

This block displays a list of related pages. Related pages can be created by specifying a parent page in the page editor. For more information see **Help - Page Sets and Relations**.

Options

* Max Number of Pages - maximum number of related pages to show
* Relation Page - Optionally specifies a specific page as the parent relation. Leave this blank to derive the relationship from currently displayed page. \(Note that the page is normally only specified while the user is in the gwiki module.\)
* Sort Pages by - select pages to display by popularity or the time last changed.

**Page Set TOC**

This block displays a Table of Contents for a page set. Page Sets can be created by specifying a page set home for pages in the page editor. For more information see **Help - Page Sets and Relations**.

This block also includes a search function. This search works like the normal system search, but it limits the search results to occurrences of the search terms in the displayed page set.

Options

* Levels of TOC to show - Limit how many levels of detail will be included in the displayed table of contents,
* Page Set to Load - Optionally specifies a specific page as the page set home. Leave this blank to derive the page set from currently displayed page. \(Note that the page is normally only specified while the user is in the gwiki module.\)

**Wiki in a Block**

This block displays a page in a block using AJAX loading. Any wiki links in the block will load the new page into the same block using AJAX. This AJAX Wiki is shown with Home and Back buttons allowing the user to navigate within a wiki subset as exposed by the initially specified page to load. This can be useful in situations where it is desirable to make information available to the user without forcing navigation away from the current page, such as help documents or other reference materials.

Options

* Wiki Page to Load
* URL to Remote gwiki module \(leave blank to use local wiki.\) A remote module must explicitly allow the remote access, established by the AJAX Wiki Allowed Origin in **Help - Preferences**.

**What Links Here**

This block displays a list of wiki pages that link to the currently displayed wiki page. Links are automatically recalculated as pages are saved.

Options

* Max Number of Pages - maximum number of related pages to show. Enter zero to show all links.
* Sort Pages by - select pages to display by alphabetic order, popularity or the time last changed.

