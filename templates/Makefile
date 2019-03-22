# Toplevel Makefile for Xymon
BUILDTOPDIR=`pwd`
CLIENTONLY = yes
LOCALCLIENT = no

# configure settings for Xymon
#
# Toplevel dir
XYMONTOPDIR = {{ xymon_client_directory }}

# Xymon settings follows
#
# Username running Xymon
XYMONUSER = {{ xymon_client_user_group }}
# Xymon server IP-address
XYMONHOSTIP = {{ xymon_server_address }}
# Large File Support settings
LFSDEF = -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
LIBRTDEF =

include build/Makefile.Linux


#
# Add local CFLAGS etc. settings here

include build/Makefile.rules
