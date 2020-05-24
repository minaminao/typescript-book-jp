# Husky

> Huskeyは、悪質なコミット、プッシュなどを防ぐことができます🐶!

コミットが行われる前に何らかのJavaScript/TypeScriptコードを実行したい場合は、huskyがそのためのツールです。

たとえば、huskyを使用して、ファイルが自動的によりきれいにフォーマットされるようにすることができます。手動でファイルをフォーマットしたかを心配する必要は二度とありません。代わりにコードの目的にフォーカスすることができます。セットアップの方法は以下の通りです：

* `npm install husky -D`
* `scripts`を`package.json`に追加します：

```javascript
    "precommit": "npm run prettier:write",
```

コードをコミットし、フォーマットの変更が必要があるときはいつでも、変更されたファイルが、git logに書き込まれます。あなたは下記のことが可能です:

* あなたのコードを既にpushしている場合は、単純に`pretty`というコメントでコミットしてください。
* コードをpushしていない場合は、最後のコミットをamendしてください。スーパーヒーローのように見えます。
