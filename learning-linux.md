# Learning Linux

| shortcut | used for       |
| -------- | -------------- |
| ctrl + R | search         |
| ctrl + L | clear          |
| ctrl + U | cut text       |
| ctrl + Y | paste cut text |

---

```bash
echo "some text" > hello.text
```

adds some text and removes everything else

```bash
echo "some more text" >> hello.text
```

appends some text

Search

```bash
find . -name "*.csv"
```

finds all csv files in current directory

```bash
find . -type f -size +100k
```

find files heavier than 100k

```bash
ls -lh
```

detail all files in a directory

```bash
tail text.txt
```

outputs last 10 lines and -f for recursive

```bash
ps aux | grep firefox
```

to find a process

```bash
kill -9 1342
```

kills process id (i.e 1342) immediately

```bash
killall firefox
```

kills firefox immediately

```bash
cat /proc/cpuinfo
```

```bash
cat /proc/meminfo
```

```bash
cat /proc/2860/status
```

displays the detail of given process id

```bash
watch 'cat /proc/2860/status | grep voluntary'
```

executes the command after every 2s
watch is best for repeated interaction

```bash
watch -n 1 'ls -l | wc'
```

check for number of files in folder real-time (useful for checking download status )
