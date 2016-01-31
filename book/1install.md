# 1.0 Install/Uninstall

No special measures necessary, follow the standard installation process – extract the module folder into the ../modules directory. Install the module through Admin -> System Module -> Modules.

Detailed instructions on installing modules are available in the [Chapter 2.12 of our XOOPS Operations Manual](https://www.gitbook.com/book/xoops/xoops-operations-guide/)

# 1.1 Module Purpose

gwiki, the geekwright wiki, is a XOOPS module which implements a wiki based on the [**WikiCreole 1.0**](http://wikicreole.org/wiki/Creole1.0) specification. In addition to the basics as defined in the WikiCreole spec, the wiki features several powerful extensions, giving it great flexibility as a content authoring and presentation tool. It also features an equally flexible permission capability, making a single instance suitable for multiple collaborative efforts, each with their own policies.
This manual covers the wiki markup syntax and directives, as well as an overview of the available administrative options.

## Design Goals

- WikiCreole 1.0 compliant
- Extended directives for rich content for real world authoring needs.
- Flexible permissions enabling any model, be it open, closed, private or some other variation.
- Support multiple communities, each with separate permission models and visual distinctions.
- Be a native module for XOOPS, incorporating existing native capabilities
 - group permissions - control who can edit what
 - comments - discussions can take place outside of content if desired
 - notifications - multiple options to focus on the changes that interest you
 - blocks - make wiki content available across the site
 - search - integration with system search, search term highlighting
 - templates - add custom templates to groups of pages
- Multiple presentation options
 - Standard - regular module style access
 - Page shown in a Block - Use wiki pages for block content
 - AJAX powered Wiki in a Block - Embed a fully functional wiki in a block
 - Relocatable Wiki script - put the wiki it where you want it
-  Easy access to editing. The wiki editor can be accessed from wherever a page is displayed
- Easy Image and File Attachment functions can be accessed without leaving the page being edited.
 
## Why a Wiki?

There are those who think wikis are a relic from the past, an antique method to output HTML invented when HTML was considered intimidating. Actually, that is far from the truth. It is true that wiki markup results in HTML output. (Of course it does -- it targets a web browser, what else would it use?) And yes, it only allows some control over the resulting HTML. The critics miss the point that the wiki is an authoring tool, designed to make authoring of content easy, especially in a collaborative setting. These apparent limitations are essential ingredients to both making the authoring easy, and making the works of many appear as a uniform whole. Before dismissing the wiki, some research might be in order. This concept of easy to author extends to other solutions as well, such as **Markdown** which has gained widespread adoption, where the similarities in goals and syntax are striking.

A Wiki provides an environment where a community can collaborate on activities of importance to that community. It is more than a presentation tool. It is more than an HTML substitute. It is a proven technology for addressing the need to capture knowledge and ideas from a community. It empowers community members to make contributions, big and small, toward the community's growth and attainment of its goals.


