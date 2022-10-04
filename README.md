# How To Use libft-unit-test For The 42 Vienna Core Curriculum

The repository https://github.com/alelievr/libft-unit-test is a great resource for automatically testing and benchmarking your libft library. This tutorial should help you with installing and using these tests. 

## Prerequisites for the tests:
1. You should already have all the required files (ft_*.c, libft.h, Makefile) in your libft directory, even if your .c files or libft.h are empty.
2. Your Makefile to create libft.a should already be working. I am not allowed to share working code here but what your Makefile should do is:
  - Create .o files from your .c files
  - Create libft.a from those .o files.

A good resource to learn about Makefile is www.makefiletutorial.com and https://www.gnu.org/software/make/.

## Installing the tests
1. Rename your local libft directory/repo to "libft".
2. Change to the libft's parent directory and clone the libft-unit-test repository:

```
git clone https://github.com/alelievr/libft-unit-test.git
```

Your folder structure should now look like this:
```
.
|- libft/
|- libft-unit-tests/
```
3. Edit libft/Makefile and add the following rule to the bottom:
```
so:
	$(CC) -nostartfiles -fPIC $(CFLAGS) $(SRC)
	gcc -nostartfiles -shared -o libft.so $(OBJ)
```
Change `$(CC)`, `$(SRC)` and `$(OBJ)` to the variable names you used for your compiler, your source and object files in your Makefile. You don't need to change `$(CFLAGS)` even if you haven't defined this variable.

4. Change to the libft-unit-tests directory
5. Complete the installation by running

```
make
```
Your tests should be correctly installed now!

## Running the tests
1. Go to the libft-unit-tests directory and run

```
make f
```
You should now see your test results!

For more information on the test results visit the official documentation for libft-unit-tests: https://github.com/alelievr/libft-unit-test#usage

## Questions?
Write me on Discord: Francis Rafal#1334
