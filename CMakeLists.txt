cmake_minimum_required(VERSION 2.4)

project(acc)

# if (MSVC)
# 	add_definitions("-D_CRT_SECURE_NO_DEPRECATE -D_CRT_NONSTDC_NO_DEPRECATE")
# elseif("${CMAKE_CXX_COMPILER_ID}" MATCHES "GNU" OR "${CMAKE_CXX_COMPILER_ID}" MATCHES "Clang")
# 	set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11 -Wno-unused-variable")
# endif (MSVC)

set(SOURCE_FILES
	acc.c
	error.c
	misc.c
	parse.c
	pcode.c
	strlist.c
	symbol.c
	token.c
	common.h
	error.h
	misc.h
	parse.h
	pcode.h
	strlist.h
	symbol.h
	token.h
)

add_executable(acc ${SOURCE_FILES})
