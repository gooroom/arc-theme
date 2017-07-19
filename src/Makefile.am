themedir     = $(datadir)/themes/Arc
ithemedir     = $(DESTDIR)$(themedir)

install-exec-hook:

install-data-local:

	$(MKDIR_P) $(ithemedir)
	cp $(srcdir)/index.theme $(ithemedir)

	$(MKDIR_P) $(ithemedir)/gtk-2.0
	cd $(srcdir)/gtk-2.0 && cp -Rv \
			assets \
			menubar-toolbar	\
			*.rc \
			gtkrc \
			$(ithemedir)/gtk-2.0

	$(MKDIR_P) $(ithemedir)/gtk-3.0
	cd $(srcdir)/gtk-3.22 && ./parse-sass.sh && cp -Rv \
			assets \
			gtk.css \
			$(ithemedir)/gtk-3.0


	$(MKDIR_P) $(ithemedir)/xfwm4
	cd $(srcdir)/xfwm4 && cp -Rv \
		*.png \
		themerc		\
		$(ithemedir)/xfwm4

uninstall-local:
	rm -rf $(ithemedir)
