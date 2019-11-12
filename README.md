# cleanremotes

cleanremotes accepts a command line filter now.  e.g. `./cleanremotes tv` will
only clean remotes that have `tv` in them

In order to permanently delete items from Trash you need to have Manager permissions on the 
Team Drive.  Content Manager and below cannot permanently delete Trash.

This script first runs rclone listremotes. Then for every remote that is configured in rclone 
the script runs the following commands:

rclone dedupe (eliminates exact duplicates)

rclone rmdirs (deletes empty directories)

rclone delete source --drive-trashed-only --drive-use-trash=false -v (permanently deletes all trash from the source - be very careful with this)


Be sure you know what each of these commands do before you run them. See rclone.org and read through the commands or forum for more information

Add a hash # at the beginning of any line you wish to omit
