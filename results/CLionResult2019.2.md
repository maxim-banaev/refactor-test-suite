# CLion

Home: [CLion](https://www.jetbrains.com/clion/)

Version: CL-192.5118.29

Notes:

Methodology: Default suggestions are selected when refactoring.  Some
refactorings can be performed successfully if suggestions are excluded.

**Add Block Delimiter** is performed by selecting the code and performing
Code / Surround With... / {}.

**Add Parameter** is performed with **Change Signature**.

**Create Setter Method** is performed with Code / Generate... / Setter.

**Flatten Conditional** is performed by repeatedly applying the fixup Merge
Nested Ifs.

**Replace If With Ternary** is performed by applying the fixup Replace
'if else' with '?:'.

**Replace Ternary With If** is performed by applying the fixup Replace
'?;' with 'if else'.

**Reorder Parameters** is performed with **Change Signature**.

**Reverse Conditional** is performed with Invert Condition

<hr/>

## Add Block Delimiter
Case | Result
---- | ------
ABD1 |  Pass
ABD2 |  Pass
ABD3 |  Pass
ABD4 |  Pass
ABD5 |  Pass
ABD6 |  Pass
ABD7 |  Pass

## Add Override
Case | Result
---- | ------
AO1  | Pass
AO2  | Pass
AO3  | Pass
AO4  | Pass
AO5  | Pass

## Add Parameter
Case | Result
---- | ------
AP01 | Pass
AP1  | Pass
AP2  | Pass
AP3  | Pass
AP4  | Pass
AP5  | Pass
AP6  | Pass
AP7  | Pass
AP8  | Pass
AP9  | Pass
AP10 | Pass
AP11 | Pass
AP12 | Pass
AP13 | Pass
AP14 | Pass
AP15 | Pass
AP16 | Pass
AP17 | Pass
AP18 | Pass
AP19 | Pass
AP20 | Pass
AP21 | Pass
AP22 | Pass
AP23 | Pass
AP24 | Failure (doesn't update other template arguments) [CPP-16560](https://youtrack.jetbrains.com/issue/CPP-16560)
AP25 | Failure (doesn't detect function, method or block) [CPP-16560](https://youtrack.jetbrains.com/issue/CPP-16560)

## Change Signature
Case | Result
---- | ------
CS1  |  Pass
CS2  |  Pass
CS3  |  Pass
CS4  |  Pass
CS5  |  Pass
CS6  |  Pass
CS7  |  Pass
CS8  |  Pass
CS9  |  Pass
CS10 |  Pass
CS11 |  Pass

## Create Declaration From Implementation

## Create Implementation From Declaration

## Create Method Stub
Case  | Result
----- | ------
CMS1  | Pass
CMS2  | Pass
CMS3  | Pass
CMS4  | Failure [CPP-1601](https://youtrack.jetbrains.com/issue/CPP-1601)
CMS5  | Failure [CPP-1601](https://youtrack.jetbrains.com/issue/CPP-1601)
CMS6  | Pass
CMS7  | Pass
CMS8  | Failure (not available) [CPP-1908](https://youtrack.jetbrains.com/issue/CPP-1908)
CMS9  | Failure (not available) [CPP-1908](https://youtrack.jetbrains.com/issue/CPP-1908)
CMS10 | Failure (not available) [CPP-1908](https://youtrack.jetbrains.com/issue/CPP-1908)
CMS11 | Pass
CMS12 | Pass
CMS13 | Pass
CMS14 | Pass
CMS15 | Pass
CMS16 | Pass
CMS17 | Pass
CMS18 | Pass
CMS19 | Pass
CMS20 | Pass
CMS21 | Pass
CMS22 | Pass

## Create Multi Variable Declaration (not available)

## Create Setter Method
Case  | Result
----- | ------
CSM1  | Pass
CSM2  | Pass
CSM3  | Pass
CSM4  | Pass
CSM5  | Pass
CSM6  | Pass
CSM7  | Pass
CSM8  | Pass
CSM9  | Pass
CSM10 | Pass
CSM11 | Pass
CSM12 | Pass
CSM13 | Pass
CSM14 | Pass
CSM15 | Pass
CSM16 | Pass
CSM17 | Pass
CSM18 | Pass
CSM19 | Pass
CSM20 | Pass
CSM21 | Pass
CSM22 | Pass
CSM23 | Pass
CSM24 | Pass
CSM25 | Pass
CSM26 | Pass
CSM27 | Pass
CSM28 | Pass
CSM29 | Failure (not available)
CSM30 | Pass
CSM31 | Pass

## Extract Constant
Case | Result
---- | ------
EC1  | Pass
EC2  | Pass
EC3  | Pass
EC4  | Pass
EC5  | Failure [CPP-1928](https://youtrack.jetbrains.com/issue/CPP-1928)
EC6  | Pass
EC7  | Failure [CPP-1929](https://youtrack.jetbrains.com/issue/CPP-1929), [CPP-1930](https://youtrack.jetbrains.com/issue/CPP-1930)
EC8  | Pass
EC9  | Failure [CPP-1928](https://youtrack.jetbrains.com/issue/CPP-1928)
EC10 | Pass
EC11 | Failure [CPP-1929](https://youtrack.jetbrains.com/issue/CPP-1929), [CPP-1930](https://youtrack.jetbrains.com/issue/CPP-1930)
EC12 | Pass
EC13 | Pass

## Extract Declaration

## Extract Define

## Extract Function
Case | Result
---- | ------
EXF1  | Pass
EXF2  | Pass
EXF3  | Pass
EXF4  | Pass
EXF5  | Pass
EXF6  | Pass
EXF7  | Pass
EXF8  | Pass
EXF9  | Pass
EXF10 | Pass
EXF11 | Pass
EXF12 | Pass
EXF13 | Pass
EXF14 | Failure [CPP-1915](https://youtrack.jetbrains.com/issue/CPP-1915)
EXF15 | Failure [CPP-1915](https://youtrack.jetbrains.com/issue/CPP-1915)
EXF16 | Failure [CPP-1915](https://youtrack.jetbrains.com/issue/CPP-1915)
EXF17 | Failure [CPP-1915](https://youtrack.jetbrains.com/issue/CPP-1915)
EXF18 | Failure [CPP-1916](https://youtrack.jetbrains.com/issue/CPP-1916)
EXF19 | Pass

## Extract Variable
Case | Result
---- | ------
EXV1 | Failure [CPP-1931](https://youtrack.jetbrains.com/issue/CPP-1931)
EXV2 | Pass
EXV3 | Pass
EXV4 | Pass
EXV5 | Pass
EXV6 | Failure [CPP-1932](https://youtrack.jetbrains.com/issue/CPP-1932)

## Extract Method
Case | Result
---- | ------
EM1  | Pass
EM2  | Failure [CPP-1917](https://youtrack.jetbrains.com/issue/CPP-1917)
EM3  | Failure [CPP-1917](https://youtrack.jetbrains.com/issue/CPP-1917)
EM4  | Failure [CPP-1917](https://youtrack.jetbrains.com/issue/CPP-1917)
EM5  | Failure [CPP-1917](https://youtrack.jetbrains.com/issue/CPP-1917)
EM6  | Failure [CPP-1917](https://youtrack.jetbrains.com/issue/CPP-1917)
EM7  | Pass
EM8  | Failure [CPP-1917](https://youtrack.jetbrains.com/issue/CPP-1917)
EM9  | Failure [CPP-1917](https://youtrack.jetbrains.com/issue/CPP-1917)
EM10 | Failure [CPP-1917](https://youtrack.jetbrains.com/issue/CPP-1917)
EM11 | Failure [CPP-1917](https://youtrack.jetbrains.com/issue/CPP-1917)
EM12 | Failure [CPP-1917](https://youtrack.jetbrains.com/issue/CPP-1917)
EM13 | Failure [CPP-1918](https://youtrack.jetbrains.com/issue/CPP-1918)
EM14 | Pass
EM15 | Failure [CPP-1919](https://youtrack.jetbrains.com/issue/CPP-1919)
EM16 | Failure [CPP-1919](https://youtrack.jetbrains.com/issue/CPP-1919)
EM17 | Failure [CPP-1919](https://youtrack.jetbrains.com/issue/CPP-1919)
EM18 | Failure [CPP-1919](https://youtrack.jetbrains.com/issue/CPP-1919)
EM19 | Pass
EM20 | Failure [CPP-1917](https://youtrack.jetbrains.com/issue/CPP-1917)

## Extract Parameter
Case | Result
---- | ------
EP1  | Failure [CPP-1920](https://youtrack.jetbrains.com/issue/CPP-1920)
EP2  | Failure [CPP-16582](https://youtrack.jetbrains.com/issue/CPP-16582)
EP3  | Failure (should not be available) [CPP-1921](https://youtrack.jetbrains.com/issue/CPP-1921)
EP4  | Pass
EP5  | Failure [CPP-1920](https://youtrack.jetbrains.com/issue/CPP-1920)
EP6  | Pass

## Extract Typedef

## Flatten Conditional
Case | Result
---- | ------
FC1  | Pass

## Inline Constant

## Inline Function

## Inline Macro
Case | Result
---- | ------
IM1  | Failure [CPP-1922](https://youtrack.jetbrains.com/issue/CPP-1922)
IM2  | Pass
IM3  | Pass
IM4  | Pass
IM5  | Pass
IM6  | Pass

## Inline Method

## Inline Recent Assignment
Case | Result
---- | ------
IRA1 | Failure (not available) [CPP-1923](https://youtrack.jetbrains.com/issue/CPP-1923)
IRA2 | Failure (not available) [CPP-1923](https://youtrack.jetbrains.com/issue/CPP-1923)

## Inline Result
Case | Result
---- | ------
IR1  | Failure [CPP-1924](https://youtrack.jetbrains.com/issue/CPP-1924)
IR2  | Failure [CPP-1924](https://youtrack.jetbrains.com/issue/CPP-1924)
IR3  | Failure [CPP-1924](https://youtrack.jetbrains.com/issue/CPP-1924)
IR4  | Failure [CPP-1924](https://youtrack.jetbrains.com/issue/CPP-1924)
IR5  | Failure [CPP-1924](https://youtrack.jetbrains.com/issue/CPP-1924)

## Inline Typedef

## Inline Variable
Case | Result
---- | ------
IV1  | Pass
IV2  | Failure (not available) [CPP-1925](https://youtrack.jetbrains.com/issue/CPP-1925)
IV3  | Pass
IV4  | Failure (not available) [CPP-1925](https://youtrack.jetbrains.com/issue/CPP-1925)
IV5  | Failure (not available) [CPP-1925](https://youtrack.jetbrains.com/issue/CPP-1925)
IV6  | Failure (not available) [CPP-1925](https://youtrack.jetbrains.com/issue/CPP-1925)
IV7  | Failure (not available) [CPP-1925](https://youtrack.jetbrains.com/issue/CPP-1925)
IV8  | Failure (not available) [CPP-1925](https://youtrack.jetbrains.com/issue/CPP-1925)
IV9  | Failure (not available) [CPP-1925](https://youtrack.jetbrains.com/issue/CPP-1925)
IV10 | Failure (not available) [CPP-1925](https://youtrack.jetbrains.com/issue/CPP-1925)
IV11 | Failure (not available) [CPP-1925](https://youtrack.jetbrains.com/issue/CPP-1925)
IV12 | Failure (not available) [CPP-2252](https://youtrack.jetbrains.com/issue/CPP-2252)

## Move Method
Case | Result
---- | ------
MM1   | Pass
MM2   | Pass
MM3   | Pass
MM4   | Pass
MM5   | Pass
MM6   | Failure [CPP-1933](https://youtrack.jetbrains.com/issue/CPP-1933)
MM7   | Failure [CPP-1933](https://youtrack.jetbrains.com/issue/CPP-1933)
MM8   | Failure [CPP-1933](https://youtrack.jetbrains.com/issue/CPP-1933)
MM9   | Pass
MM10  | Failure [CPP-1933](https://youtrack.jetbrains.com/issue/CPP-1933)
MM11  | Failure [CPP-1933](https://youtrack.jetbrains.com/issue/CPP-1933)
MM12  | Failure [CPP-1933](https://youtrack.jetbrains.com/issue/CPP-1933)
MM13  | Pass
MM14  | Failure [CPP-1933](https://youtrack.jetbrains.com/issue/CPP-1933)
MM15  | Pass
MM16  | Pass
MM17  | Pass
MM18  | Pass
MM19  | Pass
MM20  | Pass
MM21  | Pass
MM22  | Pass
MM23  | Failure [CPP-1933](https://youtrack.jetbrains.com/issue/CPP-1933)
MM24  | Failure [CPP-1933](https://youtrack.jetbrains.com/issue/CPP-1933)
MM25  | Failure [CPP-1933](https://youtrack.jetbrains.com/issue/CPP-1933)
MM26  | Failure [CPP-1933](https://youtrack.jetbrains.com/issue/CPP-1933)
MM27  | Failure [CPP-1933](https://youtrack.jetbrains.com/issue/CPP-1933)
MM28  | Failure [CPP-1933](https://youtrack.jetbrains.com/issue/CPP-1933)
MM29  | Failure [CPP-1933](https://youtrack.jetbrains.com/issue/CPP-1933)
MM30  | Failure [CPP-1933](https://youtrack.jetbrains.com/issue/CPP-1933)
MM31  | Pass
MM32  | Pass
MM33  | Failure [CPP-16587](https://youtrack.jetbrains.com/issue/CPP-16587)
MM34  | Failure [CPP-16587](https://youtrack.jetbrains.com/issue/CPP-16587)
MM35  | Failure [CPP-1936](https://youtrack.jetbrains.com/issue/CPP-1936)
MM36  | Pass

## Move Implementation to Source File
Case   | Result
------ | ------
MISF1  | Pass
MISF2  | Pass
MISF3  | Pass
MISF4  | Pass
MISF5  | Pass
MISF6  | Pass
MISF7  | Pass
MISF8  | Pass
MISF9  | Pass
MISF10 | Pass
MISF11 | Pass
MISF12 | Pass
MISF13 | Pass
MISF14 | Pass
MISF15 | Pass
MISF16 | Failed
MISF17 | Pass
MISF18 | Pass
MISF19 | Pass
MISF20 | Pass
MISF21 | Pass
MISF22 | Pass
MISF23 | Pass
MISF24 | Pass
MISF25 | Pass
MISF26 | Failed

## Pull Members Up

## Push Members Down

## Remove Block Delimiter (Not available)
Case | Result
---- | ------
RBD1 | Failure (not available)
RBD2 | Failure (not available)
RBD3 | Pass
RBD4 | Failure (not available)
RBD5 | Failure (not available)
RBD6 | Failure (not available)
RBD7 | Pass
RBD8 | Pass

## Remove Unused Parameter
Case | Result
---- | ------
RUP1 | Pass
RUP2 | Pass
RUP3 | Pass
RUP4 | Failed [CPP-16644](https://youtrack.jetbrains.com/issue/CPP-16644)

## Rename
Case | Result
---- | ------
R1    | Failure [CPP-1938](https://youtrack.jetbrains.com/issue/CPP-1938)
R2    | Failure [CPP-1938](https://youtrack.jetbrains.com/issue/CPP-1938)
R3    | Failure [CPP-1938](https://youtrack.jetbrains.com/issue/CPP-1938)
R4    | Pass
R5    | Pass
R6    | Pass
R7    | Failure [CPP-1939](https://youtrack.jetbrains.com/issue/CPP-1939)
R8    | Failure [CPP-1939](https://youtrack.jetbrains.com/issue/CPP-1939)
R9    | Pass
R10   | Pass
R11   | Pass
R12   | Failure (not available) [CPP-1940](https://youtrack.jetbrains.com/issue/CPP-1940)
R13   | Pass
R14   | Pass
R15   | Failure [CPP-1939](https://youtrack.jetbrains.com/issue/CPP-1939)
R16   | Pass
R17   | Pass
R18   | Pass
R19   | Failure [CPP-1939](https://youtrack.jetbrains.com/issue/CPP-1939)
R20   | Pass
R21   | Pass
R22   | Pass
R23   | Pass
R24   | Pass
R25   | Pass
R26   | Pass
R27   | Pass
R28   | Pass
R29   | Pass
R30   | Pass
R31   | Pass
R32   | Failure [CPP-1939](https://youtrack.jetbrains.com/issue/CPP-1939)
R33   | Failure [CPP-1938](https://youtrack.jetbrains.com/issue/CPP-1938)
R34   | Pass
R35   | Pass
R36   | Failure [CPP-1939](https://youtrack.jetbrains.com/issue/CPP-1939)
R37   | Pass
R38   | Pass
R39   | Pass
R40   | Pass
R41   | Pass
R42   | Pass
R43   | Pass (unrelated comments selected by default) [CPP-1942](https://youtrack.jetbrains.com/issue/CPP-1942)
R44   | Pass
R45   | Pass
R46   | Pass (unrelated comments selected by default) [CPP-1942](https://youtrack.jetbrains.com/issue/CPP-1942)
R47   | Pass
R48   | Pass
R49   | Pass (unrelated comments selected by default) [CPP-1942](https://youtrack.jetbrains.com/issue/CPP-1942)
R50   | Pass
R51   | Pass (unrelated comments selected by default) [CPP-1942](https://youtrack.jetbrains.com/issue/CPP-1942)
R52   | Pass
R53   | Pass (unrelated comments selected by default) [CPP-1942](https://youtrack.jetbrains.com/issue/CPP-1942)
R54   | Pass
R55   | Pass
R56   | Pass
R57   | Pass
R58   | Pass
R59   | Pass
R60   | Pass
R61   | Pass
R62   | Pass (unrelated comments selected by default) [CPP-1942](https://youtrack.jetbrains.com/issue/CPP-1942)
R63   | Pass
R64   | Pass
R65   | Pass (unrelated comments selected by default) [CPP-1942](https://youtrack.jetbrains.com/issue/CPP-1942)
R66   | Pass
R67   | Pass
R68   | Pass
R69   | Pass (unrelated comments selected by default) [CPP-1942](https://youtrack.jetbrains.com/issue/CPP-1942)
R70   | Pass (unrelated comments selected by default) [CPP-1942](https://youtrack.jetbrains.com/issue/CPP-1942)
R71   | Pass (unrelated comments selected by default) [CPP-1942](https://youtrack.jetbrains.com/issue/CPP-1942)
R72   | Pass (unrelated comments selected by default) [CPP-1942](https://youtrack.jetbrains.com/issue/CPP-1942)
R73   | Pass (unrelated comments selected by default) [CPP-1942](https://youtrack.jetbrains.com/issue/CPP-1942)
R74   | Failure (selects unrelated macro by default) [CPP-1943](https://youtrack.jetbrains.com/issue/CPP-1943)
R75   | Failure (selects unrelated macro by default) [CPP-1943](https://youtrack.jetbrains.com/issue/CPP-1943)
R76   | Failure (selects unrelated macro by default) [CPP-1943](https://youtrack.jetbrains.com/issue/CPP-1943)
R77   | Failure (selects unrelated macro by default) [CPP-1943](https://youtrack.jetbrains.com/issue/CPP-1943)
R78   | Failure (selects unrelated macro by default) [CPP-1943](https://youtrack.jetbrains.com/issue/CPP-1943)
R79   | Failure (selects unrelated macro by default) [CPP-1943](https://youtrack.jetbrains.com/issue/CPP-1943)
R80   | Failure (selects unrelated macro by default) [CPP-1943](https://youtrack.jetbrains.com/issue/CPP-1943)
R81   | Failure (selects unrelated macro by default) [CPP-1943](https://youtrack.jetbrains.com/issue/CPP-1943)
R82   | Pass
R83   | Pass
R84   | Pass
R85   | Pass
R86   | Pass
R87   | Pass
R88   | Pass
R89   | Pass
R90   | Pass
R91   | n/a
R92   | n/a
R93   | Pass
R94   | Pass
R95   | Pass
R96   | Pass
R97   | Pass
R98   | Failure [CPP-1941](https://youtrack.jetbrains.com/issue/CPP-1941)
R99   | Pass
R100  | Pass
R101  | Pass
R102  | Pass
R103  | Pass
R104  | Pass
R105  | Pass
R106  | Pass
R107  | Pass
R108  | Pass
R109  | Pass
R110  | Pass
R111  | Pass
R112  | Pass
R113  | Pass
R114  | Pass
R115  | Pass
R116  | Pass
R117  | Pass
R118  | Pass
R119  | Pass
R120  | Pass
R121  | Pass
R122  | Pass
R123  | Pass
R124  | Pass
R125  | Pass
R126  | Pass
R127  | Failed [CPP-16647](https://youtrack.jetbrains.com/issue/CPP-16647)
R128  | Pass
R129  | Pass
R130  | Pass
R131  | Pass
R132  | Pass
R133  | Pass
R134  | Pass
R135  | Pass
R136  | Pass
R137  | Pass
R138  | Failed [CPP-16647](https://youtrack.jetbrains.com/issue/CPP-16647)
R139  | Pass
R140  | Pass
R141  | Pass
R142  | Pass
R143  | Pass
R144  | Pass
R145  | Pass
R146  | Pass
R147  | Pass
R148  | Pass
R149  | Pass
R150  | Pass
R151  | Pass
R152  | Pass
R153  | Pass
R154  | Pass
R155  | Pass
R156  | Pass
R157  | Failed [CPP-16649](https://youtrack.jetbrains.com/issue/CPP-16649)
R158  | Failed [CPP-16649](https://youtrack.jetbrains.com/issue/CPP-16649)
R159  | Pass
R160  | Pass
R161  | Pass
R162  | Failed [CPP-16649](https://youtrack.jetbrains.com/issue/CPP-16649)
R163  | Pass
R164  | Pass
R165  | Pass
R166  | Pass
R167  | Pass
R168  | Pass
R169  | Pass
R170  | Pass
R171  | Pass
R172  | Pass
R173  | Pass
R174  | Pass
R175  | Pass
R176  | Pass
R177  | Pass
R178  | Pass
R179  | Pass
R180  | Pass
R181  | Pass
R182  | Pass
R183  | Pass
R184  | Pass
R185  | Pass
R186  | Pass
R187  | Pass
R188  | Pass
R189  | Pass
R190  | Pass
R191  | Pass
R192  | Pass
R193  | Pass
R194  | Pass
R195  | Pass
R196  | Pass
R197  | Pass
R198  | Pass
R199  | Pass
R200  | Pass
R201  | Pass
R202  | Pass
R203  | Pass
R204  | Pass
R205  | Pass
R206  | Pass
R207  | Pass
R208  | Pass
R209  | Pass
R210  | Pass
R211  | Pass
R212  | Pass
R213  | Pass
R214  | Pass
R215  | Pass
R216  | Pass
R217  | Pass
R218  | Pass
R219  | Pass
R220  | Pass
R221  | Pass
R222  | Pass
R223  | Pass
R224  | Failed [CPP-16658](https://youtrack.jetbrains.com/issue/CPP-16658)
R225  | Pass
R226  | Failed [CPP-16658](https://youtrack.jetbrains.com/issue/CPP-16658)
R227  | Failed [CPP-16658](https://youtrack.jetbrains.com/issue/CPP-16658)
R228  | Pass
R229  | Failed [CPP-16659](https://youtrack.jetbrains.com/issue/CPP-16659)
...

## Reorder Parameters
Case| Result
--- | -----
RP1 | Failure (Not available) [CPP-16645](https://youtrack.jetbrains.com/issue/CPP-16645)
RP2 | Pass
RP3 | Failed (The same reason as EXF14) [CPP-1915](https://youtrack.jetbrains.com/issue/CPP-1915)
RP4 | Failed (The same reason as EXF14) [CPP-1915](https://youtrack.jetbrains.com/issue/CPP-1915)
RP5 | Pass
RP6 | Pass
RP7 | Failure (Not available) [CPP-16645](https://youtrack.jetbrains.com/issue/CPP-16645)
RP8 | Failure (Not available) [CPP-16645](https://youtrack.jetbrains.com/issue/CPP-16645)
RP9 | Failure (Not available) [CPP-16645](https://youtrack.jetbrains.com/issue/CPP-16645)

## Replace auto_ptr With unique_ptr
Case  | Result
----- | ------
RAWU1 | Pass
RAWU2 | Pass
RAWU3 | Pass
RAWU4 | Pass

## Replace If With Ternary
Case | Result
---- | ------
RIT1 | Pass
RIT2 | Failure (not available) [CPP-1944](https://youtrack.jetbrains.com/issue/CPP-1944)
RIT3 | Pass
RIT4 | Failure (not available) [CPP-1944](https://youtrack.jetbrains.com/issue/CPP-1944)
RIT5 | Pass
RIT6 | Pass
RIT7 | Pass
RIT8 | Pass
RIT9 | Failure [CPP-1945](https://youtrack.jetbrains.com/issue/CPP-1945)

## Replace Iterative For With Range For (not available) [CPP-1952](https://youtrack.jetbrains.com/issue/CPP-1952)

## Replace NULL/0 With nullptr
Case   | Result
------ | ------
RZNP1  | Pass
RZNP2  | Pass
RZNP3  | Pass
RZNP4  | Pass
RZNP5  | Pass
RZNP6  | Pass
RZNP7  | Pass
RZNP8  | Pass
RZNP9  | Pass
RZNP10 | Pass
RZNP11 | Pass
RZNP12 | Pass
RZNP13 | Pass
RZNP14 | Pass
RZNP15 | Pass
RZNP16 | Pass
RZNP17 | Pass
RZNP18 | Pass
RZNP19 | Pass
RZNP20 | Pass
RZNP21 | Pass
RZNP22 | Pass
RZNP23 | Pass
RZNP24 | Pass
RZNP25 | Pass
RZNP26 | Pass
RZNP27 | Pass
RZNP28 | Pass

## Replace String Literal With Raw String Literal (not available)

## Replace Ternary With If
Case | Result
---- | ------
RTI1 | Pass
RTI2 | Failure [CPP-1946](https://youtrack.jetbrains.com/issue/CPP-1946)
RTI3 | Pass
RTI4 | Pass
RTI5 | Failure [CPP-1946](https://youtrack.jetbrains.com/issue/CPP-1946)
RTI6 | Pass
RTI7 | Pass
RTI8 | Pass
RTI9 | Pass

## Replace Type With auto
Case   | Result
------ | ------
RTWA1  | Pass
RTWA2  | Pass
RTWA3  | Pass
RTWA4  | Pass
RTWA5  | Pass
RTWA6  | Pass
RTWA7  | Pass
RTWA8  | Pass
RTWA9  | Pass
RTWA10 | Pass
RTWA11 | Pass
RTWA12 | Pass
RTWA13 | Pass
RTWA14 | Pass
RTWA15 | Pass
RTWA16 | Pass
RTWA17 | Pass
RTWA18 | Pass
RTWA19 | Pass
RTWA20 | Pass
RTWA21 | Pass
RTWA22 | Pass
RTWA23 | Pass
RTWA24 | Pass
RTWA25 | Pass
RTWA26 | Pass
RTWA27 | Pass
RTWA28 | Pass
RTWA29 | Pass
RTWA30 | Pass
RTWA31 | Pass
RTWA32 | Pass

## Reverse Conditional
Case | Result
---- | ------
RC1  | Pass
RC2  | Pass
RC3  | Pass
RC4  | Pass
RC5  | Pass
RC6  | Pass
RC7  | Pass
RC8  | Pass

## Simplify Boolean Expression
Case | Result
---- | ------
SB1  | Pass
SB2  | Pass
SB3  | Pass
SB4  | Pass
SB5  | Pass
SB6  | Pass
SB7  | Pass
SB8  | Pass
SB9  | Pass
SB10 | Pass
SB11 | Pass
SB12 | Pass
SB13 | Pass

## Split Initialization From Declaration
Case  | Result
----- | ------
SID1  | Pass
SID2  | Failure [CPP-1947](https://youtrack.jetbrains.com/issue/CPP-1947)
SID3  | Pass
SID4  | Pass
SID5  | Pass
SID6  | Pass
SID7  | Pass
SID8  | Pass
SID9  | Pass
SID10 | Pass
SID11 | Failure (not available) [CPP-1948](https://youtrack.jetbrains.com/issue/CPP-1948)

## Split Multi-Variable Declaration
Case   | Result
-----  | ------
SMVD1  | Pass
SMVD2  | Pass
SMVD3  | Pass
SMVD4  | Pass
SMVD5  | Pass
SMVD6  | Pass
SMVD7  | Pass
SMVD8  | Pass
SMVD9  | Pass
SMVD10 | Pass
SMVD11 | Pass
SMVD12 | Pass
SMVD13 | Pass
SMVD14 | Pass
SMVD15 | Pass
SMVD16 | Pass
SMVD17 | Pass
SMVD18 | Pass
SMVD19 | Pass
