This is an automatic translation, may be incorrect in some places. See sources and examples!

# Buildtime
Parsing and receiving the date and time of compilation from constant __date__ and __time__

## compatibility
Compatible with all arduino platforms (used arduino functions)

### Documentation
There is [extended documentation] to the library (https://alexgyver.ru/buildtime/)

## Content
- [installation] (# Install)
- [initialization] (#init)
- [use] (#usage)
- [Example] (# Example)
- [versions] (#varsions)
- [bugs and feedback] (#fedback)

<a id="install"> </a>
## Installation
- The library can be found by the name ** Buildtime ** and installed through the library manager in:
    - Arduino ide
    - Arduino ide v2
    - Platformio
- [download the library] (https://github.com/gyverlibs/buildtime/archive/refs/heads/main.zip). Zip archive for manual installation:
    - unpack and put in * C: \ Program Files (X86) \ Arduino \ Libraries * (Windows X64)
    - unpack and put in * C: \ Program Files \ Arduino \ Libraries * (Windows X32)
    - unpack and put in *documents/arduino/libraries/ *
    - (Arduino id) Automatic installation from. Zip: * sketch/connect the library/add .Zip library ... * and specify downloaded archive
- Read more detailed instructions for installing libraries [here] (https://alexgyver.ru/arduino-first/#%D0%A3%D1%81%D1%82%D0%B0%BD%D0%BE%BE%BE%BED0%B2%D0%BA%D0%B0_%D0%B1%D0%B8%D0%B1%D0%BB%D0%B8%D0%BE%D1%82%D0%B5%D0%BA)
### Update
- I recommend always updating the library: errors and bugs are corrected in the new versions, as well as optimization and new features are added
- through the IDE library manager: find the library how to install and click "update"
- Manually: ** remove the folder with the old version **, and then put a new one in its place.“Replacement” cannot be done: sometimes in new versions, files that remain when replacing are deleted and can lead to errors!


<a id="init"> </a>
## initialization
No

<a id="usage"> </a>
## Usage
Construction Constants:
- `Build_year` - year
- `Build_Month` - Month
- `Build_Day` - Day
- `Build_hour` - Hour
- `Build_min` - Minute
- `Build_Sec` - Second

<a id="EXAMPLE"> </a>
## Example
`` `CPP
// Test for receiving the time and dates of compilation

#include "Buildtime.h"
VOID setup () {
  Serial.Begin (9600);
  Serial.println (__ Date__);
  Serial.println (__ time__);
  Serial.println ();
  
  Serial.print (Build_year);
  Serial.print ("");
  Serial.print (Build_Month);
  Serial.print ("");
  Serial.println (Build_Day);

  Serial.print (Build_hour);
  Serial.print (":");
  Serial.print (Build_min);
  Serial.print (":");
  Serial.println (Build_Sec);
}

VOID loop () {
}
`` `

<a id="versions"> </a>
## versions
- V1.0

<a id="feedback"> </a>
## bugs and feedback
Create ** Issue ** when you find the bugs, and better immediately write to the mail [alex@alexgyver.ru] (mailto: alex@alexgyver.ru)
The library is open for refinement and your ** pull Request ** 'ow!


When reporting about bugs or incorrect work of the library, it is necessary to indicate:
- The version of the library
- What is MK used
- SDK version (for ESP)
- version of Arduino ide
- whether the built -in examples work correctly, in which the functions and designs are used, leading to a bug in your code
- what code has been loaded, what work was expected from it and how it works in reality
- INideal to attach the minimum code in which the bug is observed.Not a canvas of a thousand lines, but a minimum code