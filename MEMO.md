# Netlify


# overview  
githubにpushしたらdeployされる仕組みをつくる時。

参考：[https://note.com/koushikagawa/n/nba1b6990649c](https://note.com/koushikagawa/n/nba1b6990649c)  

端末：imac

local：Desktop/homework/210502_netlify_vue/git/netlify-vue  

プロジェクト名 ：netlify-vue

完成（30分弱）：[https://vigorous-noyce-585208.netlify.app/](https://modest-brattain-0613c9.netlify.app/)  

masterにpushしたら自動でデプロイされる仕組みになる

## vue

nodeのバージョンを変更する

`npm install -g @vue/cli`

`vue create project-name`

`cd my-project`

`npm run serve`

→ [http://localhost:8081/](http://localhost:8081/)  

## github

new repository

```markdown
注意点：gitの名前の設定を忘れないこと

git config user.name "ying"  
git config user.email "yayoi.5677@gmail.com"
```

書いてある通りに実行（masterに反映）
```markdown
例）
echo "# newrepository" >> README.md
git init
git add .
git commit -m "first commit"
git remote add origin https://github.com/KoushiKagawa/newrepository.git
git push -u origin master
```

## netlify

New site from Git

github

```markdown
例）
Branch to deploy：master
Build command：npm run build
Publish directory：dist
```

## 感想
かなり簡単。vue-cliを使えるようになれば色々実験できる

## vue-cliでsassを使う方法
sass-loader node-sassを入れる

`<style>`に`lang="scss"` を追記