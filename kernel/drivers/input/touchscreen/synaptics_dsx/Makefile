ifneq ($(KERNELRELEASE),)
 obj-m += synaptics_dsx_i2c.o
 obj-m += synaptics_dsx_core.o
 obj-m += synaptics_dsx_fw_update.o

else
          KERNELDIR:=/hytruct/kernel_android6.0.1_2.1.0_cqsound
          CROSS_COMPILE:=/hytruct/prebuilts/gcc/linux-x86/arm/arm-linux-androideabi-4.9/bin/arm-linux-androideabi-
          PWD:=$(shell pwd)
  
default:
	$(MAKE) ARCH=arm CROSS_COMPILE=$(CROSS_COMPILE) -C $(KERNELDIR) M=$(PWD) modules LOADADDR=0x10008000 KCFLAGS=-mno-android
  
  
clean:
	rm -rf *.o *.order .*.cmd *.ko *.mod.c *.symvers *.tmp_versions 
endif
