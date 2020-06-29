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
1.text renamed as 001.text
2.text renamed as 002.text
3.text renamed as 003.text

```
