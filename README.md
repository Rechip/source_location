# source_location
GCC and Clang compilers supported functionality needed for <source_location> header for a long long time, they just missed a proper header file. MSVC bundled header file just a few versions after the compiler support. If you happen to be a person using compiler supporting the functionality but with no bundled header file, this header is just for you.


## Target audience of this header

Of course the library will work also with a newer compilers

| compiler | since | until
| -------- | ----- | -----
| GCC      | 7.1   | 11.0
| Clang    | 9.0.0 | 12.0.1
| MSVC     | 19.26 | 19.29

## Compilers with <source_location> bundled

| compiler | version | bundled
| -------- | ------- | -------
| GCC      | 10.3    | no
|          | 11.0    | yes 
| Clang    | 12.0.0  | no
|          | 12.0.1  | yes
| MSVC     | 19.28   | no
|          | 19.29   | yes

## Compilers with required functionality, but no header

| compiler | version | functionality
| -------- | ------- | -------------
| GCC      | 4.7.4   | no
|          | 4.8.1   | limited (line is not constexpr, column is not supported)
|          | 7.1     | almost (column not supported)
| Clang    | 8.0.1   | no
|          | 9.0.0   | yes
| MSVC     | 19.25   | no
|          | 19.26   | yes
