# Copyright (C) 2007-2014 LuaDist.
# Created by Cyril Romain
# Redistribution and use of this file is allowed according to the terms of the MIT license.
# For details see the COPYRIGHT file distributed with LuaDist.
# Please note that the package source code is licensed under its own license.

project ( lunatest NONE )
cmake_minimum_required ( VERSION 2.8 )
include ( cmake/dist.cmake )
include ( lua )

install_lua_module ( lunatest lunatest.lua )

install_data ( README.md )

install_doc ( index.html luadoc.css )

install_test ( test.lua test-error_handler.lua test-teardown_fail.lua )
install_test ( suite-hooks-fail.lua suite-hooks.lua suite-with-random-tests.lua )
