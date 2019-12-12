# TigerGraph Icon Loader
Tools to transform and load many icons into TigerGraph for use in GraphStudio

# Overview
TigerGraph's GraphStudio has a method to add a single icon at a time using the web interface.
However, if you have a large collection of icons from a specific industry such as healthcare
this method is very time consuming and difficult to reproduce consistently on multiple environments.

# Method
If you have a folder of icons in 512x512 png format you can copy hem into the following folder:

```
$TIGERGRAPH_USER_HOME/tigergraph/visualization/server/src/public/prod/assets/img/user-uploaded-icons
```

# Data Conversion Scripts
If you don't have the icons in this format there is a set of python libraies in the pillow package that you
can use to change the icons into the right format.

# Copy Instructions From UNIX Shell
To do a copy of a folder called $MY_ICON_FOLDER, you can use the following command

```
$ cp $MY_ICON_FOLDER/*.png $TIGERGRAPH_USER_HOME/tigergraph/visualization/server/src/public/prod/assets/img/user-uploaded-icons
```

# Instructions to Convert Icons
In the src directory you will find a python file called convert-icons.py.

You will also need to make sure the pillow

```$ pip install pillow```

Here is the UNIX Shell command

src/convert-icons.py $SRC_FOLDER $DEST_FOLDER
