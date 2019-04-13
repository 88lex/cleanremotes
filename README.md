# cleanremotes

Runs rclone listremotes and for each remote runs 

rclone dedupe (eliminate exact dupes) 
rclone rmdirs (delete empty directories)
#rclone delete source --drive-trashed-only --drive-use-trash=false -v (permanently deletes all trash - be very careful with this)

Add a hash # at the beginning of any line you wish to omit
