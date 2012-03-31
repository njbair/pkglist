pkglist - Pacman Package List Generator
=======================================
Copyright &copy; 2012 Nick Bair


License
-------
This program is free software; you can redistribute it and/or modify it
under the terms of the GNU General Public License as published by the
Free Software Foundation; either version 2 of the License, or (at your
option) any later version.

This program is distributed in the hope that it will be useful, but
WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
General Public License for more details.

You should have received a copy of the GNU General Public License along
with this program; if not, write to the Free Software Foundation, Inc.,
51 Franklin Street, Fifth Floor, Boston, MA 02110-1301, USA.


About
-----
**pkglist** is a Bash script for Pacman users to generate a list of
non-locally installed packages

pkglist takes advantage of Pacman's built-in querying functions to
generate a list of installed packages. The script outputs a plain-text
file, one package name per line. The output file is named
*{HOSTNAME}.pkglist*. The file may be backed up to a USB key, a cloud
storage service such as Dropbox, or a pastebin service such as GitHub
Gist.

This output is suitable for system backups and can be used to restore
packages on a newly-installed system using the command:

	pacman -S $(< hostname.pkglist)

More information on using Pacman with package lists is available on the
[Arch
Wiki](https://wiki.archlinux.org/index.php/Pacman_Tips#Backing_up_and_retrieving_a_list_of_installed_packages
"pacman Tips - ArchWiki").
