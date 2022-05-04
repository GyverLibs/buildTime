This is an automatic translation, may be incorrect in some places. See sources and examples!

#buildTime
Parsing and getting compile date and time from __DATE__ and __TIME__ constants

### Compatibility
Compatible with all Arduino platforms (using Arduino functions)

### Documentation
The library has [extended documentation](https://alexgyver.ru/buildTime/)

## Content
- [Install](#install)
- [Initialization](#init)
- [Usage](#usage)
- [Example](#example)
- [Versions](#versions)
- [Bugs and feedback](#feedback)

<a id="install"></a>
## Installation
- The library can be found by the name **buildTime** and installed through the library manager in:
    - Arduino IDE
    - Arduino IDE v2
    - PlatformIO
- [Download library](https://github.com/GyverLibs/buildTime/archive/refs/heads/main.zip) .zip archive for manual installation:
    - Unzip and put in *C:\Program Files (x86)\Arduino\libraries* (Windows x64)
    - Unzip and put in *C:\Program Files\Arduino\libraries* (Windows x32)
    - Unpack and put in *Documents/Arduino/libraries/*
    - (Arduino IDE) automatic installation from .zip: *Sketch/Include library/Add .ZIP library…* and specify the downloaded archive
- Read more detailed instructions for installing libraries [here] (https://alexgyver.ru/arduino-first/#%D0%A3%D1%81%D1%82%D0%B0%D0%BD%D0%BE% D0%B2%D0%BA%D0%B0_%D0%B1%D0%B8%D0%B1%D0%BB%D0%B8%D0%BE%D1%82%D0%B5%D0%BA)

<a id="init"></a>
## Initialization
Not

<a id="usage"></a>
## Usage
Compile time constants:
- `BUILD_YEAR` - year
- `BUILD_MONTH` - month
- `BUILD_DAY` - day
- `BUILD_HOUR` - hour
- `BUILD_MIN` - minute
- `BUILD_SEC` - second

<a id="example"></a>
## Example
```cpp
// test to get compilation time and date

#include "buildTime.h"
void setup() {
  Serial.begin(9600);
  Serial.println(__DATE__);
  Serial.println(__TIME__);
  Serial.println();
  
  Serial.print(BUILD_YEAR);
  serial print(" ");
  Serial.print(BUILD_MONTH);
  serial print(" ");
  Serial.println(BUILD_DAY);

  Serial.print(BUILD_HOUR);
  serial print(":");
  Serial.print(BUILD_MIN);
  serial print(":");
  Serial.println(BUILD_SEC);
}

void loop() {
}
```

<a id="versions"></a>
## Versions
- v1.0

<a id="feedback"></a>
## Bugs and feedback
When you find bugs, create an **Issue**, or better, immediately write to the mail [alex@alexgyver.ru](mailto:alex@alexgyver.ru)
The library is open for revision and your **Pull Request**'s!