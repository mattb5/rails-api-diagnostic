# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What is the purpose of a backend?

```bash
to allow the server to fetch information from databases and return it (in the form of JSON)
to the client
```

Which layer in the MVC pattern is used by the controller to fetch data?

```bash
model
```

Which layer in the MVC pattern communicates with the model?

```bash
controller
```

Why don't we use views in our interpretation of the MVC pattern?

```bash
because we are not sending any information from model that will change html structure on our client side.  
```

What does C.R.U.D stand for?

```bash
create, read, update, delete
```

In which part of the MVC pattern can we find C.R.U.D actions?

```bash
model - i think more particularly the database which interacts with only the model of the MVC
```
List at least 5 standard actions that C.R.U.D corresponds to?

```bash
create_table
insert into
update
SELECT from
delete
```

A user action fires a `GET` request for `person/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```bash
1. client makes AJAX request to server.
2. router receives that request and passes it to the person controller which is
3. person controller then issues request to person model.   the person model fetches gets necessary information from the database about person 1.  it then returns this gotten information to the person model
4. person model returns sends that get information in the form of a JSON back to the client
5. client interprets the json and can place the gotten request to the webpage
```

What is the command to generate a new rails-api app?

```bash
.create
```

What is the command to start an instance of a rails server?

```bash
rails s
```

What are the commands to drop, create and migrate a database? (3 bullet points)

```bash
- drop database
- create database
- generate migration
```

What is the command to scaffold a pet with a name and an age?

```bash
create_table :pet do |t|
  t.string :name,
  t.string :age
end```

List two advantages of using serializers? (2 bullet points)

```bash
-allows us to process data structures into a format that can be sent across a network to be used later
- allows us to store data in memory
```
