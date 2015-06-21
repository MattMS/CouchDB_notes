# Why CouchDB?

The concerns I had at various points learning CouchDB and how more study
helped me get over them.

One major point to note: CouchDB is not appropriate for every problem!

I have realised that there is not one database that is best for every
situation, even though you can probably bend most to be acceptable.

Check out [Redis](http://redis.io/), [MongoDB](https://www.mongodb.org/)
and [LevelDB](http://leveldb.org/) to broaden your tool set.


## Erlang

When choosing to learn a new application, I prefer to choose those
written in a language I am familiar with.

CouchDB is written in
[Erlang](https://en.wikipedia.org/wiki/Erlang_%28programming_language%29),
which I had not looked at before.
But reading about features, such as the focus on concurrency, made me
appreciate the choice.


## JSON documents

All data is stored in JSON documents that are grouped in databases.

Learning that you replace the entire JSON document when you make any
change seemed clunky compared to updating a single field in a row of an
SQL table.

This requires rethinking the structure of data and can help decide if
CouchDB is appropriate for your current situation.

It also promotes thinking about the features you really need.
Does the user actually need to query or update any field at any time?


## Javascript in JSON

Storing Javascript in JSON seems strange at first.
One worry was that Javascript would need to be copied into multiple
databases and a missed update would cause difficult errors.

Thinking about the database as an API that combines the server code with
the database helped this concern.
Going further, some applications may not even need a separate server!

Having the querying functionality stored with the data also means it can
be moved with the data.
