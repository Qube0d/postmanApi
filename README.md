# Postman + newman + github actions (Simple store template)

## Steps to run
1. Download this repo.
2. Run this code in BASH to install node.js dependencies:
```
npm i
```
3. Run this code in BASH to run testing server locally
```
npm run tern-on-api
```

### Overview of local server testing
Routes `/products`, `/orders` and `/users`. Below is a table of supported operations with `products` as example resource. The same operations are also supports for `orders/` and `users/`.

| VERB     |Route          | Input      | Output             |
|----------|---------------|------------|--------------------|
| GET      | /products     | *None*     | **Array**          |
| GET      | /products/:id |  **e.g 3** | **Object**         |
| POST     | /products     | **object** | **Created object** |
| PUT      | /products     | **object** | **Updated object** |
| DELETE   | /products/:id | **e.g 3**  | **Deleted object** |


5. Upload `storeV2.postman_collection` in Postman app
6. Run product folder tests in postman

### GitHub action
To see the result of testing on the GitHub page click the link on the GitHub page in the about block from the right sidebar(the top right) on this page.

On Github page we can see the result of API testing from file petstore.collection.json

