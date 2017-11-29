# Question 3

For this question, we would like you to write a Publish-Subscribe (PubSub) "class", that implements the following methods: `publish`, `subscribe`, and `unsubscribe`. If you are not familiar with this topic, a PubSub is pretty similar to the DOM events where you subscribe to an event, and when the event is fired, all your subscriptions' callbacks are called. In this case, however, all the events will be subscribed to the PubSub object.

Starting structure:

```javascript
class PubSub {
    constructor() {
        ...
    }

    publish(namespace, payload) {
        ...
    }

    subscribe(namespace, callback) {
        ...
    }

    unsubscribe(namespace, callback) {
        ...
    }
}
```

You should be able to `subscribe` multiple callbacks, and be able to `unsubscribe` them individually. The `publish` method, should call all the associated callbacks with the given namespace and pass the payload.

Example:

```javascript
// Callbacks
const log1 = x => console.log(`Log 1: ${x}`);
const log2 = y => console.log(`Log 2: ${y}`);

const p = new PubSub();

p.subscribe('example.a', log1);
p.subscribe('example.a', log2);

p.publish('example.a', 'hello-world');
// Log 1: hello-world
// Log 2: hello-world

p.subscribe('example.b', log1);
p.unsubscribe('example.a', log1);

p.publish('example.a', 'GumGum');
// Log 2: GumGum
```
