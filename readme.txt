CRUD Operations in mongo dB

db.collection.find()It is used to retrieve documents from the
collection.

db.collection.updateOne()It is used to update a single  document in the collection that satisfy the given criteria.

db.collection.updateMany()	It is used to update multiple  documents in the collection that satisfy the given criteria.

db.collection.replaceOne()It is used to replace single
document in the collection that satisfy the given criteria.

db.collection.deleteOne()It is used to delete a single document  from the collection that satisfy the given criteria.

db.collection.deleteMany()	It is used to delete multiple  documents from the collection that satisfy the given criteria

Using CURD comand 
to create collection

db.createCollection("posts")


to insert collection

db.Address.insertOne({
  title: "Post Title 1",
  body: "Body of post.",
  category: "News",
  likes: 1,
  tags: ["news", "events"],
  date: Date()
})

db.posts.insertMany([  
  {
    title: "Post Title 2",
    body: "Body of post.",
    category: "Event",
    likes: 2,
    tags: ["news", "events"],
    date: Date()
  },
  {
    title: "Post Title 3",
    body: "Body of post.",
    category: "Technology",
    likes: 3,
    tags: ["news", "events"],
    date: Date()
  },
  {
    title: "Post Title 4",
    body: "Body of post.",
    category: "Event",
    likes: 4,
    tags: ["news", "events"],
    date: Date()
  }
])
