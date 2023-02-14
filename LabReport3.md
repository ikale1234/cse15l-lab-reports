# Lab Report 3
## by Ishaan Kale

### Command 1

```grep -i``` ignores case sensitivity when searching through lines of a file.
```grep "japan" HistoryJapan.txt```
```
grep -i "japan" HistoryJapan.txt
        (“Chronicles of Japan”), the islands of Japan were born of a marriage
        who endowed the Japanese imperial family with its regalia of bronze
        Before you dismiss all this as the mere “myth” of Japan’s
        origins, remember that the Japanese continued to trace the imperial
        followed Japan’s best-known novelist Yukio Mishima in deploring this
        Japan’s origins.........```
 
This example shows that since "Japan" is never spelled out lowercase, a normal search
will not find any results. However using ```grep -i``` will solve this issue.
