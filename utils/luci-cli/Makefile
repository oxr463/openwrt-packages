include $(TOPDIR)/rules.mk

PKG_NAME:=luci-cli
PKG_VERSION:=0.1.0
PKG_RELEASE:=1

include $(INCLUDE_DIR)/package.mk

define Package/
  SECTION:=
  CATEGORY:=
  TITLE:=
endef

define Package/luci-cli/description
  OpenWrt luci command-line tool
endef

define Build/Prepare
  mkdir -p $(PKG_BUILD_DIR)
  cp $(SOURCE_DIR)/* $(PKG_BUILD_DIR)
  $(Build/Patch)
endef

define Build/Compile

endef

define Package/luci-cli/install
  $(INSTALL_DIR) $(1)/usr/bin
  $(INSTALL_BIN) $(PKG_BUILD_DIR)/luci-cli $(1)/usr/bin
endef

$(eval $(call BuildPackage,luci-cli))
