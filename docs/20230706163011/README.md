# Inline Inode Data

Files that are smaller than a certain size in UNIX-like systems are stored directly within inode (short for `index node`, files index of the OS) rather than in data blocks or a different directory. This concept is known as `inline data` or `inline inode data`. The reason is, avoiding the need for additional disk access to retrieve the related file, which accelerates read/write operations and also, it helps with disk health.
