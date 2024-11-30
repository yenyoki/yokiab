# Power Calculation Flowchart

**X: base

Y: exponent
**

```mermaid
flowchart TD
    Start([Start]) --> InputData[/Read X and Y/]
    InputData --> Calculate[ power = X^Y ]
    Calculate --> OutputData[/Print power/]
    OutputData --> End([End])
