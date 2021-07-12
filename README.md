

# Git超入門
<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**目次**

- 【Chapter 1】VisualStudioCodeでGit操作 "Merge pull request"まで!
- 【Chapter 2】コンフリクトの対処法について

<!-- END doctoc generated TOC please keep comment here to allow auto update -->


***
# 【Chapter 1】VisualStudioCodeでGit操作 "Merge pull request"まで!


### ⑴初めに


### ⑵

# 【Chapter 2】コンフリクトの対処法

### ⑴新規でブランチを作成
1.  VisualStudioCodeのブランチが表示されているところをクリックし、ブランチ作成
![スクリーンショット 2021-07-12 153032](https://user-images.githubusercontent.com/60914189/125241195-1ecdd380-e326-11eb-8cb0-1b67b4ce66ac.png)


ブランチ名は下記を入力
```
feature2
```
2. ブランチ名がfeature2になったのを確認しましたら再度index.htmlに修正を加えます。
![スクリーンショット 2021-07-12 154901](https://user-images.githubusercontent.com/60914189/125243198-baf8da00-e328-11eb-9ddb-20dcf51affc1.png)

### ⑵index.htmlを修正
1.ブランチ名がfeature2になっているのを確認。再度index.htmlに修正を加えます。

2.以下のソースをindex.htmlの31行目以降に挿入します。
挿入後上書き保存を行いローカルの修正を確認しましょう。
```
<h1>【Git入門】 コンフリクトを理解しよう</h1>
```
![スクリーンショット 2021-07-12 154425](https://user-images.githubusercontent.com/60914189/125242781-170f2e80-e328-11eb-9715-54c4ad45b955.png)

### ⑶コンフリクトを起こしてみる
1.ここでコンフリクトを発生させるためにindex.htmlをGitHub上で直接編集したいと思います。
<br>GitHubを開き、index.htmlをクリックして下さい。

![スクリーンショット 2021-07-12 155402](https://user-images.githubusercontent.com/60914189/125243758-79b4fa00-e329-11eb-8fd9-d94548675985.png)


2.index.htmlが表示されましたら右上のペンのマークの”Edit this file”をクリックし編集できるようにします。
![スクリーンショット 2021-07-12 160724](https://user-images.githubusercontent.com/60914189/125245307-6145df00-e32b-11eb-9d05-840f8716644b.png)

3.先ほどと同じ32行目に以下の文言を追加します。
```
<h1>【Git入門】 コンフリクトは注意が必要です。</h1>
```
![スクリーンショット 2021-07-12 160928](https://user-images.githubusercontent.com/60914189/125245491-981bf500-e32b-11eb-8935-7094f250cd2c.png)

4.Commit changesをクリックし修正をコミットします。
![image](https://user-images.githubusercontent.com/60914189/125245636-c568a300-e32b-11eb-9fa2-2d500df566d1.png)

5.Vscodeに戻り、先ほどの修正をpullしてみましょう。

ソースを保存した状態で左側メニューの＋マークをクリックし修正をステージにあげます。
![スクリーンショット 2021-07-12 160928](https://user-images.githubusercontent.com/60914189/125245809-f8129b80-e32b-11eb-826c-730a0720ffb7.png)


### ⑷コンフリクトの対処について
