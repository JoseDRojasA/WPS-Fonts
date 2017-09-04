# WPS Office Fonts

These are the symbol fonts required by wps-office. They are used to display math formulas. We have collected the fonts here to make things easier.

Create a sub directory in your system's fonts directory. This is usually `/usr/share/fonts`, otherwise consult your distribution's documentation.
```
sudo mkdir /usr/share/fonts/wps-fonts
```

Move fonts to the new directory.
```
sudo mv ttf-wps-fonts/* /usr/share/fonts/wps-fonts
```

Fix the file permissions.
```
sudo chmod 644 /usr/share/fonts/wps-fonts/*
```
Rebuild the font cache.
```
sudo fc-cache -vfs
```

Clean up the `tmp` directory.
```
rm -rf /tmp/ttf-wps-fonts
```





