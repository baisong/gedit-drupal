This project contains code-completion snippets, mimetypes & icons for Gedit Drupal developers

# INSTALLATION

  a)  Create a new folder and clone repository on your machine:

        # git clone git://github.com/mavimo/gedit-drupal.git gedit-drupal
        # cd gedit-drupal

  b)  Copy language definition into /usr/share/gtksourceview-2.0/language-specs/

        # sudo cp lang/drupal.lang /usr/share/gtksourceview-2.0/language-specs/

  c)  Create a new mimetype into your machine

        # sudo cp mimetype/drupal.xml          /usr/share/mime/packages/

  d)  Update mimetype database

        # sudo update-mime-database /usr/share/mime

  e)  Add icons into your icons folder 
      Here are some common icon sets (yours may not be in the list below):
      
    sudo cp icons/* /usr/share/icons/Amaranth/scalable/mimetypes/
    sudo cp icons/* /usr/share/icons/gnome/scalable/mimetypes/
    sudo cp icons/* /usr/share/icons/Gorilla/scalable/mimetypes/
    sudo cp icons/* /usr/share/icons/Lush/scalable/mimetypes/
    sudo cp icons/* /usr/share/icons/Nuvola/scalable/mimetypes/
    sudo cp icons/* /usr/share/icons/oxygen/scalable/mimetypes/
    sudo cp icons/* /usr/share/icons/SphereCrystal/scalable/mimetypes/
    sudo cp icons/* /usr/share/icons/Wasp/scalable/mimetypes/
    sudo cp icons/* /usr/share/icons/whiteglass/scalable/mimetypes/

      after that regenerate iconset cache:
      
    cd /usr/share/icons
    sudo gtk-update-icon-cache ICONSET_NAME

  f)  Enable snippet plugin from inside Gedit

        Edit -> Preferences -> Plugins

      If not already aviable please install it from your distrubution system, for 
      debian / ubuntu system you can use repostitory at deb.mavimo.org:

        # sudo sh -c "echo 'deb http://deb.mavimo.org/ binary/' >> /etc/apt/sources.list"
        # sudo apt-get update
        # sudo apt-get install gedit-plugins

  g)  Add variuos snippets

        Tools -> Manage Snippets ...

      Press "Import snippets" button (second from left on bottom) and import *.xml file
      do you require. After that you can use drupal-snippet

# USAGE

Using Snippet is very simple, when you write a drupal module or install file 
please select, from View -> Highlight Mode -> Scripts -Drupal, and now you can
write your code with snippet accelerator, a complete list of snippet is aviable
on file SNIPPET_LIST
If you create new mimetype to you machine is not required set Highlight Mode, sistem
automatically detect it.
