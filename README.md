# a85
Simple Ascii85 encoder/decoder functions written in C++.

Ascii85 is a binary-to-text encoding protocol that can acheive 80% efficiency.
For more info, [see Wikipedia](https://en.wikipedia.org/wiki/Ascii85).

## Usage
The two main functions:

```c++
// Translates the given binary data of the given size to ascii85.
// Can translate in-place.
// Optionally appends a null character.
void a85::to_a85(const u8* data, int binlen, char* text, bool append_null = false);

// Translates the given Ascii85 text to binary data.
// Can translate in-place.
void a85::from_a85(const char* text, int textlen, u8* data);
```

## License
Copy as you please. No attribution necessary.
