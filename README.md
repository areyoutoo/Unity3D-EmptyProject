Unity3D-EmptyProject
====================

Template empty project for Unity3D.

Not a very complicated project, but it's faster for me than walking someone through it every time they ask.

Unity supports external version control, but its default settings aren't entirely friendly for it. This template project contains just enough files to change some of those default settings.

* Meta files: Unity will generate a `.meta` file for each asset it imports, so that you can copy the project between computers without losing Library data.
* Force text serialization: Unity will now serialize scenes and prefabs in a text format, for easier diff+merge.

I also include a `.gitignore` file that will skip over some of Unity's generated files.

How to use this
---------------

As simply as possible:

1. Download the empty project with any of GitHub's "Download ZIP" buttons.
2. Extract the ZIP somewhere on your machine.
3. Rename the project folder.
4. Run Unity. Go to `File > Open Project... > Open Other...`, browse to the empty project folder.
5. Voila! You have a new Unity project.

Use with SVN
------------

This template project should be fully compatible with Subversion, with the exception that SVN cannot source its ignore list from a file. You can instead set the `svn:ignore` property:

    cd path/to/your/project
    svn propset svn:ignore -F .svnignore .

The `.svnignore` file is a close twin of `.gitignore`.

You should have to do this exactly once, when you first set up the project.

As far as keeping those files:

* If you're using Git, you can delete `.svnignore`.
* If you're using SVN, you can delete both `.gitignore` and `.svnignore` once you're done with them.

Advanced SVN users might consider applying the property recursively (by passing `-R` to `propset` or with `svn:global-ignores`); if you go that route, consider ignoring `Library` and `Temp` only at the project root.
    
    

