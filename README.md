# LightLog
LL is a lightweight and simple yet useful logging c++ library

## Usage example
```c++
    Log::SetLogLevel(LogLevel::Full); // decide what logs will be outputted 
    Log::InitStdOutHandle();          // initialize std output for colored output
    Log::SetTitle("Power VM");        // set console title
```
or, for dlls:
```c++
    Log::SetLogLevel(LogLevel::Full);        // decide what logs will be outputted 
    Log::InitStdOutHandle();                 // initialize std output for colored output
    Log::AllocConsoleWithTitle("Power VM"); // allocate console & set console title (for dlls)
```
