# Notion_x_Blog


![image](https://user-images.githubusercontent.com/79553411/207518036-223023e1-133a-421f-a86c-27ba7e225fcb.png)


このブログはGithub Actionsで定期的に**Notion Database**にAPIリクエストを送ってhtmlを生成しています．

またnpmパッケージの`notablog`を使ってAPIで得られたデータからhtmlを生成しています．

```bash
- run: npm i -g notablog
- run: notablog generate .
```

デプロイもGithub Actionsの`peaceiris/actions-gh-pages@v3` を用いて`gh-pages` ブランチにpushしてそれをGithub pagesでホストしています．

**Notablog**では./public内にhtmlが生成されるのでpublic内をpushする対象にすることで中身だけをpushしています．

## Usage 

使い方に関しては以下のリポジトリのREADMEを参照してください

https://github.com/dragonman225/notablog-starter
