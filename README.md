How to use
==========

Download binary package and install (or alternatively: build from sources and install):

    wget 'https://github.com/sigsergv/shell-utils/releases/download/1.4/more-shell-utils_1.4-1_all.deb'
    sudo dpkg -i more-shell-utils_1.4-1_all.deb

What's inside
=============

Several useful scripts that really improve unix-shell experience.

ff
--

Find file/directory by part of file name, starting from current directory.

~~~~~
% ff .cpp
./eclibrus/src/preferencesdialog.cpp
./eclibrus/src/moc_exportbooksprogress.cpp
...
~~~~~

Also you can use flag `-i` to ignore case.


canonical-name
--------------

Print canonical file name (resolve all symlinks, eliminate `.` and `..`).

~~~~~
% canonical-name 000-default.conf 
/etc/apache2/sites-enabled/000-default.conf
~~~~~


fixperms
--------

Fix all permissions (recursively) to all files starting with the current directory, change all files permissions
to 0644 and all directories to 0755.

~~~~~
% fixeprms
%
~~~~~


uncolor
-------

Remove shell escape special characters from stdin and put to stdout

~~~~~~
% uncolor < log.txt > clear.txt
~~~~~~



