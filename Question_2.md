# Question 2

The following endpoint:
```
https://jsonplaceholder.typicode.com/users/<INSERT_ID_HERE>
```

Returns some information about a particular user:

```javascript
{
  "id": 1,
  "name": "Leanne Graham",
  "username": "Bret",
  "email": "Sincere@april.biz",
  "address": { ... },
  "phone": "1-770-736-8031 x56442",
  "website": "hildegard.org",
  "company": { ... }
}
```

Write a function that takes a list of user Ids and returns their names.

```javascript
const usersIdList = [1, 2, 3];
```

Example:

```javascript
const output = getUserNamesByIds([1, 2]);
console.log(output); // ['Leanne Graham', 'Ervin Howell']
```

**Note**: Extra points if you can do all the request concurrently, rather than sequentially.
