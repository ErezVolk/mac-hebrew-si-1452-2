# A Modified Hebrew Keyboard for the Hebrew Typist

(Work in Progress)

## Background

As a translator who does a lot of typing in Hebrew, I find it inconvenient that
a number of "proper" Hebrew characters (makaf, geresh, greshayim) require a
modifier key to type, whereas the graphically similar Latin characters (minus
sign, apostrophe, quotation marks) are the natural thing to type. Historical
reasons aside, it's like the current Hebrew keyboard layouts are trying to make
it tough to use real Hebrew punctuation.

For this reason, I've started to experiment with a slightly modified version of
the Israeli standard layout (1452-2) that would flip the situation, making the
Hebrew punctuation natural to type and the foreign characters harder (only when
in Hebrew layout, of course).

Here are the changes (and [here](Hebrew%20Modified.dms?raw=true) is the installer):
- The minus sign now types ־ (makaf) without any modifiers and - (minus) with the
  level-3 modifier (AltGr/Option/⌥).
- The single/double quote key now produces a single/double upper mercha; to access
  the non-Hebrew characters when in Hebrew mode, use ⌥.
- The backslash (\) key now produces a geresh, allowing you to type צ׳ופצ׳יק without
  modifier keys. To get the backslash character (note that the Hebrew slash is the
  forward one), use Option+backtick.

The following table lists the changes:

| Key      | SI 1452-2                   | Hebrew Modified |
| -------- | --------------------------- | --------------- |
| -        | - U+002D HYPEN-MINUS                 | ־ U+05BE HEBREW PUNCTUATION MAQAF    |
| Option+- | ־ U+05BE HEBREW PUNCTUATION MAQAF    | - U+002D HYPEN-MINUS                 |
| '        | ' U+0027 APOSTROPHE                  | ’ U+2019 RIGHT SINGLE QUTATION MARK  |
| Option+, | ’ U+2019 RIGHT SINGLE QUTATION MARK  | ' U+0027 APOSTROPHE                  |
| Shift+'  | " U+0022 QUOTATION MARK              | ” U+201D RIGHT DOUBLE QUOTATION MARK |
| AltGt+L  | ” U+201D RIGHT DOUBLE QUOTATION MARK | " U+0022 QUOTATION MARK              |
| \        | \ U+005C REVERSE SOLIDUS             | ׳ U+05F3 HEBREW PUNCTUATION GERESH   |
| Option+` | ׳  U+05F3 HEBREW PUNCTUATION GERESH  | \ U+005C REVERSE SOLIDUS             |


## Random
- Is U+0022 QUTATION MARK really not needed? Google understands U+201D just as well...
- Modifier-less dagesh (common for disambiguation)?
- Some kind of compose sequence: maqaf-maqaf and geresh-geresh never appear in Hebrew text