## Graph-Project
name: Zehua Yu
   StudentNo: G00307279



### what is NEO4J
>Neo4j is a graph database management system developed by Neo Technology, Inc. Described by its developers as an ACID-compliant transactional database with native graph storage and processing,[3] Neo4j is the most popular graph database according to db-engines.com.[4]

>Neo4j is available in a GPL3-licensed open-source "community edition", with online backup and high availability extensions licensed under the terms of the Affero General Public License. Neo also licenses Neo4j with these extensions under closed-source commercial terms.[5]

>Neo4j is implemented in Java and accessible from software written in other languages using the Cypher Query Language through a transactional HTTP endpoint, or through the binary 'bolt' protocol.

[WIKI]:https://en.wikipedia.org/wiki/Neo4j "NEO4J WIKI"



### Introduction
>This project mainly base on information from my timetable. it includes 5 courses, such as Software Testing, Databases Management and so on, also earch class has individual teacher, project and so on. User can easily find out information they want by time, group, major.




### Data structure of NEO4J
>In Neo4j, everything is stored in the form of either an edge, a node, or an attribute. Each node and edge can have any number of attributes. Both the nodes and edges can be labelled. Labels can be used to narrow searches. As of version 2.0, indexing was added to Cypher with the introduction of schemas.[14] Previously, indexes were supported separately from Cypher.


### Neo technology
>Neo4j is developed by Neo Technology, Inc., based in the San Francisco Bay Area, United States, North America, and also in Malmö, Sweden, Europe. The Neo Technology board of directors consists of Rod Johnson (founder of the Spring Framework), Chris Barchak (Partner at Conor Venture Partners), Magnus Christerson (Vice President of Intentional Software Corp), Nikolaj Nyholm (Partner at Sunstone Capital), Guarav Tuli (Principal at Fidelity Growth Partners), and Johan Svensson (CTO of Neo Technology).



### what elements are stored in my project
* lecture
* lecturer
* project
* grade
* timeslot
* group
* room number


### The structure of project


          level   teacher                 group(groupA/B/C)
              \   |                      /
               \  |                     /
    project ---- Lecture----------timeslot------room(room number)
                  \
                   \
              timeslot(different time of class)

  I made relationship with other lectures also(there are 5 lecture)   

### console
  (make node)
  CREATE (Graph:Lecture {title:'Graph Theory' })
  CREATE (Deirdre:lecturer{Fname:'Deirder'})
  CREATE (Project1:Project {topic:'Graph for NEO4J'})
  CREATE (mTime1:TimeSlot {Timeslot:'9:00-10:00 Monday'})
  CREATE (r0145:Room {RoomNumber:'0145'})

 (make relationship)
  CREATE
  (Year)-[:Year_Of]->(Graph),
  (Year)-[:Year_Of]->(Database_Mgmt),
 


### Conclusion

Neo4j is a kind of special databases technology, it has too many advantages for users. users are able to cleary know all elements of data, also they catch relationship each other. This depends on how you are trying to make recommendations. If this is part of a real-time system, the data invariably need to be in memory anyway. The algorithms are going to involve several if not hundreds of bits of data, and if a database query is already even tens of milliseconds, there's no way it will finish "fast".     





