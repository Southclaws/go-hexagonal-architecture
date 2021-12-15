# infrastructure

This directory contains non business logic components vital for system-wide function. These are the right-most items on the typical hexagonal architecture diagram.

These are things like:

- Databases
- Message queues
- Event streams
- Email services
- SMS services

They don't necessarily have to talk to external services, you can also store:

- Logger code
- Metrics
- Observability
- Tracing

Each package in here _should_ export an interface. Most of the time. You don't have to follow these rules _by the book_ you can adapt to whatever fits best. For example, config probably won't be an interface, it'll just be a simple struct. There's no real benefit to writing all the extra code for an interface and then a SINGLE implementation of that interface with a bunch of accessor methods... just export a struct. Keep it simple and idiomatic Go.
