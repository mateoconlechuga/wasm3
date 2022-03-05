# ----------------------------
# Makefile Options
# ----------------------------

NAME = WASM3
ICON = icon.png
DESCRIPTION = "Wasm3"
COMPRESSED = YES
ARCHIVED = NO

CFLAGS = -Wall -Wextra -Oz \
         -Wno-extern-initializer -Wno-unused-function -Wno-unused-variable \
         -Wno-unused-parameter -Wno-missing-field-initializers -Iwasm3 \
         -Dd_m3HasFloat=0 \
         -Dd_m3MaxFunctionStackHeight=512 \
         -Dd_m3CodePageAlignSize=1 \
         -Dd_m3Use32BitSlots=0 \
         -Dd_m3MaxConstantTableSize=64 \
         -Dd_m3FixedHeap=32768 \
         -Dd_m3FixedHeapAlign=1 \
         -Dd_m3CascadedOpcodes=0 \
         -DM3_ARCH="\"ez80\""

EXTRA_CSOURCES = $(wildcard wasm3/*.c)
EXTRA_USERHEADERS = $(wildcard wasm3/*.h)

# ----------------------------

include $(shell cedev-config --makefile)
