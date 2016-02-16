//Write a blog over IO libraries. All Stream, reader, writer classes.
#  Console I/O
## System class
- in -> InputStream
- out -> PrintStream
- err -> PrintStream
- above stream classes to deal with stream of bytes.
- reader/writer classes to deal with stream of characters.

## BufferedReader
- preferred over FileReader/Scanner/InputStreamReader
- more efficient
```java
BufferedReader br = new BufferedReader(new InputStreamReader(System.in));
```

## PrintWriter
- preferred over System.out
```java
PrintWriter pw = new PrintWriter(Systm.out);
```
- PrintStream deals with byte encoding and is thus platform dependent. PrintWriter is more generic.

# File I/O
```java
FileInputStream(String fileName) throws FileNotFoundException
FileOutputStream(String fileName) throws FileNotFoundException
```
- Use try(resource-specification){ .. }
