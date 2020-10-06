# 🔺 handleAddPoll()

```js
import { savePoll } from "../utils/api";

export function handleAddPoll(poll) {
  return (dispatch, getState) => {
    const { authedUser } = getState();

    dispatch(showLoading());

    return savePoll({
      ...poll,
      author: authedUser,
    })
      .then((poll) => dispatch(addPoll(poll)))
      .then(() => dispatch(hideLoading()));
  };
}
```

### UTILS API

- [[api-save-poll]]
