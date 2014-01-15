# This file is part of Unity8-session-x11, a desktop session configration
# package.
#
# Copyright 2013 Canonical Ltd.
# 
# Unity8-session-x11 is free software: you can redistribute it and/or modify it
# under the terms of the GNU General Public License version 3, as published by
# the Free Software Foundation.
# 
# This program is distributed in the hope that it will be useful, but WITHOUT ANY
# WARRANTY; without even the implied warranties of MERCHANTABILITY, SATISFACTORY
# QUALITY, or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public
# License for more details.
# 
# You should have received a copy of the GNU General Public License along with
# this program.  If not, see <http://www.gnu.org/licenses/>.

icondir = ${datarootdir}/unity-greeter
upstartdir = ${datarootdir}/upstart/sessions
xsessiondir = ${datarootdir}/xsessions
lightdmdir = ${sysconfdir}/lightdm/lightdm.conf.d
sbindir = ${prefix}/sbin

dist_pkgdata_SCRIPTS = \
	start-unity8-mir

dist_xsession_DATA = \
	unity8-mir.desktop \
	unity8-x11.desktop

dist_icon_DATA = \
	custom_unity8-mir_badge.png \
	custom_unity8-x11_badge.png

dist_upstart_DATA = \
	unity8-mir.conf

dist_lightdm_DATA = \
	55-unity8.conf

dist_sbin_SCRIPTS = \
	lightdm-unity8-session

EXTRA_DIST = \
	unity8-mir.conf.in \
	unity8-mir.desktop.in \
	custom_unity8-mir_badge.xcf \
	custom_unity8-x11_badge.xcf

CLEANFILES = \
	unity8-mir.desktop \
	unity8-mir.conf

unity8-mir.conf: unity8-mir.conf.in Makefile
	$(AM_V_GEN)sed -e 's,[@]LIB_DIR[@],$(libdir),g' \
	    <$(srcdir)/unity8-mir.conf.in >unity8-mir.conf

unity8-mir.desktop: unity8-mir.desktop.in Makefile
	$(AM_V_GEN)sed -e 's,[@]EXEC_DIR[@],$(pkgdatadir),g' \
	    <$(srcdir)/unity8-mir.desktop.in >unity8-mir.desktop
