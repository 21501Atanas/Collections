# OnlineBookstore

## 📘 Общо описание
`OnlineBookstore` е примерна MongoDB база данни за онлайн книжарница, включваща автори, книги, клиенти, поръчки и ревюта.

## 📂 Колекции

### `authors`
- Информация за авторите
- Полета: `_id`, `name`, `nationality`, `birth_year`

### `books`
- Книги с категории, автор, цена и наличност
- Полета: `title`, `author_id`, `categories`, `price`, `stock`, `published`

### `customers`
- Данни за клиентите и техния адрес
- Полета: `_id`, `name`, `email`, `address`, `tags`

### `orders`
- Поръчки, направени от клиенти
- Полета: `_id`, `customer_id`, `book_ids`, `total_price`, `date`

### `reviews`
- Ревюта от клиенти за книги
- Полета: `_id`, `book_id`, `customer_id`, `rating`, `comment`, `date`

## 🛠️ Инсталация и стартиране

1. Инсталирайте MongoDB на своята система.
2. Стартирайте MongoDB shell:
   ```
   mongosh
   ```
3. Изпълнете скрипта `insert.js` за добавяне на данни:
   ```
   load("insert.js")
   ```
4. Изпълнете заявки от `queries.js` за четене, актуализиране, изтриване и агрегиране на данни:
   ```
   load("queries.js")
   ```
