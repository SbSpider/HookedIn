This is the base directory where this project will take of from. Please refer
to the google drive file for more information on what I want to have done in
this project. The purpose of this is that an application / service / extension
be developed that allows the monitoring of folders and files, essentially
making "hooks" that allow the user to do almost anything with said files -
raise email alerts on changes to the file, locking of files and folders,
automatic backups, scheduled events. It may not be anything new, but it will
combine a lot of other features that are currently scattered into a more
concise and nice to use piece of software. There should be a gui element for
those not comfortable with using a shell - this could be done through perhaps
a property page under properties, or a centralised application that allows you
to configure said directory listings and such. Initially, will only support
windows, but could consider other computer types when I try them out more and
see what sort of possibilities are available. There will also be a terminal
base (perhaps a more important part of it, as more possibility there) that
will allow configuration and setup for the application (a central database may
be required for this - this could be extended further to use online databases
to allow backed up config files). What could also be done is "hidden folders"
being introduced for files and folders, like .git and .bzr, that could store
data for local componenets and the like, especially for folder monitoring.


THis directory will act as the base, with other files extending this further.

TO see if there are changes to the file/folder, we can use MD5 checksums. 
Calculating the MD5 checksum for a file/folder is very quick (more so than for
example a diff). We can run a checksum ever so often (whatever time is required)
and if there has been a change to the file/folder, then there will be a change
to the checksum as well, so we can easily and quickly see if there has been a
change, and if there has, go for more in depth info-finding - for example, a diff.


As part of this, we can also think of integrating git. Git would serve well to allow
us to see if there has been a change to the file/folder, as it would be simple to work
with (or we could roll our own source control system specifically for this).

We can also think of including git as a module of the program - where a user can "snapshot"
the file/folder as it is now, allowing for changes to be reverted later. However, we could
roll our own source control system as well if we want to. Could be a nice to have feature.
