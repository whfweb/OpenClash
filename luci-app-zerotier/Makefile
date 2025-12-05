include $(TOPDIR)/rules.mk

PKG_NAME:=luci-app-zerotier
PKG_VERSION:=1.0
PKG_RELEASE:=17

PKG_MAINTAINER:=The LuCI Team <luci@lists.subsignal.org>
PKG_LICENSE:=Apache-2.0

LUCI_TITLE:=LuCI Support for ZeroTier
LUCI_DEPENDS:=+zerotier
LUCI_PKGARCH:=all

include $(TOPDIR)/feeds/luci/luci.mk

# call BuildPackage - OpenWrt buildroot signature

define Package/$(PKG_NAME)
  SECTION:=luci
  CATEGORY:=LuCI
  SUBMENU:=3. Applications
  TITLE:=ZeroTier LuCI Interface
  PKGARCH:=all
  DEPENDS:=+luci-base +zerotier
endef

define Package/$(PKG_NAME)/description
  LuCI web interface for ZeroTier - secure peer-to-peer networking.
endef

$(eval $(call BuildPackage,$(PKG_NAME)))

