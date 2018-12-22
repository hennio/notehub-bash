NAME

    notehub - note taking framework using VIM

SYNOPSIS

    notehub [OPTION (create/search)] [LOCATION (local/cloud)] [TYPE (note/journal)]

INSTALLATION

    1. Move notehub script to a $PATH-location
    2. Create folders;
        ~/notehub/cloud/notes (symlink this to synced folders eg dropbox/owncloud etc)
        ~/notehub/cloud/journal (symlink this to synced folders eg dropbox/owncloud etc)
        ~/notehub/local/notes (for notes not to be trusted online and kept locally)
        ~/notehub/local/journal (for journals not to be trusted online and kept locally)
        ~/notehub/templates/ (for your templates. They are copied to the apropriate folder while creating a note/journal)
    3. Restart your shell

DESCRIPTION

    A personal note-helper for personal use. You can choose for local and cloud-storage by symlinking the folders in the ~/notehub/cloud folder for backup-purposes. If you have notes rather stored locally its possible, they are stored in ~/notehub/local.

    The folowing options are available;

    -notehub create cloud journal
    	Creates a cloud journal file in the ~/notehub/cloud/journals
    -notehub create cloud note
    	Creates a cloud note file in the ~/notehub/cloud/notes
    -notehub create local journal
    	Creates a local journal file in the ~/notehub/local/journals
    -notehub create local note
    	Creates a local note file in the ~/notehub/local/notes


EXAMPLES
    notehub -cln "foo bar" -t meeting

    This wil search for a note with title "foo bar", if it is not found it creates one from templatefile 'meeting'.

TODO
    * search-methods not created
    * export-method (pandoc) not created


SEE ALSO
    vim 

BUGS
    No known bugs

AUTHOR
   Henrique van Huisstede <henrique@van.huisste.de>

COPYRIGHT
    Please use and improve.