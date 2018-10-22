GUILD = @GUILD@
GUILE_SITE_CCACHE = @GUILE_SITE_CCACHE@

bin_SCRIPTS = conf-service
CLEANFILES = $(bin_SCRIPTS)

all-local: conf-service.go

conf-service.go: conf-service
	$(GUILD) compile -o $@ $<

clean-local:
	rm -f conf-service.go

install-exec-local:
	$(INSTALL) -D conf-service.go $(GUILE_SITE_CCACHE)/conf-service.go
	$(MKDIR_P) /var/lib/conf-service



