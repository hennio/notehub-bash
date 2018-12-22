NAME

    notehub - note taking framework using VIM

SYNOPSIS

    notehub [OPTION] [-t <templatefile>]

DESCRIPTION

    A personal note-helper for personal use. You can choose for local and cloud-storage by symlinking the folders in the ~/notehub/cloud folder for backup-purposes. If you have notes rather stored locally its possible, they are stored in ~/notehub/local.

    The folowing options are available;

    -ccj <title>
    	Creates a cloud journal file in the ~/notehub/cloud/journals
    -ccn <title>
    	Creates a cloud note file in the ~/notehub/cloud/notes
    -clj <title>
    	Creates a local journal file in the ~/notehub/local/journals
    -cln <title>
    	Creates a local note file in the ~/notehub/local/notes

    -sn <keyword ...>
    	Search all notes for keywords
    -sj <keyword ...>
    	Search all journals for keywords

    -t <templatefile>
    	Only possible when creating a note or journal. This selects a templatefile from the ~/notehub/templates/ directory. It copies is to the apropriate folder and renames it and is opened in VIM.


EXAMPLES
    notehub -cln "foo bar" -t meeting

    This wil search for a note with title "foo bar", if it is not found it creates one from templatefile 'meeting'.

SEE ALSO
    vim 

BUGS
    No known bugs

AUTHOR
   Henrique van Huisstede <henrique@van.huisste.de>

COPYRIGHT
    Please use and improve.