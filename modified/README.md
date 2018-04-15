# A Modified Hebrew Keyboard for the Hebrew Typist

(Work in Progress)

## Background

As a translator who does a lot of typing in Hebrew, I find it inconvenient that
a number of "proper" Hebrew characters (maqaf, geresh, gershayim) require a
modifier key to type, whereas the graphically similar Latin characters (minus
sign, apostrophe, quotation marks) are the natural thing to type. Historical
reasons aside, it's like the current Hebrew keyboard layouts are trying to make
it tough to use real Hebrew punctuation.

For this reason, I've started to experiment with a slightly modified version of
the Israeli standard layout (1452-2) that would flip the situation, making the
Hebrew punctuation natural to type and the foreign characters harder (only when
in Hebrew layout, of course).

Here are the changes (and [here](Hebrew%20Modified.dms?raw=true) is the MacOS installer):

- The <kbd>-</kbd> (minus) key now types ־ (maqaf) without any modifiers and -
  (minus) with the level-3 modifier (<kbd>AltGr</kbd>/<kbd>OPTION</kbd>/<kbd>⌥</kbd>).

- The <kbd>\\</kbd> (backslash> key now produces a geresh, allowing you to type
  צ׳ופצ׳יק without modifier keys. To get the backslash character (note that the
Hebrew slash is the forward one), use <kbd>⇮</kbd>+<kbd>`</kbd>.

- More experimentally, I've created two "dead key" combinations:
  - Since geresh-geresh is never used in Hebrew, typing that sequence will produce
    gershayim.
  - Since maqaf-maqaf is equally unused, typing that sequence will produce _a dagesh_
    symbol. A kav mafrid may seem more natural, but the rationale is that a dagesh
    is often used for disambiguation of words, and I want to reduce the use of the
    thumb for common things.

The following table lists the changes (<kbd>⇧</kbd> = Level 2 Select (<kbd>Shift</kbd>);
<kbd>⇮</kbd> = Level 3 Select (<kbd>AltGr</kbd>/<kbd>Option</kbd>)):

| Key (Sequence)             | SI 1452-2                             | Hebrew Modified                       |
| -------------------------- | ------------------------------------- | ------------------------------------- |
| <kbd>-</kbd>               | - U+002D HYPEN-MINUS                  | ־ U+05BE HEBREW PUNCTUATION MAQAF     |
| <kbd>⇮</kbd>+<kbd>-</kbd>  | ־ U+05BE HEBREW PUNCTUATION MAQAF     | - U+002D HYPEN-MINUS                  |
| <kbd>\\</kbd>              | \ U+005C REVERSE SOLIDUS              | ׳ U+05F3 HEBREW PUNCTUATION GERESH    |
| <kbd>⇮</kbd>+<kbd>\`</kbd> | ׳  U+05F3 HEBREW PUNCTUATION GERESH   | \ U+005C REVERSE SOLIDUS              |
| <kbd>-</kbd> <kbd>-</kbd>  | - -                                   | ״ U+05F4 HEBREW PUNCTUATION GERSHAYIM |
| <kbd>\\</kbd> <kbd>\\</kbd>| \ \                                   |   U+05BC HEBREW POINT DAGESH OR MAPIQ |


## Random
- Apostrophe and (Latin) quotation marks are fine, even though they're not proper Hebrew punctuation,
  since we don't use different opening/closing quotes.
- Dead keys open up a whole new world.
- What am I missing?
