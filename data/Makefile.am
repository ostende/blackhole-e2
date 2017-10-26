SUBDIRS = fonts keymaps

dist_pkgdata_DATA = \
	encoding.conf \
	black.mvi \
	freesat.t1 \
	freesat.t2 \
	hd-testcard.mvi \
	iso-639-3.pck \
	distro-logo.png \
        *.xml \
        *.bh

if HAVE_TEXTLCD
SUBDIRS += displaytext
endif

if HAVE_COLORLCD
SUBDIRS += display96
endif

if HAVE_COLORLCD2
SUBDIRS += display96
endif

if HAVE_COLORLCD3
SUBDIRS += display128dm
endif

if HAVE_COLORLCD128
SUBDIRS += display128
endif

if HAVE_COLORLCD220
SUBDIRS += display220
endif

if HAVE_COLORLCD400
SUBDIRS += display400
endif

if HAVE_COLORLCD400DM
SUBDIRS += display400dm
endif

if HAVE_COLORLCD480
SUBDIRS += display480
endif

if HAVE_COLORLCD720
SUBDIRS += display720
endif

if HAVE_COLORLCD800
SUBDIRS += display800
endif

if HAVE_BWLCD255
SUBDIRS += vfd255
endif

if HAVE_BWLCD140
SUBDIRS += vfd140
endif

if HAVE_BWLCD128
SUBDIRS += vfd128
endif

iso-639-3.pck: $(srcdir)/iso-639-3.tab
	python $(srcdir)/convert-iso-639-3.py $< $@
