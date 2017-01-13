<div id="wrap">

[Skip Navigation](loop_files_for_item.html#content)
<div id="header">

<div class="padding">

<span
id="logo">[![Omeka](http://omeka.org/ui/i/logo-horizontal-288px.gif)](../../index.html)</span>
<div id="search-form">

</div>

-   <div id="nav-showcase">

    </div>

    [Showcase](../../showcase.1.html)
-   <div id="nav-involved">

    </div>

    [Get Involved](../../index.html%3Fp=124.html)
-   <div id="nav-addons">

    </div>

    [Add-Ons](../../add-ons.1.html)
-   <div id="nav-forums">

    </div>

    [Forums](../../forums/topic/mysqli-stmt.bind-result.html)
-   <div id="nav-documentation">

    </div>

    [Documentation](http://omeka.org/codex/)
-   <div id="nav-download">

    </div>

    [Download](../../download.1.html)

</div>

</div>

<div id="content">

<div class="padding">

<div id="user-meta">

-   <div id="pt-login">

    </div>

    [Log
    In](http://omeka.org/c/index.php?title=Special:UserLogin&returnto=Functions/loop%20files%20for%20item)

</div>

Functions/loop files for item
=============================

<div id="contentSub">

<span class="subpages">&lt;
[Functions](../Functions.html "Functions")</span>

</div>

<div id="primary">

<span id="Description" class="mw-headline"> Description </span>
---------------------------------------------------------------

`loop_files_for_item()` provides a loop through the files, allowing you
to template things like lists of files associated with an item.

<span id="Usage" class="mw-headline"> Usage </span>
---------------------------------------------------

<div class="mw-geshi mw-content-ltr" dir="ltr">

<div class="php source-php">

``` {.de1}
<?php while(loop_files_for_item()): ?>
<!-- Template the file info -->
<?php endwhile; ?>
```

</div>

</div>

<span id="Arguments" class="mw-headline"> Arguments </span>
-----------------------------------------------------------

-   **\$item** (object) or null (default). If null, the current item
    is used.

<span id="Return_Value" class="mw-headline"> Return Value </span>
-----------------------------------------------------------------

Mixed. The current file within the loop, or null if at the end of the
loop

<span id="Examples" class="mw-headline"> Examples </span>
---------------------------------------------------------

### <span id="Creating_a_list_of_file_names_for_an_item" class="mw-headline"> Creating a list of file names for an item </span>

This example begins by creating an unordered list, then populating its
list items by using a while loop to step through the individual files.

<div class="mw-geshi mw-content-ltr" dir="ltr">

<div class="php source-php">

``` {.de1}
<ul>
    <?php while(loop_files_for_item()): 
        $file = get_current_file();?>
        <li><?php echo $file->original_filename; ?></li>
    <?php endwhile; ?>
</ul>
```

</div>

</div>

<div class="printfooter">

Retrieved from
"[http://omeka.org/codex/Functions/loop\_files\_for\_item](loop_files_for_item.html)"

</div>

<div id="catlinks" class="catlinks catlinks-allhidden">

</div>

</div>

<div id="secondary">

<div class="portlet">

Documentation
-------------

-   [Home](http://omeka.org/codex/)
-   [Screencasts](http://omeka.org/codex/Screencasts)
-   [Themes](http://omeka.org/codex/Managing_Themes_2.0)
-   [Appearance](http://omeka.org/codex/Managing_Appearance_2.0)
-   [Plugins](http://omeka.org/codex/Plugins2.0)

</div>

<div class="portlet">

Page View
---------

-   <div id="nav-page">

    </div>

    [Page](loop_files_for_item.html)
-   <div id="nav-discussion">

    </div>

    [Discussion](http://omeka.org/c/index.php?title=Talk:Functions/loop_files_for_item&action=edit&redlink=1)
-   <div id="nav-view_source">

    </div>

    [View
    source](http://omeka.org/c/index.php?title=Functions/loop_files_for_item&action=edit)
-   <div id="nav-history">

    </div>

    [History](http://omeka.org/c/index.php?title=Functions/loop_files_for_item&action=history)

</div>

<div id="wiki-toolbox" class="portlet">

Toolbox
-------

-   <div id="t-whatlinkshere">

    </div>

    [What links
    here](../Special:WhatLinksHere/Functions/loop_files_for_item.html)
-   <div id="t-recentchangeslinked">

    </div>

    [Related
    changes](../Special:RecentChangesLinked/Functions/loop_files_for_item.html)
-   <div id="t-specialpages">

    </div>

    [Special pages](http://omeka.org/codex/Special:SpecialPages)

</div>

[![Creative Commons
License](https://i.creativecommons.org/l/by/3.0/us/88x31.png)](http://creativecommons.org/licenses/by/3.0/us/)\
Omeka Documentation is licensed under a [Creative Commons Attribution
3.0 United States
License](http://creativecommons.org/licenses/by/3.0/us/).

</div>

</div>

</div>

<div id="footer">

<div class="padding">

<div id="sitemap">

<div class="section">

### About

-   [Project](../../index.html%3Fp=2.html)
-   [Staff](../../index.html%3Fp=3.html)
-   [News](../../blog.1.html)
-   [License](http://www.gnu.org/copyleft/gpl.html)

</div>

<div class="section">

### Help

-   [User Forums](../../forums/topic/mysqli-stmt.bind-result.html)
-   [Documentation](http://omeka.org/codex/)
-   [Dev Listserv](http://groups.google.com/group/omeka-dev)
-   [Contact](http://omeka.org/contact/)

</div>

<div class="section">

### Downloads

-   [Download Omeka](../../download.1.html)
-   [Plugins](../../plugins.html)
-   [Themes](../../download/themes/index.html)
-   [Packages](../../index.html%3Fp=222.html)

</div>

</div>

<div id="chnm-meta">

<span id="chnm-logo">[![Roy Rosenzweig Center for History and New
Media](http://omeka.org/ui/i/rrchnm-logo-regular.gif)](http://chnm.gmu.edu)</span>
Omeka is a project of the [Roy Rosenzweig Center for History and New
Media](http://chnm.gmu.edu), [George Mason
University](http://www.gmu.edu). Copyright © 2007–2016 CHNM.

</div>

</div>

</div>

</div>