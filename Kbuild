dtbo-$(CONFIG_ARCH_NEO) += display/neo-sde.dtbo \
		display/neo-sde-display-idp-overlay.dtbo \
		display/neo-sde-display-qxr-overlay.dtbo

ifneq ($(CONFIG_ARCH_QTI_VM), y)
dtbo-y += display/waipio-sde.dtbo \
#		display/waipio-sde-display-mtp-overlay.dtbo \
#		display/waipio-sde-display-cphy-mtp-overlay.dtbo \
#		display/waipio-sde-display-cdp-overlay.dtbo \
#		display/waipio-sde-display-qrd-overlay.dtbo \
#		display/waipio-sde-display-hdk-overlay.dtbo \
#		display/waipio-sde-display-waipio-lemur-cdp-overlay.dtbo \
#		display/waipio-sde-display-waipio-lemur-mtp-overlay.dtbo \
#		display/waipio-sde-display-rumi-overlay.dtbo

#PLUS_DTS_OVERLAY start
dtbo-y += oplus/wly-20846-display-waipio-overlay.dtbo
dtbo-y += oplus/mt-20845-display-waipio-overlay.dtbo
dtbo-y += oplus/jnc-20865-display-waipio-overlay.dtbo
dtbo-y += oplus/baize-21001-display-waipio-overlay.dtbo
dtbo-y += oplus/ferrari-21631-display-waipio-overlay.dtbo
dtbo-y += oplus/kunpeng-21009-display-waipio-overlay.dtbo
dtbo-y += oplus/jennie-21605-display-waipio-overlay.dtbo
dtbo-y += oplus/jennie-21606-display-waipio-overlay.dtbo
dtbo-y += oplus/ovaltine-21841-display-waipio-overlay.dtbo
#PLUS_DTS_OVERLAY end
else
dtbo-$(CONFIG_ARCH_WAIPIO) += display/trustedvm-waipio-sde-display-mtp-overlay.dtbo \
		display/trustedvm-waipio-sde-display-cdp-overlay.dtbo \
		display/trustedvm-waipio-sde-display-rumi-overlay.dtbo \
		display/trustedvm-waipio-sde-display-qrd-overlay.dtbo
endif

ifneq ($(CONFIG_ARCH_QTI_VM), y)
dtbo-$(CONFIG_ARCH_CAPE) += display/cape-sde.dtbo \
		display/cape-sde-display-atp-overlay.dtbo \
		display/cape-sde-display-cdp-overlay.dtbo \
		display/cape-sde-display-cdp-qhd-overlay.dtbo \
		display/cape-sde-display-mtp-overlay.dtbo \
		display/cape-sde-display-mtp-120fps-overlay.dtbo \
		display/cape-sde-display-mtp-nodisplay-overlay.dtbo \
		display/cape-sde-display-qrd-overlay.dtbo
else
dtbo-$(CONFIG_ARCH_CAPE) += display/trustedvm-cape-sde-display-qrd-overlay.dtbo
endif

ifneq ($(CONFIG_ARCH_QTI_VM), y)
dtbo-$(CONFIG_ARCH_DIWALI) += display/diwali-sde.dtbo \
		display/diwali-sde-display-atp-overlay.dtbo \
		display/diwali-sde-display-idp-overlay.dtbo \
		display/diwali-sde-display-idp-amoled-overlay.dtbo \
		display/diwali-sde-display-qrd-overlay.dtbo \
		display/diwali-sde-display-rumi-overlay.dtbo
else
dtbo-$(CONFIG_ARCH_DIWALI) += display/trustedvm-diwali-sde-display-idp-overlay.dtbo \
		display/trustedvm-diwali-sde-display-qrd-overlay.dtbo
endif

always-y    := $(dtb-y) $(dtbo-y)
subdir-y    := $(dts-dirs)
clean-files    := *.dtb *.dtbo