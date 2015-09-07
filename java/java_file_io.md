# Java File I/O
* Most of the stuff is available in java.io package.

## Stream
* A sequence of data elements made available *over time*.
* Two kinds of streams: *Byte*Streams and *Character*Streams.

### Byte Streams
* Byte streams can be read in 8 bit units.
* Name of classes using this stream generally ends in "-Stream"
* Eg. FileInputStream, FileOutputStream

### Character Streams
* Are read in 16 bit units.
* Provide support for unicode characters.
* Name classes using this stream ends in "-reader/writer"
* Built on top of Byte Streams.
* Eg. FileReader, FileWriter

## Usage
* Basically the same for both streams:
1. Declare the class that you want to use:
    ```java
    FileReader in = null;
    ```
2. Instantiate it:
    ```java
    in = new FileReader("input.txt");
    ```
3. Use it:
    ```java
    int c = in.read(); // returns -1 on end of file
    ```


# Reference
http://www.tutorialspoint.com/java/java_files_io.htm