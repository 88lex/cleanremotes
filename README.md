# cleanremotes

Runs rclone listremotes and for each remote runs rclone dedupe (eliminate exact dupes) and rclone rmdirs (delete empty directories).

Add a hash # at the beginning of the rclone dedupe or rmdirs line if you only want to run one, not both.
