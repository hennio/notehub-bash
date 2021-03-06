NAME

    notehub - note taking framework using VIM

SYNOPSIS

    notehub [OPTION (create/search)] [LOCATION (local/cloud)] [TYPE (note/journal)]

INSTALLATION

    Note: for export functions install pandoc

    1. Move notehub script to a $PATH-location
    2. Create folders;
        ~/notehub/cloud/notes (symlink this to synced folders eg dropbox/owncloud etc)[1]
        ~/notehub/cloud/journal (symlink this to synced folders eg dropbox/owncloud etc)
        ~/notehub/local/notes (for notes not to be trusted online and kept locally)
        ~/notehub/local/journal (for journals not to be trusted online and kept locally)
        ~/notehub/templates/ (for your templates. They are copied to the apropriate folder 
        while creating a note/journal)
    3. Restart your shell

    [1] ln -s ~/Nextcloud/notehub/cloud/journals ~/notehub/cloud/journals

DESCRIPTION

    A personal note-helper for personal use. You can choose for local and cloud-storage by symlinking the folders in the 
    ~/notehub/cloud folder for backup-purposes. If you have notes rather stored locally its possible, they are stored 
    in ~/notehub/local.


EXAMPLES

    - notehub create cloud journal
        Creates a cloud journal file in the ~/notehub/cloud/journals
    - notehub create cloud note
        Creates a cloud note file in the ~/notehub/cloud/notes
    - notehub create local journal
        Creates a local journal file in the ~/notehub/local/journals
    - notehub create local note
        Creates a local note file in the ~/notehub/local/notes

    - for export use: pandoc file.md -o ~/Desktop/file.pdf
    - for search use: "grep -i -H -R string *" in folder

    - for adding images to your note, place image in "img" folder and add in text; 
      ![titel of image](img/file.jpg)

TODO

    - search and export-functions 

SEE ALSO

    vim 

BUGS

    No known bugs

AUTHOR

   Henrique van Huisstede <henrique@van.huisste.de>

COPYRIGHT

    Please use and improve.