# redmine wiki index tree view

This is a plugin for Redmine which convert wiki index page to tree view

## Open first hierarchy.

this is default.

![first_open](http://f.st-hatena.com/images/fotolife/b/basyura/20140428/20140428235403.png)

## Open second hierarchy.

![second_open](http://f.st-hatena.com/images/fotolife/b/basyura/20140428/20140428235402.png)

You must modify souce to open second hierarchy.

- redmine_wiki_index_tree_view/assets/javascripts/redmine_wiki_index_tree_view.js

```diff
   $(document).ready(function(){
     $(".pages-hierarchy:first").treeview({
       collapsed: true,
     });
     $(".hitarea:first").click();
     // open second hierarchy
-    //$('.treeview:first').find('ul:first').children('li').find('.hitarea:first').click();
+    $('.treeview:first').find('ul:first').children('li').find('.hitarea:first').click();
   });
```

## LICENSE

MIT License

This plugin contain Jörn Zaefferer's jquery-treeview.

- http://bassistance.de/jquery-plugins/jquery-plugin-treeview/
- https://github.com/jzaefferer/jquery-treeview


