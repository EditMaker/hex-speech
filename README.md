# Hex-Speech

A natural spoken and written language for hexadecimal numbers that makes hexadecimal values speakable in conversation.

## Overview

Hex-Speech transforms complex hexadecimal notation into natural spoken or written language.

**Example:**
- Hex: `FAD,1022` 
- Hex-Speech: "F duhex A hex D sec 1, 1 trihex and 2 hex 2"

## Language Structure Rules

The rules for this language are simple, they are actually more simple than English decimal.

### Digit position in section markers
- **base:** `0001` would be written as just "1"
- **hex:** `0010` would be written as "1 hex" meaning 1 * 16 <sup>1</sup> decimal
- **duhex:** `0100` would be written as "1 duhex" meaning 1 * 16<sup>2</sup> decimal
- **trihex:** `1000` would be written as "1 trihex" meaning 1 * 16<sup>3</sup> decimal
- **and:** If there is a zero gap between nonzero digits in a section you may optionally include "and" such as `1001` being "1 trihex and 1"

### Section Values as Names
- In Hex-Speech sections are divided into sections of 4 digits (16 bits) unlike English decimal digits which are divided after 3.
- You do not say the base section. **Example:** `AF24` is "A trihex F duhex 2 hex 4"
- When there are two or more sections you state the section name as "sec" then its number counting up from the base section which is left unstated as 0. **Example:** `A,000F,AF24` is "A sec 2, F sec 1, A trihex F duhex 2 hex 4"

### Hexadecimal points
- Number units after "hexadecimal points" or "hex points" can also be divided into sections but may also be listed. Hex point sections use "minus" before section number `1.1000,01` is "1, 1 sec minus 1, 1 duhex sec minus 2" however listing digits the same as English decimal is preferred.

## Notes Beyond Language
I think if someone wants to intuitively learn hex they should learn "landmarks" such as 0.8 being half, 0.4 being a quarter, 20 being decimal 2*16 and so on.
Try it. Share it. Fork it. I find it is a great way to learn hex use.
