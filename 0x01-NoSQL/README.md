# 0x01-NoSQL

This project focuses on learning and implementing NoSQL databases, specifically MongoDB. It covers basic MongoDB operations using both the MongoDB shell and PyMongo in Python.

## Author
- Shighi

## Requirements

### MongoDB Command Files
- All files will be interpreted/compiled on Ubuntu 18.04 LTS using MongoDB (version 4.2)
- All files should end with a new line
- The first line of all files should be a comment: `// my comment`
- A README.md file at the root of the project folder is mandatory
- File length will be tested using `wc`

### Python Scripts
- All files will be interpreted/compiled on Ubuntu 18.04 LTS using Python 3.7 and PyMongo 3.10
- All files should end with a new line
- The first line of all files should be exactly `#!/usr/bin/env python3`
- Code should use pycodestyle style (version 2.5.*)
- All modules should have documentation (`python3 -c 'print(__import__("my_module").__doc__)'`)
- All functions should have documentation (`python3 -c 'print(__import__("my_module").my_function.__doc__)'`)
- Code should not be executed when imported (use `if __name__ == "__main__":`)

## Installation Guide
Install MongoDB 4.2 in Ubuntu 18.04:
```bash
$ wget -qO - https://www.mongodb.org/static/pgp/server-4.2.asc | apt-key add -
$ echo "deb [ arch=amd64,arm64 ] https://repo.mongodb.org/apt/ubuntu bionic/mongodb-org/4.2 multiverse" > /etc/apt/sources.list.d/mongodb-org-4.2.list
$ sudo apt-get update
$ sudo apt-get install -y mongodb-org
$ sudo service mongod start
$ pip3 install pymongo
```

## Tasks

### 0. List all databases
- Write a script that lists all databases in MongoDB.
- File: `0-list_databases`

### 1. Create a database
- Write a script that creates or uses the database `my_db`.
- File: `1-use_or_create_database`

### 2. Insert document
- Write a script that inserts a document with attribute name="ALX" in the collection `school`.
- File: `2-insert`

### 3. All documents
- Write a script that lists all documents in the collection `school`.
- File: `3-all`

### 4. All matches
- Write a script that lists all documents with name="ALX" in the collection `school`.
- File: `4-match`

### 5. Count
- Write a script that displays the number of documents in the collection `school`.
- File: `5-count`

### 6. Update
- Write a script that adds a new attribute to documents with name="Holberton school" in the collection `school`.
- The attribute is address with value "972 Mission street".
- File: `6-update`

### 7. Delete by match
- Write a script that deletes all documents with name="ALX School" in the collection `school`.
- File: `7-delete`

### 8. List all documents in Python
- Write a Python function that lists all documents in a collection.
- Prototype: `def list_all(mongo_collection):`
- File: `8-all.py`

### 9. Insert a document in Python
- Write a Python function that inserts a new document in a collection based on kwargs.
- Prototype: `def insert_school(mongo_collection, **kwargs):`
- File: `9-insert_school.py`

### 10. Change school topics
- Write a Python function that changes all topics of a school document based on the name.
- Prototype: `def update_topics(mongo_collection, name, topics):`
- File: `10-update_topics.py`

### 11. Where can I learn Python?
- Write a Python function that returns the list of schools having a specific topic.
- Prototype: `def schools_by_topic(mongo_collection, topic):`
- File: `11-schools_by_topic.py`

### 12. Log stats
- Write a Python script that provides stats about Nginx logs stored in MongoDB.
- Display: number of logs, methods count, number of status checks.
- File: `12-log_stats.py`

### 13. Regex filter (Advanced)
- Write a script that lists all documents with name starting by "ALX" in the collection `school`.
- File: `100-find`

### 14. Top students (Advanced)
- Write a Python function that returns all students sorted by average score.
- Prototype: `def top_students(mongo_collection):`
- File: `101-students.py`

### 15. Log stats - new version (Advanced)
- Improve 12-log_stats.py by adding the top 10 of the most present IPs in the nginx collection.
- File: `102-log_stats.py`

## Repository
- GitHub repository: `alx-backend-storage`
- Directory: `0x01-NoSQL`
