
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
VisualStudioCodeのブランチが表示されているところをクリックし、ブランチ作成
![スクリーンショット 2021-07-12 153032](https://user-images.githubusercontent.com/60914189/125241195-1ecdd380-e326-11eb-8cb0-1b67b4ce66ac.png)


ブランチ名は下記を入力
```
feature2
```
ブランチ名がfeature2になったのを確認しましたら再度index.htmlに修正を加えます。
![image](https://user-images.githubusercontent.com/60914189/125241827-ea0e4c00-e326-11eb-800b-2ae6bb62dbae.png)

### ⑵index.htmlを修正
ブランチ名がfeature2になったのを確認しましたら再度index.htmlに修正を加えます。
![スクリーンショット 2021-07-12 154339](https://user-images.githubusercontent.com/60914189/125242646-f2b35200-e327-11eb-8774-517e1e9a2fb6.png)



以下のソースをindex.htmlの31行目以降に挿入します。
挿入後上書き保存を行いローカルの修正を確認しましょう。
```
<h1>【Git入門】 コンフリクトを理解しよう</h1>
```
![スクリーンショット 2021-07-12 154425](https://user-images.githubusercontent.com/60914189/125242781-170f2e80-e328-11eb-9715-54c4ad45b955.png)

### ⑶コンフリクトを起こしてみる
