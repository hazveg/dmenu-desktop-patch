# dmenu-desktop-patch

commit 13911e8:
> This patch allows dmenu to use .desktop files from a given list of
> directories. The directories are defined in dmenu_desktop_path. The name
> of the Desktop Entry is extracted from the file and a relationship
> between it and its file is output with format {FILE};{NAME} by
> dmenu_desktop_name. This is then taken by dmenu_run_desktop; which
> passes the names into dmenu. The returning string from dmenu is then
> related back to the file and it is executed.
> OOTB functionality of dmenu is unaffected.
    
> It is recommended to use with the 'case insensitive' patch.

Just a little patch I wrote to use dmenu with XDG Desktop Entries.
A bit too cowardly to try getting this onto suckless.org.
Don't really think it's up to snuf anyway.

# For myself

How to create diffs: [suckless.org](https://suckless.org/hacking/)
How to apply patches[^1]:
```bash
patch -i {PATCH NAME}
```

[^1]: I have forgotten before.
