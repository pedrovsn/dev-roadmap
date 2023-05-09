
# Backend Mid

Create a Banking Service

## Task

### Use case

BooBank is a new Fintech which offers to it's customers an affordable bank account without burocracy. 

### Resources

#### Backoff Service
The business rules requires that each account belongs to an bank agency. So, we need to create an Default Agency with the following attributes: Id (numeric, generated by the service), code (numeric, given by the admin), name (string, given by the admin), address (Address object)

#### Account Creation
As an API Client, I need to make a request with the POST method to create a banking account. The account must be saved in a database with my account ID, generated by the service, my first name, my last name, my address, my register (CPF), my password and my phone number. Also, the current date and time, to audit later.

#### Create a Wire
As an API Client, I need to create a wire to another bank account. The wire must be saved in a database with the wire ID, generated by the service, the origin account number, the destination account number, the value, it's status (PENDING, REFUSED, PROCESSED), notes (string which could contain the reason to a wire be refused), the creation date and time and the update date and time. As an wire requires a few internal validations, the recurn code should be 201 CREATED, and the wire should be in a Queue.

## How to deliver it?

The task can be marked as finished if it has a Github repository containing the source code, and a readme with the instructions to build and test it. As a database is required to finish this task, a docker-compose and instructions on how to use it would be great.