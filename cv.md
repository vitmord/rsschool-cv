# Mordovin Vitaliy CV

## Contacts

- Address: Ryazan, Russia
- Email: vitmord@gmail.com
- Github: [vitmord](https://github.com/vitmord)
- Discord chat: VM (@vitmord)

## Summary

I'm currently working as frontend engineer at «Magnito-Kontakt» Ltd

## Skills

- HTML (BEM)
- CSS (SCSS)
- Bootstrap
- JS (Vanilla)
- Gulp
- Git
- Figma
- VS Code

## Code examples

```js
const express = require('express')
const app = express()
const port = 3000
const fs = require('fs')

app.post('/users', function (req, res) {
  const user = req.body
  fs.appendToFile(
    'users.txt',
    JSON.stringify({
      name: user.name,
      age: user.age
    }),
    (err) => {
      res.send('successfully registered')
    }
  )
})

app.listen(port, (err) => {
  if (err) {
    return console.log('something bad happened', err)
  }

  console.log(`server is listening on ${port}`)
})
```
