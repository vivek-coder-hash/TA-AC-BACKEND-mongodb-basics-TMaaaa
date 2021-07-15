writeCode

Write code to:-

- create a database named `sports`.
// use sports
- list all databases present in local mongod server.
// show dbs
- create 3 collections named `cricket`, `football`, `TT` in sports databse.
// db.createCollection("cricket")
//db.createCollection("football")
//db.createCollection("TT")
- add multiple players in those collections which should have fields like `name`, `age` and `email` and `bid_price`.
//  db.cricket.insert([{"name":"vivek"}, {"age":27}, {"email":"info@email.com"}, {"bidPrice":1000000} ])
//db.cricket.insert([{"name":"vicky"}, {"age":27}, {"email":"info@email.com"}, {"bidPrice":1000000} ])
//db.football.insert([{"name":"vickyfootball"}, {"age":27}, {"email":"info@email.com"}, {"bidPrice":1000000}])

// db.TT.insert([{"name":"vickyfootball"}, {"age":27}, {"email":"info@email.com"}, {"bidPrice":1000000}])
- list all collections in sports database.
// show collections
- rename `TT` collection to `tennis`.

- create a capped collection called `khokho` which should have max 3 documents.
// db.createCollection("khokho" , {capped:true, size:1024 , max:3})
  Try inserting more than 3 and see what happens?
 // db.khokho.insert({p1:1})
 // db.khokho.insert({p2:2})
 // db.khokho.insert({p3:3})

 //  {p1:1} is removed
- check whether a collection is capped or not?
// db.khokho.isCapped()
- drop all documents from `football` collection.
 // db.football.drop()
- delete cricket collection completely.
// db.cricket.drop()
- delete sports database.
// db.dropDatabase()
- check which database you are connected to ?
// db
- connect to test database
//use test
