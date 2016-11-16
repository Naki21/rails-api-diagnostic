# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.

What is the purpose of a backend?

```bash
The backend allows for remote storage of data and data manipulators. It also helps make pages run faster by doing a lot of the computational processes remotely and returning the relavent info to the front end.
```

Which layer in the MVC pattern is used by the controller to fetch data?

```bash
The model layer
```

Which layer in the MVC pattern communicates with the model?

```bash
The controller
```

Why don't we use views in our interpretation of the MVC pattern?

```bash
Because we allow the browser to render the views locally which isnt really heavy enough for it to make that great of a difference.
```

What does C.R.U.D stand for?

```bash
Create, Read, Update, Destroy
```

In which part of the MVC pattern can we find C.R.U.D actions?

```bash
The controller and the model are both involved in carrying out CRUD operations but the controller is responsible for issuing CRUD commands
```

List at least 5 standard rails actions that C.R.U.D requests correspond to?

```bash
index, create. show, update, destroy
```

A user action fires a `GET` request for `/people/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```bash
- GET '/people/1' is parsed by the router
- The router tells the people controller to use the people#show actions
- This method involks the people modle to run its show function.
- It communicates with the server and returns the info to the controller
- the controller then passes that info back to the server and that is passes back to the client.
```

What is the command to generate a new rails-api app?

```bash
bundle exec rails new app_name
```

What is the command to start an instance of a rails server?

```bash
bundle exec rails server
```

What are the commands to drop, create and migrate a database from the command
line? (3 bullet points)

```bash
bundle exec rake db:drop
bundle exec rake db:create
bundle exec rake db:migrate
```

What is the command to scaffold a pet with a name and age attributes (hint:
Also think of the data types for each attribute)?

```bash
bundle exec rails g scaffold pet name:string age:integer attributes:string
```
