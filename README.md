# Create Daily english Issue Action

automatic create daily english issue for nick19910321/study-every-day

## Inputs

## `token`

**Required** github token.

## Example usage

uses: nick19910321/create-daily-english-issue-action@main

with:
token: 'github token'

```js
jobs:
  create_daily_english_issue:
    runs-on: ubuntu-latest
    name: create daily english issue
    steps:
      - name: Checkout
        uses: actions/checkout@v2
      - name: create daily english issue action step
        uses: nick19910321/create-daily-english-issue-action@main
        env:
          TOKEN: ${{ secrets.TOKEN }}
        with:
          token: ${{env.TOKEN}}
```
