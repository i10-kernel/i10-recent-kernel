# SPDX-License-Identifier: GPL-2.0

ccflags-y				+= -I$(src)

obj-$(CONFIG_NVME_TARGET)		+= nvmet.o
obj-$(CONFIG_NVME_TARGET_LOOP)		+= nvme-loop.o
obj-$(CONFIG_NVME_TARGET_RDMA)		+= nvmet-rdma.o
obj-$(CONFIG_NVME_TARGET_FC)		+= nvmet-fc.o
obj-$(CONFIG_NVME_TARGET_FCLOOP)	+= nvme-fcloop.o
obj-$(CONFIG_NVME_TARGET_TCP)		+= nvmet-tcp.o
obj-$(CONFIG_I10_TARGET)		+= i10-target.o

nvmet-y		+= core.o configfs.o admin-cmd.o fabrics-cmd.o \
			discovery.o io-cmd-file.o io-cmd-bdev.o
nvmet-$(CONFIG_NVME_TARGET_PASSTHRU)	+= passthru.o
nvme-loop-y	+= loop.o
nvmet-rdma-y	+= rdma.o
nvmet-fc-y	+= fc.o
nvme-fcloop-y	+= fcloop.o
nvmet-tcp-y	+= tcp.o
i10-target-y	+= i10.o
nvmet-$(CONFIG_TRACING)	+= trace.o
