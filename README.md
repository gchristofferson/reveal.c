# Questions

## What's `stdint.h`?

stdint.h is a header file in the C standard library that specifically defines the bit lengths of the integers used, independent of the system specifications

## What's the point of using `uint8_t`, `uint32_t`, `int32_t`, and `uint16_t` in a program?

To ensure that these unsigned ints don't differ in size accross different architectures or compilers

## How many bytes is a `BYTE`, a `DWORD`, a `LONG`, and a `WORD`, respectively?

A 'BYTE' is 1 byte, a 'DWORD' is 4 bytes, a 'LONG' is 4 bytes and a 'WORD' is 2 bytes

## What (in ASCII, decimal, or hexadecimal) must the first two bytes of any BMP file be? Leading bytes used to identify file formats (with high probability) are generally called "magic numbers."

The file type; must be BM

## What's the difference between `bfSize` and `biSize`?

bfSize contains the total size of the file in bytes, including the pixels, the padding, and the headers while biSize contains the total size of the bitmap image in bytes, including pixels and padding.

## What does it mean if `biHeight` is negative?

If biHeight is negative, the bitmap is a top-down DIB and its origin is the upper-left corner.

## What field in `BITMAPINFOHEADER` specifies the BMP's color depth (i.e., bits per pixel)?

The biBitCount field of the BITMAPINFOHEADER structure determines the number of bits that define each pixel and the maximum number of colors in the bitmap.

## Why might `fopen` return `NULL` in lines 24 and 32 of `copy.c`?

The file may not exist or may be spelled incorrectly.

## Why is the third argument to `fread` always `1` in our code?

The third argument is the number of elements to read, so we will only be reading one element within the struct(file).

## What value does line 63 of `copy.c` assign to `padding` if `bi.biWidth` is `3`?

Line 63 will assign 0 to padding if bi.biwidth is 3.

## What does `fseek` do?

The fseek function will move the file position indicator within the file we're reading. To move the position within the file, it takes the file pointer that we're seeking over, the number of bytes to move the indicator, and then whether we're moving relative to the current position in the file, the beginning of the file, or the end.

## What is `SEEK_CUR`?

TODO
# reveal.c
