
include $(srctree)/drivers/misc/mediatek/Makefile.custom

# Module project related part

ifeq ($(CONFIG_MTK_SENSOR_SUPPORT),y)
ifeq ($(CONFIG_MTK_MC3XXX),y)
obj-y   +=  accelerometer/mc3xxx/
endif

ifeq ($(CONFIG_MTK_KXTJ2_1009),y)
obj-y   +=  accelerometer/KXTJ2_1009/
endif

endif

ifneq ($(CONFIG_ARCH_MTK_PROJECT),)
ARCH_MTK_PROJECT := $(shell echo $(CONFIG_ARCH_MTK_PROJECT))
obj-y	+= core/
obj-y	+= dct/dct/
endif

obj-y   +=  lcm/
#obj-y	+=  hdmi/
obj-y	+=  camera/camera/
obj-y	+=  imgsensor/ov5648_mipi_raw/
obj-y	+=  imgsensor/ov2659_yuv/
obj-y	+=  imgsensor/ov2686_yuv/
obj-y   +=  flashlight/constant_flashlight/
obj-y	+=  vibrator/
obj-y	+=  leds/
obj-y	+=  keypad/
obj-y	+=  sound/
obj-y	+=  accdet/
obj-y	+=  partition/
obj-y 	+=  multibridge/sn65dsi8x/

