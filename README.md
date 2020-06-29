# perl-rename

Perl `rename` command line, with no dependencies.

Originally written by Larry Wall, updated by Robin Barker.

# Example

```
$ ls -1
1.txt
2.txt
3.txt
```

Command:
```
$ rename -n 's/(\d+)/sprintf "%03d", $1/e' *.text
```

Output:
```
rename(1.text, 001.text)
rename(2.text, 002.text)
rename(3.text, 003.text)
```
