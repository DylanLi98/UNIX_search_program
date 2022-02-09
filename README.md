# UNIX_search_program

a popular UNIX command that traverses a file hierarchy and performs various functions on each file in the hierarchy.

## Usage

```
To compile
>  gcc unix.c

To run: ./<name of executable> <commands and arguments> <directory>

To execute
ex: ./executable -f txt -S -s 100 -t f ./projects/
ex: ./a.out -S -f c -e "wc -l"
ex: ./a.out -S -s 1024 -e "ls -l"
```

To use Makefile type

> make

### Output

```
$ ./a.out -e "ls -l"
/home/UAB/duo1998/project2
-rwxr-xr-x 1 duo1998 domain users 13688 Oct 31 14:48 a.out
	a.out
-rwxr-xr-x 1 duo1998 domain users 8257 Oct 31 14:48 hw3.c
	hw3.c
-rwxr-xr-x 1 duo1998 domain users 12 Oct 31 14:30 input.txt
	input.txt
-rwxr-xr-x 1 duo1998 domain users 19296 Oct 31 13:46 lab7
	lab7
-rwxr-xr-x 1 duo1998 domain users 2837 Oct 30 19:14 lab7.c
	lab7.c
-rwxr-xr-x 1 duo1998 domain users 39 Oct 11 00:44 Makefile
	Makefile
-rwxr-xr-x 1 duo1998 domain users 0 Oct 31 14:31 output.log
	output.log
-rwxr-xr-x 1 duo1998 domain users 6950 Oct 30 18:49 project2.c
	project2.c
-rwxr-xr-x 1 duo1998 domain users 9728 Oct  9 23:43 projects.tar
	projects.tar
```

```
$ ./a.out -S -e "ls -l"
/home/UAB/duo1998/project2
-rwxr-xr-x 1 duo1998 domain users 13688 Oct 31 14:48 a.out
	a.out 13688
-rwxr-xr-x 1 duo1998 domain users 8257 Oct 31 14:48 hw3.c
	hw3.c 8257
-rwxr-xr-x 1 duo1998 domain users 12 Oct 31 14:30 input.txt
	input.txt 12
-rwxr-xr-x 1 duo1998 domain users 19296 Oct 31 13:46 lab7
	lab7 19296
-rwxr-xr-x 1 duo1998 domain users 2837 Oct 30 19:14 lab7.c
	lab7.c 2837
-rwxr-xr-x 1 duo1998 domain users 39 Oct 11 00:44 Makefile
	Makefile 39
-rwxr-xr-x 1 duo1998 domain users 0 Oct 31 14:31 output.log
	output.log 0
-rwxr-xr-x 1 duo1998 domain users 6950 Oct 30 18:49 project2.c
	project2.c 6950
-rwxr-xr-x 1 duo1998 domain users 9728 Oct  9 23:43 projects.tar
	projects.tar 9728
```

```
$ ./a.out -S -s 1024 -e "ls -l"
/home/UAB/duo1998/project2
-rwxr-xr-x 1 duo1998 domain users 13688 Oct 31 14:48 a.out
	a.out 13688
-rwxr-xr-x 1 duo1998 domain users 8257 Oct 31 14:48 hw3.c
	hw3.c 8257
-rwxr-xr-x 1 duo1998 domain users 19296 Oct 31 13:46 lab7
	lab7 19296
-rwxr-xr-x 1 duo1998 domain users 2837 Oct 30 19:14 lab7.c
	lab7.c 2837
-rwxr-xr-x 1 duo1998 domain users 6950 Oct 30 18:49 project2.c
	project2.c 6950
-rwxr-xr-x 1 duo1998 domain users 9728 Oct  9 23:43 projects.tar
	projects.tar 9728
```

```
$ ./a.out -S -s 1024 -f c -e "ls -l"
/home/UAB/duo1998/project2
-rwxr-xr-x 1 duo1998 domain users 8257 Oct 31 14:48 hw3.c
	hw3.c 8257
-rwxr-xr-x 1 duo1998 domain users 2837 Oct 30 19:14 lab7.c
	lab7.c 2837
-rwxr-xr-x 1 duo1998 domain users 6950 Oct 30 18:49 project2.c
	project2.c 6950
-rwxr-xr-x 1 duo1998 domain users 9728 Oct  9 23:43 projects.tar
	projects.tar 9728
```

```
$ ./a.out -S -s 1024 -f tar -e "ls -l"
/home/UAB/duo1998/project2
-rwxr-xr-x 1 duo1998 domain users 9728 Oct  9 23:43 projects.tar
	projects.tar 9728
```

```
$ ./a.out -s 1024 -f c -e "wc -l"
/home/UAB/duo1998/project2
236 hw3.c
	hw3.c
107 lab7.c
	lab7.c
225 project2.c
	project2.c
0 projects.tar
	projects.tar
```

## Contact me

Author: Duo Li

Blazer: duo1998

Email: duo1998@uab.edu
