ifeq ($(CONFIG_OPPO_FINGERPRINT),y)
obj-y        += oppo_fp_common/
obj-y        += fpc/
ifneq ($(filter MSM_18081 MSM_18381 MSM_18181 MSM_18385 MSM_18097 MSM_18041 MSM_18099 MSM_18397 MSM_18115 MSM_18501 MSM_18503, $(OPPO_TARGET_DEVICE)),)
obj-y        += goodix_optical_fp/
obj-y        += silead/
endif
ifneq ($(filter MSM_17011 MSM_17015 MSM_17081 MSM_17085, $(OPPO_TARGET_DEVICE)),)
obj-y        += goodix_fp/
endif
ifneq ($(filter full_oppo6763 full_oppo6771, $(shell echo $(TARGET_PRODUCT) | sed -e 's/_1.*//g')),)
obj-y        += goodix_fp/
endif
endif
