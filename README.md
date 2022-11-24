# LightLog
LL is a lightweight and simple yet useful logging c++ library

## Usage example
### Initialization
```c++
    Log::SetLogLevel(LogLevel::Full); // decide what logs will be outputted 
    Log::InitStdOutHandle();          // initialize std output for colored output (ignore for normal colors)
    Log::SetTitle("LightLog");        // set console title
```
or, for dlls:
```c++
    Log::SetLogLevel(LogLevel::Full);        // decide what logs will be outputted 
    Log::InitStdOutHandle();                 // initialize std output for colored output (ignore for normal colors)
    Log::AllocConsoleWithTitle("LightLog");  // allocate console & set console title (for dlls)
```
### Output
```c++
    Log::Ok("(%i) Ok!", 1);
    Log::Info("(%i) Info...", 2);
    Log::Warn("(%i) Warn", 3);
    Log::Err("(%i) Error!", 4);
```
### Using xor helpers for output
(xor is automatically used, if not imported it will simply not xor)
```c++
    __Ok("(%i) Ok!", 1);
    __Info("(%i) Info...", 2);
    __Warn("(%i) Warn", 3);
    __Err("(%i) Error!", 4);
```
