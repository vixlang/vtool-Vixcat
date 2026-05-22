# vixcat

A simple file viewer (like `cat`) written in the [Vix programming language](https://github.com/vixlang).  
It reads a file given as a command-line argument and prints its content to standard output.

## Repository

[https://github.com/vixlang/vixcat](https://github.com/vixlang/vixcat)

## Usage

```
vixcat <filename>
```

Example:

```
vixcat hello.txt
```

If no filename is provided, the program prints:

```
Usage: vixcat <filename>
```

## Building

Ensure you have a working Vix compiler (`vixc`) installed.  
Compile the source file `vixcat.vix` to an executable:

```
vixc vixcat.vix -o vixcat
```

The program uses `extern "C"` to call C standard library functions (`fopen`, `fread`, `printf`, `malloc`, `free`, etc.).  
Your Vix runtime must support linking against the system’s C library. No additional dependencies are required.

## License

Copyright 2026 The Vixcat Contributors

Licensed under the Apache License, Version 2.0 (the "License");  
you may not use this file except in compliance with the License.  
You may obtain a copy of the License at

[http://www.apache.org/licenses/LICENSE-2.0](http://www.apache.org/licenses/LICENSE-2.0)

Unless required by applicable law or agreed to in writing, software  
distributed under the License is distributed on an "AS IS" BASIS,  
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.  
See the License for the specific language governing permissions and  
limitations under the License.
