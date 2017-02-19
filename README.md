# simple-pub-sub
Simple pub-sub system to include in JS projects.

Written in ES6, to include with babel-like stacks.

## Usage

### Subscribe: 

```js
import { subscribe } from './pubsub';

subscribe('eventSubscribedTo', param => {
  // action to do when the event will be published
  // could be internal state update or side effect
});
```

### Publish:

```js
import { dispatch } from './pubsub';

dispatch('eventSubscribedTo', param); // action triggered
```
