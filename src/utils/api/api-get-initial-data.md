# getInitialData()

```js
export function getInitialData() {
    return Promise.all([
        _getUsers(),
        _getPolls(),
    ]).then(([users, polls])) => ({
        users: formatUsers(users),
        polls: formatPolls(polls)
    })
}
```
