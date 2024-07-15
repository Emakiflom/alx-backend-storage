# 0x01. NoSQL

## Resources
Read or watch:
- [NoSQL Databases Explained](https://www.mongodb.com/nosql-explained)
- [What is NoSQL?](https://www.mongodb.com/scale/nosql)
- [MongoDB with Python Crash Course - Tutorial for Beginners](https://www.youtube.com/watch?v=E-1xI85Zog8)
- [MongoDB Tutorial 2: Insert, Update, Remove, Query](https://www.youtube.com/watch?v=CB9G5Dvv-EE)
- [Aggregation](https://docs.mongodb.com/manual/aggregation/)
- [Introduction to MongoDB and Python](https://realpython.com/introduction-to-mongodb-and-python/)
- [mongo Shell Methods](https://docs.mongodb.com/manual/reference/method/)
- [Mongosh](https://docs.mongodb.com/mongodb-shell/)

## Learning Objectives
At the end of this project, you are expected to be able to explain to anyone, without the help of Google:

### General
- What NoSQL means
- What is the difference between SQL and NoSQL
- What is ACID
- What is a document storage
- What are NoSQL types
- What are the benefits of a NoSQL database
- How to query information from a NoSQL database
- How to insert/update/delete information from a NoSQL database
- How to use MongoDB

## Requirements

### MongoDB Command File
- All your files will be interpreted/compiled on Ubuntu 18.04 LTS using MongoDB (version 4.2)
- All your files should end with a new line
- The first line of all your files should be a comment: `// my comment`
- A `README.md` file, at the root of the folder of the project, is mandatory
- The length of your files will be tested using `wc`

### Python Scripts
- All your files will be interpreted/compiled on Ubuntu 18.04 LTS using python3 (version 3.7) and PyMongo (version 3.10)
- All your files should end with a new line
- The first line of all your files should be exactly `#!/usr/bin/env python3`
- A `README.md` file, at the root of the folder of the project, is mandatory
- Your code should use the pycodestyle style (version 2.5.*)
- The length of your files will be tested using `wc`
- All your modules should have a documentation (`python3 -c 'print(__import__("my_module").__doc__)'`)
- All your functions should have a documentation (`python3 -c 'print(__import__("my_module").my_function.__doc__)'`)
- Your code should not be executed when imported (by using `if __name__ == "__main__":`)

## More Info

### Install MongoDB 4.2 on Ubuntu 18.04
Follow the official installation guide:
```bash
$ wget -qO - https://www.mongodb.org/static/pgp/server-4.2.asc | apt-key add -
$ echo "deb [ arch=amd64,arm64 ] https://repo.mongodb.org/apt/ubuntu bionic/mongodb-org/4.2 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-4.2.list
$ sudo apt-get update
$ sudo apt-get install -y mongodb-org
$ sudo service mongod status
$ mongo --version

