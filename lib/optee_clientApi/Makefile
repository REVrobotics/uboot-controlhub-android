#Copyright 2012 The Chromium Authors
#
# SPDX-License-Identifier:	GPL-2.0+
#

obj-y += OpteeClientMem.o
obj-y += OpteeClientApiLib.o
obj-y += OpteeClientInterface.o
obj-y += OpteeClientSMC.o
obj-y += OpteeClientRPC.o
obj-y += tee_smc-arm64.o
obj-y += 258be795-f9ca-40e6-a8699ce6886c5d5d.o
obj-y += OpteeClientRkFs.o

lib/optee_clientApi/258be795-f9ca-40e6-a8699ce6886c5d5d.o: lib/optee_clientApi/258be795-f9ca-40e6-a8699ce6886c5d5d.c
lib/optee_clientApi/258be795-f9ca-40e6-a8699ce6886c5d5d.c: lib/optee_clientApi/258be795-f9ca-40e6-a8699ce6886c5d5d.ta
	$(srctree)/lib/optee_clientApi/tabinary_to_cfile.py --prefix keymaster --TA $< --out $@
