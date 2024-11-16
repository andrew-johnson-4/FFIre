# FFIre
Quickly generate FFI bindings from any language to any language

LM is a typed macro assembler that can be used to generate code from templates. Here we have examples for Python to Rust or Node to C etc. 

Generating FFI Bindings can usually be broken down into logically distinct stages.
* extracting information from the low-level language
* defining the API for the high-level language
* generating the glue code

This project is structured to address these issues individually by
* providing common language parsers to extract symbol and type information from low-level languages
* providing simple macros to define the exported API to high-level languages
* uses the advanced LM type system to generate good glue code that allocates resources and frees resources correctly
