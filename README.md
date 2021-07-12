# Git超入門
<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**目次**

- 【Step1】VisualStudioCodeでGit操作 "Merge pull request"まで!
- 【Step2】恐怖のコンフリクトの対処法

<!-- END doctoc generated TOC please keep comment here to allow auto update -->


***
# 【Step1】WebARを作成しよう
マーカーベースのWebARを作成していきましょう。マーカーベースとはカメラで特定の画像を設定し、カメラがそれを認識するとARの内容が表示される仕組みです。今回のハンズオンでは、好きな画像を設定し、その画像をカメラで認識した時にテキストを表示するコードを作成します。

### ⑴初めに
1. 当ページの上部から当リポジトリをGitでクローン、またはDownloadZipしローカル上の任意フォルダで展開してください。<br/>
![image](https://user-images.githubusercontent.com/66664167/115134407-c2228b80-a04a-11eb-813e-7b6cd00414fd.png)

<br/>※展開後のディレクトリ例<br/>
　・クローンした場合：C:\workspace\miracleave\meetup\meet-webar<br/>
　・DownloadZIPした場合：C:\workspace\miracleave\meetup\meet-webar-main<br/>
![image](https://user-images.githubusercontent.com/66664167/115102750-f2552600-9f87-11eb-82c1-1f19312882c8.png)
<br/><br/>

### ⑵WebARの作成
Web上でARを可能とするには、Google社製model-viewerとMozilla社製A-frameがありますが、今回はA-frameを基に作っていきます。<br/>
1. 【Step1】の⑴でクローン、またはDownloadZIPで展開したパスを、WindowsのエクスプローラーまたはMacのFinderで開きます。

2. WebARのコードを記述するために、開いたフォルダ直下に以下のar-marker.htmlをテキストエディタで開いてください。

3. WebARには、テキストや画像そして3Dアニメーションの表示が可能ですが、今回はテキストを表示してみます。開いたar-marker.htmlに以下コードを張り付けて、保存してください。このコードはA-frameとar.jsのライブラリをスクリプトタグで読み込み、body部のa-sceneタグでARのコードを記述します。今回はマーカーベースのテキスト表示を行いますので、a-sceneタグ内にa-markerタグとa-textタグを使用します。
