Chitter Challenge
=================

Challenge:
-------
Writing a small Twitter clone that will allow the users to post messages to a public stream.

Features:
-------

```
STRAIGHT UP

As a Maker
So that I can let people know what I am doing  
I want to post a message (peep) to chitter

As a maker
So that I can see what others are saying  
I want to see all peeps in reverse chronological order

As a Maker
So that I can better appreciate the context of a peep
I want to see the time at which it was made

As a Maker
So that I can post messages on Chitter as me
I want to sign up for Chitter

HARDER

As a Maker
So that only I can post messages on Chitter as me
I want to log in to Chitter

As a Maker
So that I can avoid others posting messages on Chitter as me
I want to log out of Chitter

ADVANCED

As a Maker
So that I can stay constantly tapped in to the shouty box of Chitter
I want to receive an email if I am tagged in a Peep
```

## Technical Approach:
-----
In this unit, we integrated a database into Bookmark_Manager using the `PG` gem and `SQL` queries. we're required to continue to use this approach when building Chitter Challenge.

### Data Table:
```
Chitter:
|--------------------------------------------|
| peep_id | peeps | peeped_time | account_id |
|--------------------------------------------|
| 1       | "Hi!" | current time| 1          |
|--------------------------------------------|

Chitter_account:
|--------------------------------------------------|
| account_id | account_name | aacount_email |  pw  |
|--------------------------------------------------|
| 1          | Pikachu      | poke@mail.com | pika |
|--------------------------------------------------|
```

## Setting up:
----
Gems used:
  Capybara, Rspec, pg, Sinatra, Sinatra-contrib.

### How to
Clone this repository, and `bundle update`

### setting up data base
Connect to `psql` and create the `Chitter` database like below.
```
CREATE DATABASE Chitter;
```
To set up the appropriate tables, connect to the database in `psql` with `\c table_name` and run the SQL scripts in the `db/migrations` folder in the given order.

### Runnig app
Typing `rackup` in terminal.
It shold give you your local host "port number" at the very end.
Copy number and paste in your web browser `http://localhost:YOUR_PORT_NUMBER_HERE`

### Run tests:
`rspec` or for linting test - `rubocop`

-----------------------------------------

Notes on functionality from Makers:
------

* You don't have to be logged in to see the peeps.
* Makers sign up to chitter with their email, password, name and a username (e.g. samm@makersacademy.com, password123, Sam Morgan, sjmog).
* The username and email are unique.
* Peeps (posts to chitter) have the name of the maker and their user handle.
* Your README should indicate the technologies used, and give instructions on how to install and run the tests.

Bonus:
-----

If you have time you can implement the following:

* In order to start a conversation as a maker I want to reply to a peep from another maker.

And/Or:

* Work on the CSS to make it look good.

------------------------------
Where I've got up to:
Created Database and one table: Chitter withi no details in yet. Rokuban to do.
