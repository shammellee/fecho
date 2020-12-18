# fecho

fecho appends text to a set of files

```sh
$ ls
file_1 file_2 file_3

$ ./fecho "foo bar baz" file*
$ cat file*
foo bar baz  // contents of file_1
foo bar baz  // contents of file_2
foo bar baz  // contents of file_3

# Special character support
$ ./fecho "line 1\nline 2\nline 3" file_4
$ cat file_4
line 1
line 2
line 3
```

## Notes

* Directories are ignored if specified
* If a specified file doesn't exist, it is created

