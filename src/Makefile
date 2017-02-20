SRC = output_repair.cpp xml_repair.cpp json_repair.cpp

OBJ += 

INCLUDES= 

LIBS =

CLEANFILES = output-repair$(EXEEXT)

include config.inc
include common

all: output-repair$(EXEEXT)

###############################################################################

output-repair$(EXEEXT): $(OBJ)
	$(LINKBIN)

.PHONY: output-repair-mac-signed

output-repair-mac-signed: output-repair$(EXEEXT)
	codesign -v -s $(OSX_IDENTITY) output-repair$(EXEEXT)

