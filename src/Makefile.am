geanyplugin_LTLIBRARIES		=	geanypy.la
geanyplugindir				=	$(libdir)/geany

geanypy_la_LDFLAGS			=	-module -avoid-version -Wl,--export-dynamic
geanypy_la_CPPFLAGS			=	@PYTHON_CPPFLAGS@ \
								-DGEANYPY_PYTHON_DIR="\"$(libdir)/geany/geanypy\"" \
								-DGEANYPY_PLUGIN_DIR="\"$(libdir)/geany\"" \
								-DG_LOG_DOMAIN=\"GeanyPy\"
geanypy_la_CFLAGS			=	@PYGTK_CFLAGS@ @GEANY_CFLAGS@ @GMODULE_CFLAGS@
geanypy_la_LIBADD			=	@GEANY_LIBS@ @PYGTK_LIBS@ \
								$(PYTHON_LDFLAGS) $(PYTHON_LIBS) \
								@PYTHON_EXTRA_LIBS@ @PYTHON_EXTRA_LDFLAGS@ \
								@GMODULE_LIBS@
geanypy_la_SOURCES			=	geanypy-app.c \
								geanypy-dialogs.c \
								geanypy-document.c geanypy-document.h \
								geanypy-editor.c geanypy-editor.h \
								geanypy-encoding.c geanypy-encoding.h \
								geanypy-filetypes.c geanypy-filetypes.h \
								geanypy-glog.c \
								geanypy.h \
								geanypy-highlighting.c \
								geanypy-indentprefs.c \
								geanypy-interfaceprefs.c \
								geanypy-keybindings.c geanypy-keybindings.h \
								geanypy-main.c \
								geanypy-mainwidgets.c \
								geanypy-msgwindow.c \
								geanypy-navqueue.c \
								geanypy-plugin.c geanypy-plugin.h \
								geanypy-prefs.c \
								geanypy-project.c geanypy-project.h \
								geanypy-scinotification.c \
								geanypy-scinotifyheader.c \
								geanypy-scintilla.c geanypy-scintilla.h \
								geanypy-search.c \
								geanypy-signalmanager.c geanypy-signalmanager.h \
								geanypy-templates.c \
								geanypy-uiutils.c geanypy-uiutils.h
