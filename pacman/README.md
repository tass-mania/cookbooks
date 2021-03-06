DESCRIPTION
===========

Refreshes the pacman package cache from the FTP servers and provides an LWRP for managing package groups.

REQUIREMENTS
============

Platform: ArchLinux. Pacman is not relevant on other platforms.

USAGE
=====

Include `recipe[pacman]` early in the run list, preferably first, to ensure that the package caches are updated before trying to install new packages.

Use the `pacman_group` resource to install or remove pacman package groups. Note that at this time the LWRP will check if the group is installed but doesn't do a lot of error checking or handling. File a ticket on the COOK project at tickets.opscode.com for improvements and feature requests.

LICENSE AND AUTHOR
==================

Author:: Joshua Timberman (<joshua@opscode.com>)

Copyright:: Opscode, Inc. (<legal@opscode.com>)

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
