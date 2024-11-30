# Salary Calculation Flowchart
**BP: bons payment

WWH: weely working hours

BPH: bonus rate per hours

GS: gross salary

BS: base salary

BP: bonus payment

P: payment

T: tax

TD: tax deduction

PD: pension deduction

NS: net salary**

```mermaid
flowchart TD
    Start([Start]) --> InputData[/read name,BP,WWH and BPH/]
    InputData --> CalculateBonus[calculate BP= WWH * BPH]
    CalculateBonus --> CalculateGross[calculate GS = BS + BP]
    CalculateGross --> CalculatePension[calculate PD = GS * P]
    CalculatePension --> CalculateTax[calculate TD = GS * T]
    CalculateTax --> CalculateNet[calculate NS = GS - PD- TD]
    CalculateNet --> OutputData[/Print NT, BP and GS/]
    OutputData --> End([End])
