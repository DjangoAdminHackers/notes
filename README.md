Notes and Resources
===================

* https://github.com/exogen/django-adminbrowse
* http://garlicjs.org/ [autosaving]
* http://mcpants.github.com/jquery.shapeshift/ [drag and drop for gallery ordering]
* http://djangosnippets.org/snippets/431/ [Automatic edit popup for related objects]
* https://github.com/charettes/django-admin-enhancer
* https://github.com/burke-software/django-report-builder
* http://stackoverflow.com/a/10267927/45955 [possible fix for admin template inheritance problems]
* http://source.mihelac.org/2012/12/20/django-import-export/ [nice import/export]
* http://djangosnippets.org/snippets/2868/ [Another admin CSV export]  
* https://github.com/liberation/django-admin-tabs/ [out of date and badly architectured]
* https://github.com/KrzysiekJ/django-typed-models and https://github.com/craigds/django-typed-models
* https://github.com/jsocol/django-ratelimit
* http://packages.python.org/django-authority/index.html
* https://github.com/benjaoming/django-relatedadminwidget
* https://github.com/pullswitch/django-freeplay
* https://readthedocs.org/projects/django-fluent-dashboard/
* http://django-admin-tools.readthedocs.org/en/latest/

Faking the ORM
==============

* https://github.com/liberation/django-sneak
* http://code.larlet.fr/django-roa/wiki/Home
* https://github.com/liberation/django-admincommand


Random Thoughts
===============

ADMIN TABS FOR COMPLEX FORMS
(each tab takes you to a separate changelist). Each tab is a changelist for the same model but shows different inlines (use different ModelAdmin's or via proxy models?)

Checkout Mezzanine and Cartridge

Admin Next
==========

* https://code.djangoproject.com/wiki/AdminNext
* https://groups.google.com/forum/?fromgroups=#!topic/django-developers/Vozu6U3gz84
* https://speakerdeck.com/amiramazig/django-composite
* https://github.com/django-composite/django-composite-admin/
* https://github.com/django-composite/django-composite
* https://github.com/zbyte64/django-hyperadmin
* https://github.com/django-djam/django-djam
* https://github.com/disqus/nexus

* http://sshwsfc.github.io/django-xadmin/



Future Admin improvements
=========================

Google maps picker:
http://www.randomsequence.com/articles/django-admin-google-maps-location-picker-with-jquery/

Switch to a different tag libraru and sort out the filters. Maybe use: http://djangosnippets.org/snippets/2807/

Some useful genric actions: https://github.com/saxix/django-actions

Use ButtonAdmin:
http://djangosnippets.org/snippets/1016/ or
http://djangosnippets.org/snippets/2673/
(can it be a mixin?)

Split Changeform into tabs
Tabs for related changeforms (i.e. split a long changeform into different proxy changeforms with different sets of fields and link them via a tabbed interfacr.
Either use proxy models or use https://github.com/ionelmc/django-admin-customizer

Tabs for fieldsets
Either all jQuery or use: https://github.com/liberation/django-admin-tabs

Filefields that don't lose input on validation errors
https://github.com/generalov/django-resubmit

Use plupload for client-side resizing

User controlled changeform column and filter customization
https://github.com/ionelmc/django-admin-customizer

Better TinyMCE button set

Use the Molior long filter fix on all projects

Complete MCE/Filebrowser integration and replace the insert/edit image dialog with filebrowser

Improve the add/insert link dialog

Allow choosing existing uploaded files/images when using FileField or ImageField

Factor admin customizations out into multiple apps

Implement django-locking 

Ajaxey list_editable that doesn't overwrite all fields

Mini changeforms within changelist. 'Click to expand' IFrames?

Configurable dashboard replaces index page. Pluggable

Fix breadcrumbs in current app/model renaming system. Allow model as well as renaming in admin

revisit the admin submit line customization in Molior

automatically switch filter selects to more compact layout when over a certain length

http://pypi.python.org/pypi/django-admin-flexselect/0.4.1
https://github.com/charettes/django-admin-enhancer
https://github.com/benjaoming/django-relatedadminwidget
http://ionelmc.wordpress.com/2012/01/19/tweaks-for-making-django-admin-faster/
http://code.google.com/p/django-ajax-filtered-fields/
http://django-filer.readthedocs.org/en/latest/index.html
http://djangosnippets.org/snippets/2194/

[should internal urls be stored in a format that does a lazy lookup] i.e. href="model://xxx,id###". Replace it when the page is rendered. That way there is no need for a slug and all internal links update automatically. Still a chance of breaking external links though. Maybe use a 301 for those?]


Current Tweaks
==============

Hierarchical page editor

Check for unsaved pages when navigating away from changeform

Show/hide filters on changelist

drag/drop reorder inlines

drag/drop reorder changelist

MCEField

File browser button in MCE

Convert action SELECT control into buttons

You can rename App label in ModelAdmin

Thumbnails for ImageFields

CSV Export action (also see https://github.com/saxix/django-actions above )

django-reversion

Display uploaded docs in MCE insert/edit link dialog

Display all page-like objects in MCE insert/edit link dialog

Pluggable admin error blocks

Pluggable admin index page blocks

Pluggable dynamic fields in changeform based on selection of another field (pagetypes)






Old List from Google Docs
===================

Remove File Browser upload button after browsing images 
Mailto: instructions / way of creating this link?	.
Swap 'choose' and 'manual' in MCE link dialog	
Admin dates should use UK date format	Reuse code from Lily or update Django to 1.2
Remove word 'change' from news photo admin	
"extra content" help text sucks	Make specific to page type "This content is displayed after the list of events."
Hide 'extra content' on pages that don't use it	fixed but buggy
Would like to be able to change titles of treatment and catogories on summary page without entering into page	Maybe have on/off switch for list editable.
slide show app (active/ non active pages in summary)	Make slide show into an app.
change image preview if image has been changed before saving, so you can see the update. This was on the lily shop catogory and product pages	
Cache settings error, never viewed by users – sent as email to Andy	
Add page button clearer	
Go straight to summary pages	
Change the action button to just have delete selected event	
Swap add page buttons to be more prominent and before recover button	
Take name coloumn out of summary page	
Help text on summary – with regards to changing order	
Active and in nav to be changeable on summary – add in delete page tick box	needs rewrite of treeview
Save order button – change to "save changes"?	
When editing a page – page name will be hidden until menu title is changed, then will highlight in red.	
url name – small grey title – click here to edit url name	
Nice icons and image up load from grappelli	
Help text on hover for tiny mce	
Tinymce has scrollbars and limit to auto-resize	
Move page type to top and add page specific help text – read only	
Colour page types row	
Ixxy colouring and branding	
Check inlines on lily	
General content to be the first tab	
Help text for models on index page	
Tools and settings for link manager, file browser and site settings	
Fix expires headers for media	"http://code.google.com/p/django-compress/wiki/FarFutureExpires
http://stackoverflow.com/questions/1411542/what-is-the-best-way-to-set-far-future-expires-on-images-with-django"
Remove word 'change' from photo admin	
Repopulate matching related-item ChoiceFields when using 'add another'	
Hide inline 'delete' column when no existing items	
Switch media to use subdomain	"http://wiki.moxiecode.com/index.php/TinyMCE:Cross_domain_loading
http://forum.webfaction.com/viewtopic.php?id=2826"
unsaved changes warning for changelists	

James H. Suggestions
=================

Remember filter settings when returning to changelist

 
