# testrst
### Instructions Groups
#### - Data Movement Instructions
 **Example**:
        ```
        mov ax, bx  ; move data from bx to ax
        ```
     ```
     lda 897        ; load 897 into accumulator 
     ```
#### - Arithmetic/Logical Instructions
 **Example**:
 ```
 and ax, 124  ; AND 123 with ax
 add ax, 44   ; ADD 44 to ax
 add bx, [685] ; ADD data at address 685 to bx
 ```

#### - Program Control Instructions
**Example:**
```
cmp ax, 0   ; compare ax with zero
jne 1234    ; jump if not equal
            ; to the instruction at address 1234
//if ax is not equal to zero then jump to instruction at address at 1234
```
#### - Special Instructions
**Example:**
```
cli    ; clear the interrupt flag
sti    ; set the interrupt flag
```



## IAPX 8080 Registers [16 bit]

 ##### 1 General Purpose Registers
 - AX  AH, AL
 - BX  BH, BL
 - CX  CH, CL
 - DX  DH, DL

|AH|AL|
|-|-|
Each AH and AL are 8 bit in size

|Register|Description|
|-|-|
|AX| Accumulator Register(Mathematical and logical Operations). 8/16/32/64bit processor means size of accumulator 
|BX|Base Register
|CX| Counter Register
|DX| Destination Register


 #### 2. Index/Base/Pointer Registers
Holds the address of operands

 - SI  (Source Index)
 - DI  (DEstination Index)
 - IP (Instruction Pointer)
 - SP (Stack Pointer)
 - BP (Base Pointer)

  #### 3. Flag Register

Collection of different boolean information. Each bit has its independent meaning.

   | -  |  - | -  | -  |  O | D | I | T  |  S | Z  | - |A  | - | P  |-|C|
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|

|Bit Name|Description|
|-|-|
|C|Counter
|P|Parity
|A|Auxiliary carry
|Z| Zero bit
|S|Sign bit
|T| Trap flag
|I|Interrupt flag
|D|Direction flag (0 means from lower to higher and 1 means higher to lower)|
|O|Overflow flag

#### 4. Segment Registers
 - CS (Code Segment)
 - DS (Data Segment)
 - SS (Stack Segment)
 - ES (Extra Segment)


