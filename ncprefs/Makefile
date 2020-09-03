include $(THEOS)/makefiles/common.mk

BUNDLE_NAME = NCPrefs

SYSROOT = $(THEOS)/sdks/iPhoneOS11.2.sdk
NCPrefs_FILES = NCDRootListController.m
NCPrefs_INSTALL_PATH = /Library/PreferenceBundles
NCPrefs_FRAMEWORKS = UIKit
NCPrefs_PRIVATE_FRAMEWORKS = Preferences
NCPrefs_CFLAGS = -fobjc-arc

include $(THEOS_MAKE_PATH)/bundle.mk

internal-stage::
	$(ECHO_NOTHING)mkdir -p $(THEOS_STAGING_DIR)/Library/PreferenceLoader/Preferences$(ECHO_END)
	$(ECHO_NOTHING)cp entry.plist $(THEOS_STAGING_DIR)/Library/PreferenceLoader/Preferences/NCPrefs.plist$(ECHO_END)
