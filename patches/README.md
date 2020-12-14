## Makefile
``` diff
@@ -29,7 +29,7 @@ stest: stest.o
	$(CC) -o $@ stest.o $(LDFLAGS)

clean:
-	rm -f dmenu stest $(OBJ) dmenu-$(VERSION).tar.gz
+	rm -f dmenu stest $(OBJ) dmenu-$(VERSION).tar.gz *.rej *.orig
+	rm config.h

dist: clean
	mkdir -p dmenu-$(VERSION)
```

# Patches
The order in which to apply these patches to a clean dmenu build is the following(a couple of really easy hunks have to be manually applied here and there):
- fuzzies
- center
- borderoption
- ~~lineheight~~ [don't patch it next time, useless with any multimonitor setup]
- xresforfuzzy
- password (reverse patch!!)
- xyw
{
	add joypixels and change font size:
	"monospace:size=16",
	"Noto Color Emoji:pixelsize=16:antialias=true:autohint=true"
}
- mouse support
- rejectnomatch (-r support, i.e. useful for dmenu-aliases script)
- remove "iscol [...]"
- change keybinding for `paste` to `ctrl+v`.
