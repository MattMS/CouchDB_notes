# Futon

Once CouchDB is installed, you can access
[Futon](http://localhost:5984/_utils/)
which is a web interface for working with CouchDB.
It is great for playing with databases straight away.

The [CouchDB docs](http://localhost:5984/_utils/docs/) will also be
available locally.
These will be appropriate to the version you have installed, where
others on the Internet may not be.

There will be 2 databases installed, `_replicator` and `_users`, but you
should leave these alone for now.


## Admin party

CouchDB starts in "admin party" mode.
This is shown in the bottom right corner, along with a "fix this" link.
Clicking the link will open a dialog with username and password inputs,
along with information on users that *you should read*.

"Admin party" means that anyone with access to the server has permission
to do anything they like.
This is not a problem to start with because the default is to only
provide access to your local machine.
When you make CouchDB available to anyone else, you will need to make
sure you have set up an admin account and permissions on databases.

Leaving the server in "admin party" mode while learning will mean that
you do not have to keep logging in each time your session expires.


## Create a database and documents

Use the link in the top left corner to create a database and then you
can create documents within it.

Avoid starting a database, document or field name with an underscore
because these can have special meanings.

The document `_id` field is used in the URL to access it.

Make sure you save your document (top left corner) when you are done,
you will get reminded of this if you try to leave the page.
