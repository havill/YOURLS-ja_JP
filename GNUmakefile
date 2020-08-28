binaries = ja_JP.mo

.PHONY: all
all: $(binaries)

ja_JP.mo: ja_JP.po
	msgfmt $^ -o $@

.PHONY: clean
clean:
	@rm -f $(binaries)
