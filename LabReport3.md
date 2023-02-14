# Lab Report 3
## by Ishaan Kale

### Command 1

```grep -i``` ignores case sensitivity when searching through lines of a file.

```
grep "japan" HistoryJapan.txt

```
```
grep -i "japan" HistoryJapan.txt
        (“Chronicles of Japan”), the islands of Japan were born of a marriage
        who endowed the Japanese imperial family with its regalia of bronze
        Before you dismiss all this as the mere “myth” of Japan’s
        origins, remember that the Japanese continued to trace the imperial
        followed Japan’s best-known novelist Yukio Mishima in deploring this
        Japan’s origins.........
```
 
This example shows that since "Japan" is never spelled out lowercase, a normal search
will not find any results. However using ```grep -i``` will solve this issue.

```
grep "Lucca" IntroItaly.txt 
Tuscany — where lie the ageless beauties of Pisa, Lucca, Florence, and
```
```
grep -i "Lucca" IntroItaly.txt
Tuscany — where lie the ageless beauties of Pisa, Lucca, Florence, and
```

This example shows that case doesn't matter in this instance because the initial search
was specific enough for case to not matter.

### Command 2

```grep -n``` will show the line number in the text file for each found line with the word.

```
grep -n "Japan" HistoryJapan.txt 
9:        (“Chronicles of Japan”), the islands of Japan were born of a marriage
12:        who endowed the Japanese imperial family with its regalia of bronze
15:        Before you dismiss all this as the mere “myth” of Japan’s
16:        origins, remember that the Japanese continued to trace the imperial
19:        followed Japan’s best-known novelist Yukio Mishima in deploring this
22:        Japan’s origins.
27:        Sakhalin Island and northern Japan some 100,000 years ago. These
28:        migrants, who later settled throughout the Japanese archipelago, were
49:        third-century Chinese documents speak of a Japanese priestess-queen,
52:        centuries later, Japan’s own Kojiki and Nihon-shoki chronicles describe
59:        begins with the arrival of Korean scribes at the Japanese court around
60:        a.d. 400, at a time when Japan also had a military foothold in southern
61:        Korea. The state of Yamato, as early Japan was known, was organized
66:        The Japanese were forced out of the Korean peninsula in the
```
This quote shows the line numbers included with each line where "Japan" is found. This
is useful when attempting locate a usage in a large file.

```
grep -n "japan" HistoryJapan.txt 

```
```grep -n``` will still return nothing if not a single line is found.

### Command 3
