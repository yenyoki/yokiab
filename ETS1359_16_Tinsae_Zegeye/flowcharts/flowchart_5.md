# File Transfer Time Calculation Flowchart
**FS: file size
 
 time taken (TT) in:

 D: days

 H: hours
 
 M: minutes
**

```mermaid
flowchart TD
    Start([Start]) --> InputData[/Read FS /]
    InputData --> InitializeRate[rate = 960]
    InitializeRate --> CalculateTime[ calculate TT = FS/ rate]
    CalculateTime --> CalculateDays[convert TT to: D= TT/ 86400]
    CalculateDays --> CalculateHours[convert TT to: H =TT/ 3600]
    CalculateHours --> CalculateMinutes[convert TT to: M = TT / 60]
    CalculateMinutes --> OutputData[/Print D,H,M and TT/]
    OutputData --> End([End])
