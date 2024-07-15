## Домашнее задание к занятию «2.6. База данных и хранение данных»

### Выполнил Сергей Жвакин scripscratch@mail.ru

### Задания 1

Ознакомился с документацией MongoDB.

### Задания 2

`запрос(ы) для вставки данных минимум о двух книгах в коллекцию books`

```
db.books.insertMany( [
      {
        title: 'Book 1',
        description: 'Description 1',
        authors: 'Author 1',
      },
      {
        title: 'Book 2',
        description: 'Description 2',
        authors: 'Author 2',
      }
   ] );
```

---

`запрос для поиска полей документов коллекции books по полю title`

```
db.books.find(
    {
     "title": "SearchingTitle",
   }
)
```

---

`запрос для редактирования полей: description и authors коллекции books по _id записи`

```
db.books.update(
    { _id: 1 },
    {
        $set: {
            description: "NewDescription",
            authors: "NewAuthors"
        }
    }
)
```

---

Благодарю за внимание!
