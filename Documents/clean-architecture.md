# Clean architecture
[Source](https://jasontaylor.dev/clean-architecture-getting-started/) 

## Domain 

- Entities of the project 

- Domain exceptions in domain logic 

## Application 

- Services (Logic to communicate with a repository and logic that belongs to a service) 

- Interfaces (Can be used by the Persistence layer and Infrastructure) -> IRepository(TEntity), IRepository(TDto) 

- Data Transfer Objects (Entity -> Dto, Dto -> Entity)  

- Configurations (Specific changes in Json file(How you configure your service to run)) 

## Persistence  

- Database Choice (Why not annotate using EF? (Required) --> Configuration over Convention (Database choice has nothing to do with your domain!)). 

- Configuration (EFCore) -> Modelling of relationships  

## Infrastructure 

- Third party services -> Communication outside your application (Network code, websockets etc.) 

## Presentation 

- Mapping (Dirty code to glue everything together) supposed to be a separate layer 

- Controllers (Communication between frontend and backend that are dependent of off interfaces.) 
