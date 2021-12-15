#############################################################################################

# GraphQl Server

#############################################################################################

# What you need to run this ?

1. node
2. git

follow the instructions

1. clone the repository
2. npm install
3. npm run dev:server // to run the graphql server
4. npm run json:server // to run the Json server (in new terminal)
5. localhost:5000/graphql // graphql playground
6. localhost:3000 // json server

# What is GraphQl ?

1. Application layer query language
2. Open sourced by facebook in 2015
3. can be used with any type of database
4. Ability to ask for excatly what you need and nothing more
5. Get multiple resources in a single request

# Simple Query Vs Payload

- Query:
```
{
user(id:"33"){
name,
email
}
}
```
- Payload:

{
"user":{
"id": "33",
"name": "kathir karthik",
"email": "kathirkarthik2602@gmail.com"
 }
}

- Multiple Resources in Query vs Payload:

- Query:

{
user(id:"33"){
name,
email
posts{
title
}
}
}

- Payload:

{
"user":{
"id": "33",
"name": "kathir karthik",
"email": "kathirkarthik2602@gmail.com"
"posts":[
{"title":"Post1"},
{"title":"Post2"}
]}
}

- GraphQl Types

\*\* GraphQL API's are organized in terms of types and fileds

Type Query {
user:User
}

Type User {
name:String
age:int
friends:[User]
}

# GraphiQl Tool

1. Graphical intractive GraphQl IDE
2. Runs in the browser
3. Syntax highlihting
4. Error reporting
5. Automation & Hinting

# Support languages

(C# , Javascript , PHP, Go lang, Java, Ruby, Erlang, Elixir, Clojure, Python)

# follow me : https://github.com/raydcode

# referDocs : https://graphql.org/graphql-js/running-an-express-graphql-server/
