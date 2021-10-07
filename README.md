## Making requests
### ``By default, the API_HOST is http://localhost:5000/api/v1``

#### Create a new books
request url `API_HOST/books`

request method `POST`

request body 
`{`
name: `{String}`(required),
type: `{String}`(required),
lang: `{String}`(required(ru,en,he))
`}`  
 
 
#### Get all books or search
request url `API_HOST/books`

request method `GET`

##### The following filters and sorting are allowed
`{`

   type: `{String}`,

   lang: `{RU or EN or HE}`,
   
`}`


#### Get a single book
request url `API_HOST/books/:bookId`
request method `GET`

#### Update a book
request url `API_HOST/books/:bookId`
request method `PATCH`
request body 
`{`
name: `{String}`,
type: `{String}`,
lang: `{String(ru,en,he)}`
`}`         

#### Delete the book
request url `API_HOST/books/:bookId`
request method `DELETE`
