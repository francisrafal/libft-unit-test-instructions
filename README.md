# How To Use libft-unit-test for the 42 Vienna Core Curriculum

The repository https://github.com/alelievr/libft-unit-test is a great resource for automatically testing and benchmarking your libft library. This guide should help you with installing and using these tests.

## Prerequisites for the tests:
1. You should already have all the required files (ft_*.c, libft.h, Makefile) in your libft directory
2. Your Makefile to create libft.a should already be working. I am not allowed to share working code here but what your Makefile should do is:
  - Create .o files from your .c files
  - Create libft.a from those .c files.

A good resource to learn about Makefiles is www.makefiletutorial.com and https://www.gnu.org/software/make/.

## Installing the tests
1. Rename your local libft directory/repo to "libft".
2. Change to the libft's parent directory and clone the libft-unit-test repository:

```
git clone https://github.com/alelievr/libft-unit-test.git
```

Your folder structure should now look like this now:
```
.
|- libft/
|- libft-unit-tests/
```
