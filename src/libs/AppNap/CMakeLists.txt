#
# Copyright (C) 2020 Adrian Carpenter
#
# This file is part of Pingnoo (https://github.com/fizzyade/pingnoo)
#
# An open-source cross-platform traceroute analyser.
#
# Created by Adrian Carpenter on 27/03/2020.
#
# This program is free software: you can redistribute it and/or modify
# it under the terms of the GNU General Public License as published by
# the Free Software Foundation, either version 3 of the License, or
# (at your option) any later version.
#
# This program is distributed in the hope that it will be useful,
# but WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
# GNU General Public License for more details.
#
# You should have received a copy of the GNU General Public License
# along with this program.  If not, see <http://www.gnu.org/licenses/>.
#

pingnoo_start_shared_library()

pingnoo_add_sources(
    AppNap.cpp
    AppNap.h
    AppNap_mac.mm
)

pingnoo_set_description("Application Nap extension")

pingnoo_use_qt_libraries(Core)

pingnoo_use_frameworks("Foundation" "Cocoa")
pingnoo_use_system_libraries(APPLE stdc++ objc)

pingnoo_end_shared_library()
