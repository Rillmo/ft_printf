# <img src="https://github.com/Rillmo/ft_printf/assets/51233626/da50795f-578f-4a4b-ba5c-04b60602421d" width="50"/>FT_PRINTF
>This is simple printf library for 42.

## Prerequisites
You'll need IDE for C to use this libaray.

## Before using
You can use this libaray just same as original ***printf()***.
```
int  ft_printf(const char *, ...);
```
This printf library provides only some of the real ***printf()***'s features.
Features provided are as follows.
- %c : Prints a single character.
- %s : Prints a string (as defined by the common C convention).
- %p : The void * pointer argument has to be printed in hexadecimal format.
- %d : Prints a decimal (base 10) number.
- %i : Prints an integer in base 10.
- %u : Prints an unsigned decimal (base 10) number.
- %x : Prints a number in hexadecimal (base 16) lowercase format.
- %X : Prints a number in hexadecimal (base 16) uppercase format.
- %% : Prints a percent sign.

Also ft_printf doesn't use buffer management of the original ***printf()***.
It means that you can use it just like ***write()***, which is system call.

## How to use
You just need to clone this repository and write Makefile commnad in your terminal.
1. Clone this repository in your local environment.
```
git clone https://github.com/Rillmo/ft_printf.git <your-dir>
```
2. Use Makefile command.
```
make
```
3, Now you can see ***libftprintf.a*** in your directory, then it's ready to use library.
  You can complie your C source code (*.c) with command below. 
```
cc -L./<your-dir> -lftprintf <your-c-source-codes>
```

## How to remove
1. If you want to remove object files, run this command.
```
make clean
```
2. If you want to remove object files, and also library file (***libftprintf.a***), run this command.
```
make fclean
```
