# Question 1

Given the following arrays of post:

```javascript
const posts = [
    {
        id: '1',
        userId: '15',
        text: '...',
        images: [
            'http://via.placeholder.com/310x10',
            'http://via.placeholder.com/250x170',
        ]
    },
    {
        id: '2',
        userId: '65',
        text: '...',
        images: [
            'http://via.placeholder.com/330x35',
        ]
    },
    {
        id: '3',
        userId: '12',
        text: '...',
        images: [
            'http://via.placeholder.com/150x90',
            'http://via.placeholder.com/50x550',
            'http://via.placeholder.com/670x120'
        ]
    },
    {
        id: '4',
        userId: '15',
        text: '...',
        images: []
    },
]
```

Write a function that takes the array above and gives us the following output, which is an array of all images in the posts listed above.

Output:

```javascript
[
    'http://via.placeholder.com/310x10',
    'http://via.placeholder.com/250x170',
    'http://via.placeholder.com/330x35',
    'http://via.placeholder.com/150x90',
    'http://via.placeholder.com/50x550',
    'http://via.placeholder.com/670x120'
]
```
