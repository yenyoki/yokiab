# BMI Calculation and Evaluation Flowchart

**BMI: body mass index

num: nunmber of person

W: weight

H: height 

i:counter**


```mermaid
flowchart TD
    Start([Start]) --> InputData[/ read num /]
    InputData --> InitializeCounter[counter i = 1 ]
    InitializeCounter --> ReadData[/read W and H/]
    ReadData --> CalculateBMI[ calculate BMI = W / H*H ]
    CalculateBMI --> CheckBMI{BMI between 18.5 and 24.9?}
    CheckBMI -->|Yes| NormalBMI[/Print BMI and "Normal"/]
    CheckBMI -->|No| CheckOverweight{BMI greater than 25?}
    CheckOverweight -->|Yes| OverweightBMI[/Print BMI and "Overweight"/]
    CheckOverweight -->|No| UnderweightBMI[/Print BMI and "Underweight"/]
    NormalBMI --> IncrementCounter[counter i++ ]
    OverweightBMI --> IncrementCounter
    UnderweightBMI --> IncrementCounter
    IncrementCounter --> CheckCounter{i <= num?}
    CheckCounter -->|Yes| ReadData
    CheckCounter -->|No| End([End])
