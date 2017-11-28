# Question 2

Given the following endpoint:
```
https://jsonplaceholder.typicode.com/users/:userId
```
That returns some information about a particular user:
```
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

We would like to write a function that takes a list of userIds, and returns their names.

```
const usersIdList = [1, 2, 3];
```

Example:

```
const output = getUserNamesByIds([1, 2]);
console.log(output); // ['Leanne Graham', 'Ervin Howell']
```

**Note**: Extra points if you can do all the request concurrently, rather than sequentially.
