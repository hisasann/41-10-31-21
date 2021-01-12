# 41 10 31 21

[41 10 31 21](https://41-10-31-21.vercel.app/)

## やったこと

```
$ npx create-next-app 41-10-31-21 --use-yarn --example "https://github.com/vercel/next-learn-starter/tree/master/basics-final"
```

This is a starter template for [Learn Next.js](https://nextjs.org/learn).

## markdown 編集時に hot reload するために

Next.js が監視している範囲外の `posts` も監視対象にするために以下のモジュールを使っている。

[hashicorp/next-remote-watch: Decorated local server for next.js that enables reloads from remote data changes](https://github.com/hashicorp/next-remote-watch)

`"dev": "next dev"`

を

`"dev": "next-remote-watch ./posts"`

に変更している。
