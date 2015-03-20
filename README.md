How to use
==========

Download binary package and install (or alternatively: build from sources and install):

    wget 'https://github.com/sigsergv/shell-utils/raw/binary-release/more-shell-utils_1.1-1_all.deb'
    sudo dpkg -i more-shell-utils_1.1-1_all.deb

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
