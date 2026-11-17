# Wrap-Up

#### Cheat Sheet:

- **Bit and Byte :**
    - a **Bit** is a single binary switch that holds either 1 or 0.
    - **Byte** is standard group of 8 bits. it can hold up-to 256 different values. (2^8 = 256)
- **The 2ⁿ rule (place values) :**
    - from right to left the values represent the increasing power of 2 (2ⁿ…..16 8 4 2 1).
    - when ever a 1 appears you sum the value.
    - Ex: `0011`→ 0 + 0 + 2 + 1 = 3
- **The "all 1s" rule ( 2ⁿ - 1 ) :**
    - a binary number of ***n*** consecutive 1 s is always **2ⁿ - 1**.
    - Ex: `1111`→ 2^4 -1 = 16 - 1 = 15.
- **The 4-bit hex table (0 to F):**
    - Every 4-bit nibble maps cleanly to one hexadecimal digit, where `0000`–`1001` are **0–9** and `1010`–`1111` are **A–F** (10–15).
        
        
        | Decimal | Binary (4 bits) | Hex |
        | --- | --- | --- |
        | 0 | `0000` | `0` |
        | 1 | `0001` | `1` |
        | 2 | `0010` | `2` |
        | 3 | `0011` | `3` |
        | 4 | `0100` | `4` |
        | 5 | `0101` | `5` |
        | 6 | `0110` | `6` |
        | 7 | `0111` | `7` |
        | 8 | `1000` | `8` |
        | 9 | `1001` | `9` |
        | 10 | `1010` | `A` |
        | 11 | `1011` | `B` |
        | 12 | `1100` | `C` |
        | 13 | `1101` | `D` |
        | 14 | `1110` | `E` |
        | 15 | `1111` | `F` |
- **The octal 4-2-1 trick:**
    - Linux file permissions use three bits per role (**4** = read, **2** = write, **1** = execute).
    - add together to get digits like :
        - `7` (`4+2+1` = full access).
        - `5` (`4+0+1` = read/execute).
- **The ASCII anchors:**
    - You can find any alphanumeric character's decimal code by counting up from three base anchors:
        - **'0' = 48**
        - **'A' = 65**
        - **'a' = 97**
- **Signed vs. unsigned:**
    - **Unsigned** integers use all bits for positive magnitude (0 to 255 for a byte).
    - **signed** integers reserve the leftmost bit for the sign (-128 to +127 in two's complement).
- **Overflow:**
    - Overflow happens when an arithmetic result exceeds the maximum or minimum value a fixed number of bits can hold, causing the number to wrap around unexpectedly.
- **RGB colors:**
    - A standard color pixel uses **3 bytes (24 bits)**
    - one byte each for Red, Green, and Blue (0–255)
    - combining to create 256³ or about **16.7 million** colors.
- **Unicode / UTF-8:**
    - UTF-8 is a variable-width encoding that uses **1 to 4 bytes per character** to represent over a million global symbols and emojis while keeping standard 1-byte ASCII backward-compatible.

#### Secret message :

- The secret message **RADHE** converts to **40 bits** (5 bytes) of ASCII data. Each uppercase letter is encoded using the standard `'A' = 65` anchor.
    
    
    | **Letter** | **ASCII Decimal** | **8-Bit Binary** | **Hex** |
    | --- | --- | --- | --- |
    | **R** | 82 | `01010010` | `52` |
    | **A** | 65 | `01000001` | `41` |
    | **D** | 68 | `01000100` | `44` |
    | **H** | 72 | `01001000` | `48` |
    | **E** | 69 | `01000101` | `45` |
- full Binary Message :
    
    `01010010 01000001 01000100 01001000 01000101`
    

### Your week at a glance

Everything you did was one idea, built up step by step: **a computer only has switches, and clever agreements turn those switches into everything we see.**

| Lesson | What you learned | Your one-line takeaway |
| --- | --- | --- |
| 1. Why 0 and 1 | Computers use ON/OFF switches because they’re simple, fast, and hard to get wrong | Your cars-and-bulbs idea: n bulbs give 2ⁿ outcomes |
| 2. Bits and bytes | 1 bit = 1 switch, 1 byte = 8 bits, and the size ladder KB → MB → GB → TB | Your ringtone was 470 KB, your photo 189 KB |
| 3. Counting in binary | Place values 1, 2, 4, 8, 16... and counting 0 to 31 | Your 32-row table had zero errors |
| 4. Binary to decimal | Add the place values of the ON bulbs | All 1s = one less than a power of two |
| 5. Decimal to binary | Biggest-coin method and the keep-halving method | 255 = `11111111`, the biggest byte |
| 6. Hexadecimal | One hex digit = 4 bits, which gives short, readable bytes | FF = 255, and colors like `#40da33` |
| 7. Octal | One octal digit = 3 bits, and 4-2-1 gives Linux permissions | 755 = `rwxr-xr-x` |
| 8. ASCII and Unicode | Letters are stored as agreed numbers (A = 65, a = 97) | “5” is the symbol 53, while 5 is the amount |
| 9. Colors, pictures, sound | A pixel is 3 bytes (RGB), a picture is a grid of pixels, sound is many measurements per second | Your color was (64, 218, 51), a bright green |
| 10. Negative numbers and overflow | Two’s complement, signed vs unsigned, and wraparound | 127 + 1 can become −128, a real security risk |