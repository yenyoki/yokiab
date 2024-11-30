# Fuel Mileage Calculation Flowchart

**FC: fuel capacity

MPH: miles per hour

TM: total miles
**

```mermaid
flowchart TD
    Start([Start]) --> InputData[/ read FC, MPH/] 
    InputData --> Calculate[calculate TM = FC * MPH ]
    Calculate --> OutputData[/Print TM /]
    OutputData --> End([End])
