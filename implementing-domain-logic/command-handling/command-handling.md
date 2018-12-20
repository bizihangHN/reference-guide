# Command model

In a CQRS-based application, a Domain Model \(as defined by Eric Evans and [Martin Fowler](https://martinfowler.com/bliki/CQRS.html)\) can be a very powerful mechanism to harness the complexity involved in the validation and execution of state changes. Although a typical domain model has a great number of building blocks, one of them plays a dominant role when applied to command processing in CQRS: the Aggregate.

A state change within an application starts with a Command. A command is a combination of expressed intent \(which describes what you want done\) as well as the information required to undertake action based on that intent. The command model is used to process the incoming command, to validate it and define the outcome. Within this model, a command handler is responsible for handling commands of a certain type and taking action based on the information contained inside it.