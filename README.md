Unity3D-EmptyProject
====================

Template empty project for Unity3D.

Not a very complicated project, but it's faster for me than walking someone through it every time they ask.

Unity supports external version control, but its default settings aren't entirely friendly for it. This template project contains just enough files to change some of those default settings.

* Meta files: Unity will generate a `.meta` file for each asset it imports, so that you can copy the project between computers without losing Library data.
* Force text serialization: Unity will now serialize scenes and prefabs in a text format, for easier diff+merge.

I also include a `.gitignore` file that will skip over some of Unity's generated files.
