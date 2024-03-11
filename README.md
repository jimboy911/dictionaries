# dictionaries
Working with Dictionaries

python - working with dictionaries

From:
https://www.w3schools.com/python/python_dictionaries_nested.asp

///////

sample of a basic dictionary

basic_dictionary = { "brand": "Subaru", "model": "WRX", "year": "2017"}

////////

to get the keys (brand, model, year)

keys = basic_dictionary.keys()
print(keys)

///////

to access the data stored in one of the keys

data = basic_dictionary.get("model")
print(data)

///////////

how to add to a dictionary

basic_dictionary["color"] = "red"

///////

how to remove from a dictionary

del basic_dictionary["color"]

this is the most common way. there is also pop(), popitem(), and clear() methods

//////////

nested dictionary

myfamily = {
  "child1" : {
    "name" : "Emil",
    "year" : 2004
  },
  "child2" : {
    "name" : "Tobias",
    "year" : 2007
  },
  "child3" : {
    "name" : "Linus",
    "year" : 2011
  }
}

//////

alternatively you can create dictionaries that reference other dictionaries

child1 = {"name": "Emil", "year": 2004}
child2 = {"name": "Tobias", "year": 2007}
child3 = {"name": "Linus", "year": 2011}

myfamily = {"child1": child1, "child2": child2, "child3": child3}

////////

how do you access data from this?

print(myfamily["child2"]["name"])
