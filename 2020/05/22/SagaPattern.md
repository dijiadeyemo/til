Saga Microservices Pattern

**Author** : Diji

## Notes

Saga Pattern is a way of ensure ACID in a microservices system. It is a work around for one database per serivce pattern that microsevices use

### Two Approaches
* Choreography : each local transaction publishes domain events that trigger local transactions in other services.
* Orchestration : an orchestrator (object) tells the participants what local transactions to execute.

### Downsides
* Complexity 
* Over dependendence on the SEC
* Scalability?
