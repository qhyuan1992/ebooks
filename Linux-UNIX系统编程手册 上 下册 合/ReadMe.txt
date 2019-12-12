该书对应网站
http://www.man7.org/tlpi/

代码下载地址：
http://www.man7.org/tlpi/code/index.html
Source Code of the Programs in The Linux Programming Interface

The source code for the program examples in TLPI is provided in two versions:

【Distribution version:】[tlpi-171205-dist.tar.gz]
(http://www.man7.org/tlpi/code/download/tlpi-171205-dist.tar.gz)
 a tarball of the source code that includes extra material not shown in the book. Probably, this is the version of the code that you want.
翻译：源代码的一个tarball，其中包含了没有在书中显示的额外内容。可能，这是您想要的代码版本。

【Book version:】 [tlpi-171205-book.tar.gz]
(http://www.man7.org/tlpi/code/download/tlpi-171205-book.tar.gz)
a tarball of the source code as it appears in the book.
For an explanation of why there are two versions of the code, look here.
源代码的一个tarball，就像它在书中所显示的那样。

Please take a look at the README file and the BUILDING file for general information about the program source code and how to compile it.

If you encounter compilation problems, please read the source code FAQ.

For a summary of changes that have been made to the code since it was printed in the book, see the CHANGES file.

If you want to browse individual source files online, look here.


【ReadMe】
README for code in The Linux Programming Interface

Gidday!

This is the code for the book "The Linux Programming Interface"
and this is a note from me, the author, Michael Kerrisk.

For instructions on building the programs, see the file BUILDING.

For notes on changes that have been made to the code since it was
published in the book, see the file CHANGES.


Source code licensing
=====================

All complete programs provided in this distribution are covered by
the GNU General Public License (Version 3), a copy of which is
contained in the file COPYING.gpl-v3, which should have arrived with
this tarball.  The library functions (in the lib/ directory) are
covered by the GNU Lesser General Public License (Version 3); see the
files COPYING.lgpl-v3 and COPYING.gpl-v3 provided with this tarball.


A note on the source code
=========================

The source code is available in two versions: "dist" and "book".
The "book" version contains the program source files as published in
the book. The source files in the "dist" version contain extra code
beyond that published in the book. The differences between the "dist"
and "book" versions are as follows:

a) The "dist" versions of some programs contain extra comments.
   These additional comments were stripped out of the printed version
   to make the published versions of the programs shorter. (The book
   itself contains text describing the operation of the programs.)

b) In a few cases, some changes have been incorporated into the
   "dist" versions to make it possible to compile programs on UNIX
   implementations other than Linux, so that you can try them out
   on other implementations if you wish.  Where necessary, the
   additional code is conditionally compiled using the following
   platform-specific macros:

        __linux__       Defined on Linux
        __sun           Defined on Solaris
        __FreeBSD__     Defined on FreeBSD
        __NetBSD__      Defined on NetBSD
        __OpenBSD__     Defined on OpenBSD
        __APPLE__       Defined on Mac OS X
        __hpux          Defined on HP-UX
        __osf__         Defined on Tru64 UNIX (formerly DEC OSF1)
        __sgi           Defined on Irix
        _AIX            Defined on AIX

c) In the "dist" version, some programs have extra functionality beyond
   that in the "book" versions. Where this is significant, comments in
   the programs explain the differences.


Subdirectories
==============

Under the 'tlpi' directory are a number of subdirectories. Each
subdirectory corresponds to one or more chapters of the book.
The following paragraphs give brief notes on the contents of
each subdirectory.

Note that in some cases, files are (hard) linked to appear in more than
one directory. This is particularly the case for each of the files in
the 'lib' directory, most of which are also linked in the directory
of the chapter relating to that file.

Directory       Files for Chapter...

lib             This contains library routines used by other 
                programs. The tlpi_hdr.h and error_functions.* 
                files are located here.
                
progconc        3 (System Programming Concepts)

fileio          4 and 5 (File I/O)

proc            6 (Processes)

memalloc        7 (Memory Allocation)

users_groups    8 (Users and Groups)

proccred        9 (Process Credentials)

time            10 (Time)

syslim          11 (System Limits and Options)

sysinfo         12 (System and Process Information)

filebuff        13 (File I/O Buffering)

filesys         14 (File Systems)

files           15 (File Attributes)

xattr           16 (Extended Attributes)

acl             17 (Access Control Lists)

dirs_links      18 (Directories and Links)

inotify         19 (Monitoring File Events)

signals         20 to 22 (Signals)

timers          23 (Timers and Sleeping)

procexec        24 (Process Creation), 25 (Process Termination),
                26 (Monitoring Child Processes), 27 (Program Execution),
                and 28 (Further Details on Process Creation and Program
                Execution)

threads         29 to 33 (POSIX Threads)

pgsjc           34 (Process Groups, Sessions, and Job Control)

procpri         35 (Process Priorities and Scheduling)

procres         36 (Process Resources)

daemons         37 (Daemons)

cap             39 (Capabilities)

loginacct       40 (Login Accounting)

shlibs          41 and 42 (Shared Libraries)
    
pipes           44 (Pipes and FIFOs)

svipc           45 (System V IPC)
    
svmsg           46 (System V Message Queues)

svsem           47 (System V Semaphores)

svshm           48 (System V Shared Memory)

mmap            49 (Memory Mappings)

vmem            50 (Virtual Memory Operations)

pmsg            52 (POSIX Message Queues)

psem            53 (POSIX Semaphores)

pshm            54 (POSIX Shared Memory)

filelock        55 (File Locking)

sockets         56 to 61 (Sockets and Network Programming)

tty             62 (Terminals)

altio           63 (Alternative I/O Models)

pty             64 (Pseudoterminals)

getopt          Appendix B: Parsing Command-Line Options
(C) 2017 Michael Kerrisk
