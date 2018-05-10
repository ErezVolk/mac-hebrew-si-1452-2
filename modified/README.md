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

- The <kbd>-</kbd> (minus) key now types ־ (maqaf) when used without any
  modifiers and - (minus) with the level-3 modifier
(<kbd>AltGr</kbd>/<kbd>OPTION</kbd>/<kbd>⌥</kbd>).

- The <kbd>\`</kbd> (backtick) key now produces a geresh instead of a
  semicolon, allowing you to type צ׳ופצ׳יק without modifier keys. To get the
semicolon character, use <kbd>⇮</kbd>+<kbd>\`</kbd>.

- More experimentally, I've created a "dead key" combination:

  - Since maqaf-maqaf is never used in Hebrew, typing that sequence will
    produce a minus symbol (-).

  - The same goes for geresh-geresh to produce a semicolon (;).

  - And by analogy, typing the equal sign twice produces qav mafrid (en-dash).

  - This proved so convenient to me, that I went ahead and created double-click
    versions of the shin/sin dots, since the sequences ץץ and ןן don't occur
    in normal Hebrew text.

The following table lists the changes (<kbd>⇧</kbd> = Level 2 Select (<kbd>Shift</kbd>);
<kbd>⇮</kbd> = Level 3 Select (<kbd>AltGr</kbd>/<kbd>Option</kbd>)):

| Key (Sequence)               | SI 1452-2                             | Hebrew Modified                       |
| ---------------------------- | ------------------------------------- | ------------------------------------- |
| <kbd>-</kbd>                 | - U+002D HYPEN-MINUS                  | ־ U+05BE HEBREW PUNCTUATION MAQAF     |
| <kbd>⇮</kbd>+<kbd>-</kbd>    | ־ U+05BE HEBREW PUNCTUATION MAQAF     | - U+002D HYPEN-MINUS                  |
| <kbd>\`</kbd>                | ; U+003B SEMICOLON                    | ׳ U+05F3 HEBREW PUNCTUATION GERESH    |
| <kbd>⇮</kbd>+<kbd>\`</kbd>   | ׳  U+05F3 HEBREW PUNCTUATION GERESH   | ; U+003B SEMICOLON                    |
| <kbd>-</kbd> <kbd>-</kbd>    | - -                                   | - U+002D HYPHEN-MINUS                 |
| <kbd>\`</kbd> <kbd>\`</kbd>  | \` \`                                 | ; U+003B SEMICOLON                    |
| <kbd>=</kbd> <kbd>=</kbd>    | = =                                   | – U+2013 EN DASH                      |
| <kbd>Q</kbd> <kbd>Q</kbd>    | ץ ץ                                   | U+05C2 HEBREW POINT SIN DOT           |
| <kbd>W</kbd> <kbd>W</kbd>    | ן ן                                   | U+05C1 HEBREW POINT SHIN DOT          |


## Random
- Apostrophe and (Latin) quotation marks are fine, even though they're not proper Hebrew punctuation,
  since we don't use different opening/closing quotes.
- Dead keys open up a whole new world.
- Add the Yiddish digraphs
- Level-4 modifieres? Should be good for cantillation marks
- What am I missing?
