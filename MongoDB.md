---
title: "MongoDB"
author: "WeizhouS"
date: "3/20/2019"
output: pdf_document
---

JavaScript Object Notation (JSON) is the basis of MongoDB  

- objects: `{tring: value,...}`  
- arrays: `[value,...]`  
- values: `string, number, true, false, null, object, array`

``` py
import requests
from pymongo import MongoClient

# Client connect to "localhost" by default
client = MongoClient()
# Create local "nobel" dta base on the fly
db = client["nobel"]

for collection_name in ["prizes", "laurestes"]:
  singular = collection_name[:-1]
  response = request.get("http://api.nobelprize.org/vq/{}.josn".format(singular))
  documents = response.json()[collection_name]
  
  # Crete collections on the fly
  db[collection_name].insert_many(documents)

# Access dbs and collections as attributes
assert client.nobel == db
assert db.prizes == db["prizes"]

# Count documents
n_prizes = db.prizes.count_documents({})
n_laureates = db.laureates.count_documents({})

# Find one document to inspect
doc = db.prizes.find_one({})

```

- access database names
- access collection names








