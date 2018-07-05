# Footnotes, Citations and References

## **References**

`{ref id|first|repeat}citation{endref}`

This general form is used for both numeric and parenthetical form documentation styles. Although is is not blocked by the wiki engine, mixing the two styles on a single page may produce undesired results.

* **id** is an author assigned unique identifier made of alphanumeric characters for the specified Citation Information. The id is optional, and not needed if the reference is the only one to the citation. The id is internal to the page, and is not displayed to a viewer.
* **first** is specified only if a parenthetical reference is desired. The text of first is shown enclosed in parenthesis for the first reference to a citation, as a link to the Citation Information in the reference list.
* **repeat** is also specified only for parenthetical references. The text of repeat is used for subsequent references to a citation, usually as a condensed version of the more detailed first reference. If not specified, the first value will be used instead.
* **citation** is the source cited for this reference. The reference will produce a link to this citation in the reference list. Citation can contain wiki markup to format the display in the list.

  For repeated references to the same citation, only the id is considered.

## **Numeric Style**

`{ref}Wiki Author, //Example One, a simple one time citation//, 2013.{endref}`

This shows the simplest form of reference.1

`{ref my1}Wiki Author, //Example Two, a repeated citation with an "id"//, 2013.{endref}` `{ref my1}{endref}`

Sometimes you need to make more than one reference to a citation.2 This shows how this can be accomplished2 quickly and easily.

## **Parenthetical Style**

`{ref |Wiki Author, 2013}Wiki Author, //Example Three, a parenthetical citation//, 2013.{endref}`

This shows a simple one time parenthetical citation. \(Wiki Author, 2013\)

```text
{ref cmos|The Chicago Manual of Style Online|Chicago-Style}The Chicago Manual  of Style Online, "Chicago-Style Citation Quick Guide", Accessed April 25, 2013, 
[[http://www.chicagomanualofstyle.org/tools_citationguide.html]]{endref}
{ref cmos}{endref}
```

Formatting of the actual citation can be accomplished using normal wiki markup, based on your chosen style guide. In some guides the numeric style is called notes and bibliography, while the parenthetical style is known as author-date \([The Chicago Manual of Style Online](http://localhost/257geek/modules/gwiki/admin/pages.php?page=Help:References&op=display#ref3)\). There are many ways to format and reference citations, and the formatting can vary based on the type of source being cited \([Chicago-Style](http://localhost/257geek/modules/gwiki/admin/pages.php?page=Help:References&op=display#ref3)\).

## **Reference List**

To display the citations collected in you can use this command: {reflist} 1. Wiki Author, Example One, a simple one time citation, 2013. 2. Wiki Author, Example Two, a repeated citation with an "id", 2013. Wiki Author, Example Three, a parenthetical citation, 2013. The Chicago Manual of Style Online, "Chicago-Style Citation Quick Guide", Accessed April 25, 2013, [http://www.chicagomanualofstyle.org/tools\_citationguide.html](http://www.chicagomanualofstyle.org/tools_citationguide.html)

