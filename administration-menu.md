# Administration Menu

## 2.0 Administration Menu

### Home and About

These sections check for issues with the wiki installation, and provide some information about the currently installed version

### Manage Revisions

In this section you can manage wiki page revisions. You can locate the page of interest either by paging through the data or using the Page Name Filter. The initial display shows the page name, title, number of revisions and a list of possible actions. Choosing history will show the details for each revision of a given page, again with a list of possible actions.

* **View** - display the selected page revision
* **History** - display a list of page revisions
* **Lock** or **Unlock** - The administrator may lock pages so that they may not be edited.
* **Delete** - delete a wiki page. Actually, this does not delete the page directly, but it marks all of the page revisions as inactive. The clean up process can be used to actually delete the pages from the database.
* **Restore** - make a given revision the current active page
* **Fix** - make a given revision the current active page, and delete all other revisions. This function does physically delete the inactive pages.
* **Tools** - bring up a tool which can be used to set the user id that last edited the page and/or the date time the page was last modified.

There are also actions which will show under the list of pages.

* **Clean up the database** - This option will physically delete all inactive page revisions older than the Minimum History Retention Days specified in **module preferences**. It is possible to automate this process, if desired, by calling the "cleanit.php" script in the wiki module directory using a cron job, such as an entry invoking something like "wget [http://xoops.example.com/modules/gwiki/cleanit.php](http://xoops.example.com/modules/gwiki/cleanit.php)" on a daily basis. If you do not want to purge the old history, the preferences option can also turn it off completely.
* **Partition** - If the page database grows to a very large size, it is possible that partitioning the table could give a performance boost. This option partitions the table such that all active pages are in one partition, while the inactive ones are in another. The results of this depend on many factors, and are not always positive, so treat with caution. Reversing this process \(removing the partitioning\) will require use of additional MySQL tools outside of the wiki module. More sophisticated partitioning strategies might be more appropriate depending on the nature of both your wiki database and the performance issues you are facing.
* **Add Help Pages** - Inserts these help pages into the wiki. This will also restore the help pages if they have been previously added and modified.

## Permissions

Wiki permissions are assigned by system group. There are two basic permissions, edit and create. Edit permissions allow one to edit an existing page, while create permissions allow one to create a new page.

Each of these permissions is further sub-divided by the qualifiers of any or namespace. Any permissions allows one to edit or create any wiki page, while Namespace permissions restrict the edit or create permissions to pages belonging to a namespace assigned to one or more of the user's groups.

## Namespaces

Namespaces provide a powerful set of options to manage your wiki. In the simplest form, namespaces are simply wiki pages with names in the form of namespace:page. The inclusion in a namespace enable more finely grained permissions, dedicating a portion of the wiki to specific authors. Namespaces also enable the possibility of a unique look through a custom page display template. It also becomes possible to link to another wiki with only the need for the author to enter the page name, instead of a full remote URL.

* Namespace - the name of the namespace
* Home Page - the home page for the namespace
* Enable Automatic Names - enable automatic date based naming for the namespace. This allows the author to create a page using just the namespace designation, and the system will create the page name portion. This can be useful for using the wiki in a blog or news type roll.
* Template - this is a full XOOPS template. When you opt to create a new template, it will default to a copy of the normal wiki view template. You can then modify that to add a different look and feel for pages in the namespace.
* External - indicate if this is an external \(interwiki\) namespace
* External URL Format - the URL template for the external wiki. This is a PHP sprintf\(\) string. The page name without the namespace portion will be passed as the only argument.
* Assigned Groups - this indicates groups that are assigned to this namespace. If a user is part of a group that is assigned to this namespace, and that group has been granted Edit Namespace and/or Create Namespace permissions, the user can edit and/or create pages in this namespace.

  **Attachments**

  This allows the administrator to review and search through files attached to wiki pages. The newest attachments are shown first.

  **Recent Activity**

  This shows the most recently modified pages in the wiki.

