# LightLog
LL is a lightweight and simple yet useful logging c++ library

## Usage example
```c++
    Log::SetLogLevel(LogLevel::Full); // decide what logs will be outputted 
    Log::InitStdOutHandle();          // initialize std output for colored output
    Log::SetTitle("LightLog");        // set console title
```
or, for dlls:
```c++
    Log::SetLogLevel(LogLevel::Full);        // decide what logs will be outputted 
    Log::InitStdOutHandle();                 // initialize std output for colored output
    Log::AllocConsoleWithTitle("LightLog"); // allocate console & set console title (for dlls)
```
