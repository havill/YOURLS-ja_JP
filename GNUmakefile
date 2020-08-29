dir# the below is the standard location of an Apache 
# HTML directory, and it assumes that YOURLS is installed
# in the root directory. Change if needed.

wwwdir = /var/www/html/user/language
binaries = ja_JP.mo

.PHONY: all
all: $(binaries)

ja_JP.mo: ja_JP.po
	msgfmt $^ -o $@

.PHONY: install
install: $(binaries)
	install -m 644 $(binaries) $(wwwdir)

.PHONY: clean
clean:
	@rm -f $(binaries)
