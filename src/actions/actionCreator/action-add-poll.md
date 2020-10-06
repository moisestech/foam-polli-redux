# 🔺 addPoll()

```js
export const APP_POLL = "ADD_POLL";
export const RECEIVE_POLLS = "RECEIVE_POLLS";

function addPoll(poll) {
  return {
    type: ADD_POLL,
    poll,
  };
}
```
