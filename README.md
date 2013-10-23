Tcl-Dict
========

#forked# An implementaion of tcl dict

A backport of the Tcl 8.5 [dict] command for Tcl 8.4.

Updated: 17 November 2005.

The original dict extension from May 2004 has been updated with todays code
from the Tcl CVS repository.

This version doesn't have support for mp_int, because 8.4 has no such support.

April 2004.

This is a backport of the Tcl 8.5 [dict] command for Tcl 8.4. 

Most code was taken straight from from the Tcl-core CVS HEAD and
sampleextension on 14 April 2004. I glued it together with the help of
Donal K. Fellows, Don G. Porter and others to make this extension.

Perhaps the most significant change in the code is that it is slighly
less efficient than the real thing, mostly because some optimization
tricks are only available when linking against tclInt.h, not tcl.h.

- Pascal Scheffers.
