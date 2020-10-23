Private files download permission
=================================

Provides a simple permission to allow downloading of private files per-directory
by-user and by-role filter.

Installation
------------

- Install this module using the official Backdrop CMS instructions at
  <https://backdropcms.org/guide/modules>

Configuration
-------------

Browse to Configuration > Media > Private files download permission (url:
/admin/config/media/private-files-download-permission). Then add or edit each
directory path you want to put under control, associating users and roles which
are allowed to download from that location.
All directory paths are relative to your private file system path, but must
have a leading slash ('/'), as the private file system root itself could be put
under control.

E.g.:
Suppose your private file system path is /opt/private.
You could configure /opt/private (and all of its subdirectories) by adding a
'/' entry, while a '/test' entry would specifically refer to /opt/private/test
(and all of its subdirectories).

Please note that per-user checks may slow your site if there are plenty of
users. You can then bypass this feature by browsing to Configuration > Media >
Private files download permission > Preferences (url:
/admin/config/media/private-files-download-permission/preferences) and change
the setting accordingly.
Additional settings are available to cache users and/or log activities.

Also configure which users and roles have access to the module configuration
under People > Permissions (url: /admin/people/permissions).

Issues
------

Bugs and Feature requests should be reported in the Issue Queue:
<https://github.com/backdrop-contrib/webform_layout/issues>

Current Maintainers
-------------------

- Herb v/d Dool <https://github.com/herbdool>

Credits
-------

- Ported to Backdrop by Herb v/d Dool <https://github.com/herbdool>
- Originally developed for Drupal by zanonmark <https://www.drupal.org/u/zanonmark>.

Idea and code were inspired by <http://www.beacon9.ca/labs/drupal-7-private-files-module>.
Partly sponsored by Cooperativa Italiana Artisti <http://www.cita.coop>.

License
-------

This project is GPL v2 software. See the LICENSE.txt file in this directory for
complete text.
Credit
------
