#
# Copyright (c) 2019 Nordic Semiconductor
#
# SPDX-License-Identifier: LicenseRef-Nordic-5-Clause
#

zephyr_library()

#zephyr_library_sources(paw32xx.c)
zephyr_library_sources_ifdef(CONFIG_PAW32XX src/paw32xx.c)
zephyr_include_directories(${APPLICATION_SOURCE_DIR}/include)
