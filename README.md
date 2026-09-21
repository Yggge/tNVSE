Windows-1251 support

tNVSE supports Windows-1251 (CP1251) text encoding for Russian localization.

Set the following in tnvse.ini:

[Multibyte]

bEnableMultibyteFontHook = 0
uiEncoding = 5

uiEncoding = 5 selects Windows-1251.

CP1251 text is converted to Unicode before being rendered by FreeType, allowing standard Unicode TTF fonts with Cyrillic glyphs to be used without modifying or remapping the font.

This mode does not require the multibyte font hooks.
