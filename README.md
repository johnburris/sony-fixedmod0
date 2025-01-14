# Sony FixedMOD0

## Overview
**FixedMOD0** is a modification to Sony's 8x16 Fixed font, one of the default X11 fonts. The Latin (`8x16.pcf`) and Katakana (`8x16rk.pcf`) versions have been merged, and it has been re-encoded from `jisx0201.1972` to `ISO 10646-1`. Some characters have been added or modified. Please see the changelog for more details. A shell script (`demo.sh`) is included that shows all the characters.

## Quickstart
On Debian:
```
git clone https://github.com/johnburris/sony-fixedmod0.git
cd sony-fixedmod0
sudo mkdir /usr/share/fonts/local
sudo cp FixedMOD0Medium-16.bdf /usr/share/fonts/local/
sudo chmod 644 /usr/share/fonts/local/*.bdf
sudo chown root:root /usr/share/fonts/local/*.bdf
sudo mkfontdir /usr/share/fonts/local
xset fp rehash
```
It should appear on your system like so:
```
-sony-fixedmod0-medium-r-normal-*-16-*-*-*-*-*-iso10646-1
```

## Changelog

### BASIC LATIN
-"0" Shortened and struckthrough
-"7" Shortened and struckthrough
-"N" Modified
-"HYPEN-MINUS" Shortened

### GENERAL PUNCTUATION
-"EN/EM DASH" Added

### MATHEMATICAL OPERATORS
-"GREATER/LESS-THAN OR EQUAL TO" Added
-"NOT EQUAL TO" Modified to match "="

### MISCELLANEOUS SYMBOLS
-"ORTHODOX CROSS" Added

### DINGBATS
-"LATIN CROSS" Added
-"SHADOWED WHITE LATIN CROSS" Added
