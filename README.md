# Huffman Text File Encoder and Decoder

This project provides the implementation of Huffman coding for compressing and decompressing text files.

## Files

- `encode.cpp`: Contains the logic for encoding a text file using Huffman coding.
- `decode.cpp`: Contains the logic for decoding a compressed file back to the original text file.
- `huffman.cpp`: Contains the Huffman tree and related utilities used in both encoding and decoding.
- `huffman.hpp`: Header file for `huffman.cpp`.

## Prerequisites

Ensure you have a C++ compiler installed (e.g., `g++`).

## Compilation Instructions

To compile the encoder and decoder, use the following commands:

### Encoder

```sh
g++ encode.cpp huffman.cpp -o encode
```

### Decoder

```sh
g++ decode.cpp huffman.cpp -o decode
```

## Usage

### Encoding a file

To use the encoder, run the following command:

```sh
./encode inputFile.txt compressed.huf
```

This will create a compressed file named `compressed.huf` in the current directory.

- `inputFile.txt`: The input text file you want to compress.
- `compressed.huf`: The output compressed file.

### Decoding a File

To use the decoder, run the following command:

```sh
./decode compressed.huf outputFile.txt
```

This will create a decompressed file named `outputFile.txt` in the current directory.

- `compressed.huf`: The input compressed file.
- `outputFile.txt`: The output text file that will contain the decompressed content.
