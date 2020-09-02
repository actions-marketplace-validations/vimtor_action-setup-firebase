<div align="center">
   <h1>🔥 setup-firebase</h1>
   <p>Setup firebase-tools CLI for multiple steps</p>
</div>

## 🧠 Why

There is an excellent action already: [firebase-action](https://github.com/w9jds/firebase-action), but it forces you to run a command in order to work.

With this one, after running the action you can use the firebase-tools CLI from anywhere: npm script, shell...

## 🚀 Usage

Simply add the action to get access to the firebase CLI.

```yaml
jobs:
  setup-firebase:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v2
      - uses: actions/setup-node@v1
      - uses: pocket-studios/action-setup-firebase@v1
        with:
          firebase-token: YOUR_TOKEN
```

## ⚙ Inputs

**Name**|**Description**|**Required**
-----|-----|-----
firebase-token|Firebase token you can get by running `firebase login:ci`|✔

## 👋 Support

If you find our work useful, you can [support our work](https://github.com/sponsors/pocket-studios) and win a burrito 🌯
