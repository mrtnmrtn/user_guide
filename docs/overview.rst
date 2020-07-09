Overview
========

STUB


Architecture
------------

Example plantuml:

.. uml::

   @startuml
   caption High level architecture

   [Component 1] as c1
   [Component 2] as c2

   package "My Package" {
      [<<TechType>>\nPart 1] as p1
      [<<Python>>\nProcessor] as p2
      Database "<<PostgreSQL DB>>\nDatastore" as database
   }

   c1 --> p1
   c2 --> p1
   p1 <--> p2
   p2 --> database
   p1 <-- database
   @enduml
