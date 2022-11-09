### запрос(ы) для вставки данных минимум о двух книгах в коллекцию books

```
db.books.insertMany([
   { title: "one", description: "one", authors: "one"},
   { title: "two", description: two", authors: two"},
   ...
]);
```
### запрос для поиска полей документов коллекции books по полю title

```
db.books.find( { title: { $gt: "two" } } )
```

### запрос для редактирования полей: description и authors коллекции books по _id записи

```
db.books.updateOne(
      { "_id" : 1 },
      { $set: { "title" : "hello" }, {"description": "goodbye"} }
   );
```
