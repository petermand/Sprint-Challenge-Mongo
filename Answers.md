#1. A database is a structed store of data that is  organized an accessible.
    A collection is how a non-relation DB (like mongo) stores its documents.
    A document is the format that mongo stores datarecords in

#2.  To create a relationship in MongoDB, either embed a BSON document within another, or reference it from another.

Sometimes it's not feasible to embed entire document — for example, when we are modeling people. Use this pattern to build relationships.

Determine if data "belongs to" a document — is there a relation?

Embed when possible, especially if the data is useful and exclusive ("belongs in").

Always reference _id values at minimum.

Denormalize the useful parts of the relationship. Good candidates do not change value often, or ever, and are useful.

Be mindful of updates to denormalized data and repair relationships

#3 Model–view–controller (MVC) is a software architectural pattern for user interfaces that divides an application into three interconnected parts. This is done to separate internal representations of information from the ways information is presented to, and accepted from, the user. The MVC design pattern decouples these major components allowing for efficient code reuse and parallel development.S