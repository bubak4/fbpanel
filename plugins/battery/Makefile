## miniconf makefiles ## 1.1 ##

TOPDIR := ../..

# power_supply.c is used only by os_linux.c which is included based on
# platform in battery.c, compiling it here does no harm even on other
# platforms than linux -- it just won't be used and linked to shared
# library
battery_src = battery.c power_supply.c
battery_cflags = -DPLUGIN $(GTK2_CFLAGS)
battery_libs = $(GTK2_LIBS)
battery_type = lib

include $(TOPDIR)/.config/rules.mk
