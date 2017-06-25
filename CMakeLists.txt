cmake_minimum_required(VERSION 3.7)
project(lab)

set(CMAKE_CXX_STANDARD 11)

set(SOURCE_FILES
        boot/main.c
        fs/test.c
        inc/assert.h
        inc/elf.h
        inc/error.h
        inc/kbdreg.h
        inc/memlayout.h
        inc/mmu.h
        inc/stab.h
        inc/stdarg.h
        inc/stdio.h
        inc/string.h
        inc/types.h
        inc/x86.h
        kern/console.c
        kern/console.h
        kern/entrypgdir.c
        kern/init.c
        kern/kclock.c
        kern/kclock.h
        kern/kdebug.c
        kern/kdebug.h
        kern/monitor.c
        kern/monitor.h
        kern/pmap.c
        kern/pmap.h
        kern/printf.c
        lib/printfmt.c
        lib/readline.c
        lib/string.c
        user/sendpage.c)

add_executable(lab ${SOURCE_FILES})

include_directories(.)