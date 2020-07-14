This is a x86 Linux command line tool for converting ihex files to bin files.

For doing microbootloader mode recovery, the data contained in an ihex files
is used. This tool parses the data in an ihex file and saves it in a bin file.

To use this tool, copy it to a Linux PC, change its access permission settings
to make it executable, and run the command below from terminal
./ihex2bin name_of_ihex_file

The output is a binary file named name_of_hex_file.bin stored in the same
directory as the tool. The binary file can be used for building into the kernel
image for doing automatic microbootloader mode recovery during system power-on.
