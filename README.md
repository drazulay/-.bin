# DOT-BIN

Some handy scripts for in the `~/.bin` folder

## `backup-keychains`

Backs up keychain files stored in `~/.keychains` to a mounted volume.

### Arguments
`backup-keychains` takes two optional arguments. The first argument is the name of a mounted volume to back up to, the default is `KEYCHAINS`. The second argument is the path where volumes are mounted at in your system. The default is `/Volumes`.

### To-Do
- Use an argument parser instead of unstable positional arguments.

## `backup-config`

Backs up files and directories in your home directory to a mounted volume.

### Arguments
`backup-config` takes two optional arguments. The first argument is the name of a mounted volume to back up to, the default is `CONFIG`. The second argument is the path where volumes are mounted at in your system. The default is `/Volumes`.

### Configuration
The file `backup-config.conf` is a file where you simply list all the files and directories (as absolute paths) in your home directory that are important to you. They will all be backed up when the command is run.

### To-Do
- Use an argument parser instead of unstable positional arguments;
- Compress backups as tar.gz files.
