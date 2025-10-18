+++
date = '2025-10-19T01:08:08+02:00'
draft = true
title = 'PlantUMP'
+++




## Diagramme de séquence

{{</* plantuml */>}}
@startuml
Alice -> Bob : Bonjour
Bob -> Alice : Salut !
@enduml
{{</* /plantuml */>}}

## Diagramme de classes

{{</* plantuml */>}}
@startuml
class Car {
  -String model
  +void start()
  +void stop()
}

class Driver {
  -String name
  +void drive(Car car)
}

Driver --> Car : drives >
@enduml
{{</* /plantuml */>}}
