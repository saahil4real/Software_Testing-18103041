# Software Testing
## Lab Assignment 1 
## Sahil Kakkar (18103041) 

//TODO
usecase diagram

#### Sequence Diagram (Student)

```
@startuml Use Case Diagram
left to right direction
skinparam packageStyle rectangle
actor Student
actor Admin
actor Teacher
rectangle Student_Wellness_Monitor {
  
  Teacher -- (Login)
  Student -- (Login)
  (Login Error) .> (Verify Password) : extends
  (Login) .> (Verify Password) : include
  Student -- (Fill Questionnaire)
  (Fill Questionnaire) .> (Analysis) : include
  (Analysis) -- Admin
  Teacher -- (Student Details)
  (Student Details) .> (Display Data) : include
  (Display Data) -- Admin
}
@enduml
```

<img src="https://github.com/saahil4real/Software_Testing-18103041/blob/main/Lab_Assignment_1/Sequence_Diagram_student.png" alt="SEQUENCE_DIAGRAM" width="400" height="500">

#### Usecase Diagram

<img src="https://github.com/saahil4real/Software_Testing-18103041/blob/main/Lab_Assignment_1/UseCase_Diagram.png" alt="UseCase_Diagram" width="400" height="500">

