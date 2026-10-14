Contract aspect

Product, CreateProductInput, shared identifiers, and any intentionally reusable paging abstractions.

Public contract; no resolver implementation or persistence dependency.

Operation aspect

ProductQueries, ProductMutations, resolver methods, DataLoaders, and calls into the Data aspect.

Implements the contract and coordinates application behavior.

Endpoint aspect

Registers the GraphQL services and maps the HTTP endpoint; its host configuration composes the schema.

Transport and hosting, not capability business logic.

Data aspect

EF Core queries, persistence models, and capability-specific data access.

Does not need to know about GraphQL's resolver machinery.