## Tabelas

### Users
- id: INT (primary key)
- name: VARCHAR(255)
- email: VARCHAR(255)

### Books
- id: INT (primary key)
- title: VARCHAR(255)

### Authors
- id: INT (primary key)
- name: VARCHAR(255)

### BookAuthors
- bookId: INT (foreign key to Books.id)
- authorId: INT (foreign key to Authors.id)

### BorrowedBooks
- userId: INT (foreign key to Users.id)
- bookId: INT (foreign key to Books.id)

### BookRatings
- userId: INT (foreign key to Users.id)
- bookId: INT (foreign key to Books.id)
- rating: INT
