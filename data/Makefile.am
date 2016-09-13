# This file is part of Unity8-session, a desktop session configration
# package.
#
# Copyright 2013-2016 Canonical Ltd.
# 
# unity8-desktop-session is free software: you can redistribute it and/or modify
# it under the terms of the GNU General Public License version 3, as published by
# the Free Software Foundation.
# 
# This program is distributed in the hope that it will be useful, but WITHOUT ANY
# WARRANTY; without even the implied warranties of MERCHANTABILITY, SATISFACTORY
# QUALITY, or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public
# License for more details.
# 
# You should have received a copy of the GNU General Public License along with
# this program.  If not, see <http://www.gnu.org/licenses/>.

icondir = ${datadir}/unity-greeter
lightdmdir = ${datadir}/lightdm
lightdm_confdir = ${lightdmdir}/lightdm.conf.d
lightdm_sessiondir = ${lightdmdir}/sessions

dist_pkgdata_DATA = \
	sensors.txt

dist_icon_DATA = \
	custom_unity8_badge.png \
	custom_unity8-snap_badge.png

dist_lightdm_conf_DATA = \
	45-unity8.conf

dist_lightdm_session_DATA = \
	unity8.desktop \
	unity8-snap.desktop

dist_bin_SCRIPTS = \
	lightdm-unity8-session

EXTRA_DIST = \
	unity8.desktop.in

