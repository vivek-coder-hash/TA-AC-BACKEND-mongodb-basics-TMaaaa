writeCode

Write command to

- List collections from a database.
// show collections
- create a new collection in your country database which you created recently.
// db.createCollection("Mumbai")

Write code to:-

- crate a database named `weather`
// use weather
- create a capped collection named `temperature` with maximum of 3 documents and try inserting more than 3 to see the result.
//  db.createCollection("temprature" , {capped:true, size:1024 , max:3})
// db.temprature.insert({Delhi:34})
// db.temprature.insertMany([{delhi:34} , {mumbai:32} , {chennai:45}])  => Insert three documents

//db.temprature.find()  =>  Find all documents inside "temprature" collection inside weather database
//db.temprature.insert({Dharamshala:30})  =>  Insert 4th document , it will pop out very first document

- create a simple collection named `humidity`
// db.createCollection("Humididty")
// show collections =>  It will show list of collections inside database
- check whether `temperature` collection is capped or not ?
// db.temprature.isCapped()
- Delete `humidity` collection and then the entire database(weather).
//db.humidity.drop()

// db.dropDatabase()  =>  Delete current database
