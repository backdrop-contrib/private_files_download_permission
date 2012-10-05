Private files download permission
=================================

DESCRIPTION
----------------------------

Version 1.x provided "two useful features which Drupal itself is missing: a
simple permission to allow downloading of private files by role, plus the
ability to combine both public and private downloads".

Version 2.x removes the "global" permission and implements a by-directory and
by-role grid instead, to make the administrator better tweak the whole website
and increment the overall security.

Idea and code (mostly for version 1.x) were inspired by
http://www.beacon9.ca/labs/drupal-7-private-files-module.

INSTALLATION / CONFIGURATION
----------------------------

Browse to Configuration > Media > Private files download permission (url:
/admin/config/media/private-files-download-permission). Then add or edit each
directory path you want to put under control, associating roles which are
allowed to download from it.
All directory paths are relative to your private filesystem path, but must have
a leading slash ('/'), since the private filesystem root itself could be put
under control.

Example.
Suppose your private file system path is /opt/private.
You could protect /opt/private itself by configuring a '/' directory entry,
while a '/test' item would refer to /opt/private/test.

Also configure which roles have access to the module configuration under
People > Permissions (url: /admin/people/permissions).
