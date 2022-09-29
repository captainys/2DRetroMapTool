# 2D Retro Game Map Stitching Tool
# 二次元レトロゲーム マップ貼り合わせツール


    作者連絡先:     PEB01130@nifty.com
    作者Webサイト:  http://www.ysflight.com
    取り扱い種別:   フリー
    ソースコード:   BSDライセンスでフリー
    動作環境:       Windows, Mac, Linux (それぞれ対応パッケージをダウンロードしてください)

---

    Author:      CaptainYS (PEB01130@nifty.com)
    Web Site:    http://www.ysflight.com
    License:     Free
    Source Code: Open Source, BSD License
    Platform:    Windows, macOS, Linux (Please download a package for your platform.)

---

# 注意 (重要!)
このプログラムを使うと、レトロ(レトロじゃなくてもいいけど)二次元ゲームの原寸大マップを作製できる。例えば、自分で攻略サイトを立ち上げたいような場合に使える。とくに、マイナー過ぎてまだ誰も攻略サイト作ってないようなゲームの攻略サイトを作ると価値が高いかもしれない。

ただし、このプログラムのデータ形式 (.retromap形式)ファイルは、公開しない方がいい。もしも、自分で攻略サイトを立ち上げたいような場合は、完成品のマップをPNG形式の画像ファイルに出力したものをアップロードした方がいい。

このプログラムのデータ形式 (.retromap形式)は、スクリーンショットのPNGファイルの情報をそのまま記録する。トリムしても、あとからトリム範囲を広げられるように、元データを残したままにしている。

実はこのプログラム、ゲームのマップ作るだけかと思ったら、案外実用的な利用方法もあって、スクロールしないと全部が見えないWebサイトのスクリーンショットをつなげて一枚のPNGファイルにする、なんていうことができる。たまにPDFでセーブすると配置が崩れるとか、絵が消えるとか、そういう心配がない。

しかし、そのスクリーンショットには、他人に見てほしくない情報まで写りこんでいるかもしれない。企業秘密情報であったり、学生さんの成績情報とか漏洩するとリアルな人生がエンドになってしまうかもしれない。あるいは、他人に見てほしくないブックマークとか写りこんでしまって、突然、カミングアウトを余儀なくされたりするリスクがある。

それでなくてもスクリーンショットなので、このツールで作ったデータ(PNG形式でも)を公開するときは、細心の注意を払った方がいい。

このプログラムで作ったデータを公開した結果、大変なことになった、というような場合でも、作者は一切責任を負わないので、この点が了承できない場合は、使用を中止してください。

# Disclaimer!
This program saves a 1x1 scale bitmap of retro (not necessarily retro, but any 2-dimensional) Role-Playing Games.  You can start your game-solution site by using this program, if you choose to.

But, I STRONGLY RECOMMEND NOT TO POST MAP DATA IN ITS NATIVE DATA FORMAT (.retromap format).  Instead, this program can save maps as a large .PNG image.  If you want to post maps, I suggest to upload those .PNG format.  That way, the visitors can see the image without installing this program on their computers.

The reason is because the .retromap data format stores the original screenshots.  You can trim them in the program, but the original image is remaining in the data so that you can un-trim the screenshot later.  What if your screenshots are showing what you don't want other people see?

Actually, this program turned out to be practically useful.  When you want to make an image of a web site that you need to scroll down to see all contents, and print-to-PDF gives you a mess, you can take screenshots of the web site, and stitch them together in this program.

But, your web-site screenshot may include your bookmarks.  Bookmarks may leak important information.  If I end up leaking like grading information of my students, my real career will be at risk.  Or, you may end up exposing bookmarks that you wanted to keep to yourself.

You should pay extreme attention before making a screenshot public in general.

I won't be held responsible for any damage or career change or life-style change caused by this program.  Unless you can agree with this condition, please stop using this program immediately.

---
## はじめに
このプログラムは、ザナドゥ・コンプリート・コレクションに収録されているの、リバイバル・ザナドゥ2を自力クリアする、という極めて限られた目的のために作った。

攻略サイトを見ればいいじゃないって? 自力で作るのがいいんだよ。

アイディアは非常に単純で、スクリーンショットのマップ部分を切り抜いて、それを貼り合わせて、原寸大マップを作るというもの。だから、リバイバル・ザナドゥ2に限らず、二次元マップのレトロゲームで、WindowsまたはMacで動くものであれば利用可能なはず。iOSのPhoto Streamを利用すれば、iOSデバイス上のスクリーンショットをPCまたはMacにPNG形式ファイルとして送ることができるので、iOS上のゲームにも対応可能。

このプログラムを開発した時点では、まだザナドゥ・コンプリート・コレクションは、手元になく、日本に帰省していた同僚に回収してきてもらうところだったため、二年前に買ってきて積んであったドラゴン・スレイヤー・クロニクル収録のPC88用ザナドゥで機能を検証した。自分としては欲しいレベルの機能を実現できて、大成功だったので、そこで止めても良かったのだが、ザナドゥをクリアしたもんだから、ザナドゥ・シナリオ2もムラムラとクリアしたくなってきてしまったため、結局シナリオ2もこのツールでマップを作りながらクリアしてしまった。

Falcomのザナドゥが登場した当時、僕は、なぜかファミコンは無いのにFM7を持っていた。その冬、お年玉をかき集めて、FM77AVを買った。ただ、2ドライブモデルを買えなかったもんだから、シングルドライブのモデルを買った。そのとき、頼み込んでザナドゥをおまけにつけてもらった。既に、電波新聞社発行の「山下章のチャレンジRPG」を持っていた(記憶が前後してるから多分合ってると思うんだけど)僕は、ほとんど解答集とも言える、その本の情報をフォローしてクリアしたと記憶している。

その後、ザナドゥ・シナリオ2が出る、と聞いたとき、なんとしてもやりたかった。が、果たしてFM7/77AV版が出るだろうかというのが最大の不安だった。なんせ、富士通のFMシリーズは、他機種に比べて非常に優れた特徴をいくつも持っているにも関わらず、なぜかマイナーという運命を背負っていた。その伝統はのちに続くFM-TOWNSにも脈々と受け継がれる伝統だった。当時、話題のゲームは、PC88、X1用はまず間違いなく出るものの、FM7/77AV版は出ないもんだから、何度涙を飲んだことか。

しかし、Falcomは、やってくれた。予定通り、FM77AV版、ザナドゥ・シナリオ2は発売された。前作は、攻略本を見て解いてしまったから、シナリオ2は自力クリアを目指そう。と、思った僕だったが、ザナドゥ・シナリオ2の壁は当時の僕には高すぎた。結構頑張って進めていたのだが、事故が発生。大体レベル6をなんとか歩き回れる程度になったとき、ふと、魔が差した。Black Onyxを使って次のレベルをちょっと見てみたい。レベル6の最上段に上り、そこから唯一のBlack Onyxを使ってレベル7へ。レベル7最上段には、見慣れないブロックがあった。中に入ると何かあるのだろうか？思わず、スペースキーを押すのを止められなかった、その時！「ぶーん」。ディスクの駆動音。それは、レベル11に続くCaveだった。非情にもオートセーブされてゆく。Black OnyxもFire Crystalも残ってない。レベル7の反対側の塔から脱出を試みるもボスキャラ(Buzzati)に阻まれて脱出できない。

ユーザーディスクのバックアップは取ってなかった。というか、当時フロッピーディスクは貴重品で、小遣いでそんなにたくさん買えるものではなく、そもそも、シナリオ2を買ったことによって財布が薄くなっていた僕には、バックアップ用の予備のディスクを買う金は残っていなかった。財力でも、ザナドゥ・シナリオ2に負けた。

完全に詰んだ。自力クリアの志はもろくも崩れ去ってしまったのであった。

バックアップさえあったなら。もともと、カセットテープにプログラムを保存していた時代、長い時間をかけて打ち込んだプログラムがテープが伸びて消滅という悲劇を何度も経験して、今では三重にバックアップが無いと不安で夜も眠れなくなってしまったが、このときの悲劇も、僕のバックアップ癖にいくばくかの貢献をしていると思う。

さすがに最初からやりなおす気力無くして、ディスクダンプを見てキャラクターデータを書き換えて続行して、レベル11は、コンプティークだったかな？のおまけのダンジョンマップを見ながらクリアしたと記憶している。ちなみに、FM-7版ザナドゥ、ザナドゥ・シナリオ2のデータディスクにはチェックサムがあった。が、データ部分をバイト単位で合計した値をどこかに書いてあるだけだったようで、例えば、Daggerを一本買ってセーブして、ディスクを書き換えて、Daggerを0本にしてDragon Slayer 1本に変化させることができた。

時は流れて、高校に入ってFM-TOWNSに乗り換えてからは、久しくFalcomのゲームからは遠ざかっていた。が、1998年にピッツバーグに引っ越していた僕は、Windows用にリバイバル・ザナドゥなる復刻版が出たことを知る。思わず、海外発送で買っちゃった。買ったのは、確か博士候補試験終わってからだったと思うから、多分1999年の後半。方眼紙のノートを買ってきて、タワーマップを書きつつ、多分二周はしたと思う。何がうれしかったって、BGMのWAVが入ってたから、しばらくプログラミング中のBGMに使った。今でもたまに聞くし。ちなみに、リバイバル・ザナドゥは、Windows 10ではインストールできるものの、そのままではセーブができない。Windows XP互換モードで起動するとセーブはできるようになるものの、しばらく使っていると「リソースが足りない」と言って落ちる。どうやら現実的にはプレイ不能のようだ。

そんなザナドゥにどっぷりはまった当時ゲーム少年、現在ゲーム中年の僕は、一昨年、帰省したとき、ソフマップの中古屋でドラゴン・スレイヤー・クロニクルを見つける。なんか、ガラスのショーケースに入ってて、プレミアム扱いだった。最初は、いや、買ってはいかん、そんな無駄遣いはいかん。と、思ったのだが、東京滞在の最終日、ここで買わんでどうする、と、気が変わって大人買い。ただ、買ったまま、ピッツバーグに持って帰ってきて、一年ばかり本棚に積んであった。

アメリカなんかに住んでるもんだから、いまいち日本国内の情報が遅い僕は、その年の12月に、ザナドゥ・コンプリート・コレクションなるものが発売されたことを、その一年後まで知らなかった。見つけたのは、本当に偶然、11月中に、なんかゲームでも買おうか、と、Amazon.co.jpを物色している途中見つけたと記憶している。ザナドゥ・コンプリート・コレクション、なんとしても欲しい内容があった。それは、リバイバル・ザナドゥ2。初代ザナドゥのシステムで、シナリオ2ともマップが違うらしい。なんとしても、やってみたかったのだが、Windows用に復刻してくれないから、涙を飲んでいた。しかし、そのリバイバル2が収録されているらしい。

なんとしても欲しかったのだが、情報が遅かった影響で既に予約はとっくに終わっていて、転売品を高値で買うしかできなかったが、そんなことは問題ではない。(いや、でも、できれば復刻版を数量限定とか予約限定とかしないでくれると海外に住んでる者としてはありがたいんだけど)。Amazon.co.jpで買っちゃった。そして、同僚に回収してきてもらう。

が、自力クリアするためには、マップを書かなくてはならない。そのためには、スクリーンショットをトリムして貼り合わせればいい、というわけで、できたのがこのツール。

なお、ザナドゥ・リバイバル2は、その後、このマップツールを使って、無事クリア。キング・ドラゴンはゴジラみたいな格好に変化していた。その後、友達に勧められるがままに、iOS用クロノトリガーを始めて、これもこのツールを使ってクリアして、iOS用の2次元ゲームにも対応できることを確認した。マップを書きながら進むから、道に迷うことがほとんどなくて、結果的に短時間でクリアできたと思う。ただ、iOS用で悪評が高い「死の山」だけは、友達に勧められるままに、攻略情報を見たけど。

ひょっとしたら、こういうツールって、すでに誰か別の人が作ったのがあるかもね。でも、僕っていちいちサーチするのが面倒なんだよね。まあ、こんなプログラムがひとつぐらい増えたっていいじゃないの。

## Introduction
I originally wrote this program for a very specific purpose: clear a retro role-playing game called "Xanadu Revival 2" by Nihon Falcom.

Why don't I look at a game-solution or cheating site?  I rather want to explore myself.

The idea is so simple.  I take screenshots, trim, and stitch them together to make a 1x1 pixel-scale map.  Therefore, this program must work for other 2D games if you are able to take a screenshot in .PNG format.  This program works for iOS games because you can use Photo Stream to send screenshots to your PC as a PNG image.

When I wrote the basic functionalities of this program, I didn't have a package "Xanadu Complete Collection" that included the Windows port of Xanadu Revival 2.  I was waiting for a co-worker who was visiting Japan then and was picking up the package for me.  But, I had a different package called "Dragon Slayer Chronicles" which had a Windows ports of Xanadu and Xanadu Scenario 2.

By the way, if you haven't heard about Xanadu, it is a legend in a Japanese Retro Role-Playing Games.  That was when I was an 8th grade, so it must be around 1985.  Personal Computers were not popular at all.  It was rare to have a computer at home.  Many people were skeptical about computers or even saying computers were harmful without any scientific evidence.

In that circumstance, Xanadu Scenario 1 sold 0.4 million copies.  If you scale it up to the current market size, it would be a billion-hit.  I played through so many rounds hours and hours in the ruin of Xanadu.  Actually I ended up with purchasing three re-make versions.

Anyways, I dived into the ruin of Xanadu again to test this program.  It was very successful.  Even it gave me an idea of an assignment for my programming course.  It was enough to test this program before Revival 2, but I wanted to do the same with Scenario 2.  So I did, and it was very much fun.

When Falcom released Xanadu, I had an 8-bit computer called FM-7.  My parents didn't buy me a Nintendo Entertainment System (called Family Computer in Japan).  But, they purchased a computer.  By the way, FM-7 had two CPUs running simultaneously.  One CPU was in charge of graphics.  It was also possible to send custom program to the CPU that was mainly in charge of graphics to do general-purpose processing.  Yes, it was doing GPGPU in 1982.  It's nothing new.  Computer got faster.  Better managed.  But essentially it is the same.

In the following winter, I switched to an upgraded version called FM-77AV.  Xanadu was the first game I bought for 77AV, and that time I played through by looking at a cheating book.

Then Falcom developed Xanadu Scenario 2, and I really wanted to explore by myself.  But, I was young, fool, and inexperienced.  Xanadu Scenario 2 was too much for me.  I tried, but I was not good enough to save the world.  I had to use a cheating book to finish it.

Almost 30 years later, I found that a package of Xanadu re-make versions called "Xanadu Complete Collection" was available.  It included the last in the series "Xanadu Revival 2".  Revival 2 was only available for PC-9801, which I didn't have.  This was my veyr first opportunity to play Revival 2.

I was determined to finish it without looking at a cheating book or cheating site.  To do so, I need to be able to make a map.  Well, I am not young and fool anymore.  I can combat it with my programming.

So, I made this program and defeated King Dragon in Revival 2, which disfigured from the original and looked pretty like Godzilla.

Then, my friend suggested to play "Chrono Trigger" on iPhone.  I used this program to make maps, and finished it without looking at solutions.  Only solution I looked at was for "Death Mountain" because my friend told that it was unreasonably difficult to do it with touch UI.  I played through two rounds without looking at any other solution information.  After I finished two rounds I finally looked general solution sites to see if I played right or I was doing in a hard way.

Well, maybe someone else has already written something similar.  But, what's wrong with adding one?


---

## ビルド方法
作業ディレクトリで、次のコマンドを実行。
1) git clone https://github.com/captainys/2DRetroMapTool.git
2) git clone https://github.com/captainys/public.git
3) cd 2DRetroMapTool
4) mkdir build
5) cd build
6) cmake ../src
7) cmake --build . --config Release --target 2DRetroMapTool --parallel

## Build Instruction
In the working directory:
1) git clone https://github.com/captainys/2DRetroMapTool.git
2) git clone https://github.com/captainys/public.git
3) cd 2DRetroMapTool
4) mkdir build
5) cd build
6) cmake ../src
7) cmake --build . --config Release --target 2DRetroMapTool --parallel


---

## 効能
2次元ゲームのスクリーンショットから原寸大マップ作成。

PDFにプリントすると崩れてしまうWebサイトを、8割ぐらいずつスクロールしながらスクリーンショットを撮ってつなぎ合わせて一枚の巨大なビットマップにする。

Google Mapとかのスクリーンショットを撮りたいが、入れたい範囲をすべてカバーするまで引くと肝心の地名が消えてしまうような場合、ズームした状態でちょっとずつずらしながらスクリーンショットを撮ってつなぎあわせて一枚のビットマップにする。


## What this program can do
Creating a 1x1 scale map of a 2D game.

When you want to save a web site but saving to PDF breaks the layout, you can take multiple screenshots of the web site and stitch them together to make a bitmap of the web site.

When you want to take a screenshot of Google map, but the street names disappear if you unzoom to have all you want in one window, you can zoom in and take multiple screenshots and stitch them together to make a large bitmap of the map.

---

## インストール
このファイルを適当な場所に展開するだけです。アンインストール時はファイルを削除してくださ。

## Install
Just expand files to wherever you want.  There is no installer.  You can just delete the files to uninstall.

---

## 起動方法
Windows用    bin/2DRetroMapTool.exe をダブルクリック
macOS用      bin/2DRetroMapTool.app をダブルクリック
Linux用      bin/2DRetroMapTool.app/Contents/Resources/2DRetroMapTool を起動

## Starting the Program
In Windows    Double click bin/2DRetroMapTool.exe
In macOS      Double click bin/2DRetroMapTool.app
In Linux      Start bin/2DRetroMapTool.app/Contents/Resources/2DRetroMapTool

---

## 初回起動時にすること

このプログラムでできることは、手間をかければ普通のペイントツールでもできる。新しいスクリーンショットを開いて、それを巨大ビットマップに次々に貼り付けて行けばいいだけ。しかし、普通のペイントツールでそれを実行しようとすると、新しいスクリーンショットをファイルセレクタで読み込んで、トリムするだけでも手間がかかって、やる気をくじかれてしまう。このツールが違うのは、ボタン一発で新しいスクリーンショットを読み込むことができて、それをマウスなりタッチなりでずるずると移動して張り合わせることができるという点。逆に、ボタン一発で新しいスクリーンショットを読み込むのでなければ、価値が半減すると言っていい。

デフォルトでは、~/Dropbox/Screenshots, ~/OneDrive/Pictures/Screenshots, ~/Desktop がスクリーンショット保存ディレクトリとして設定されていまる。Windowsでは、あらかじめ、このどちらかにスクリーンショットが保存されるようにシステムの設定を変更しておく必要がある。

もしも、このデフォルトの場所以外にスクリーンショットが発生するようであれば、[設定]->[設定]を選んで、場所を指定する必要がある。例えば、ドラゴンスレイヤー・クロニクルとか、ザナドゥ・コンプリート・コレクションのような、エミュレータベースのプログラムの場合、ウィンドウのスクリーンショットだと拡大がかかっている場合があって、ピクセル単位で微妙に色が違うことがある。そういう場合は、エミュレータのスクリーンショット機能を使う方が良くて、その機能を使って作ったビットマップを貼り合わせるのであれば、エミュレータが出力するスクリーンショットディレクトリを、このプログラムにも登録しておく必要がある。

また、問題は、iOS。iOSで、Photo Streamを使ってiCloud経由でスクリーンショットを同期すると、たとえば、iPhone5Sのスクリーンショットは、

    ~/Pictures/fromIPhone5S.photoslibrary/Masters

このディレクトリの、サブディレクトリのサブディレクトリ内に発生する。(ひとつのアカウントにふたつ以上の同じ機種があったらどうなるんだろう？)。

Photo Streamのスクリーンショットをボタン一発で読み込むように設定するには、[設定]→[設定]を選んで、使う機種用のMastersディレクトリをスクリーンショットフォルダに追加して、右の[Sub-Folder]をチェックする。Photo Streamだと、ときどき長いことシンクロナイズされなくて、スクリーンショットがPCに入ってこないことがあるけど、そこは忍耐力で我慢する。

## Initial Set Up
What this program can do also can be done in any other picture-processing programs if you are patient.  The point of this program is that this program remembers files in the screenshot directory, and can import a new screenshot to your map with just one push of button.  The program makes a file list every time you start a program, so you need to make sure the program is up while you are playing a game.  (If you missed, you can still manually select a file in your screenshot directory.)

So, what's important is to tell the location of your screenshot directory to this program.  By default ~/Dropbox/Screenshots, ~/OneDrive/Pictures/Screenshots, ~/Desktop are selected as a screenshot directory.  If you are using Windows, make sure to set up Windows so that it stores a new screenshot in .PNG format in one of the two directories.

If a screenshot is created in a non-default location, you need to select [Config]->[Config] and specify the screenshot directory.  It is particularly important if you are playing an emulator-based retro games.  The window size of those games may be different from the original resolution, and the image may be stretched to show in a larger window.  In such a case, the emulator may have its own screenshot-taking function that gives the original-resolution image, which is much better for the purpose of making a 1x1 map.  You should specify the screenshot directory of the emulator.

iOS games might be a bit tricky.  I figured that if I synchronize screenshot via iCloud Photo Stream, the images are created in a sub-directory of:
    ~/Pictures/fromIPhone5S.photoslibrary/Masters
(What's going to happen if I have two iPhone5S on my account?)

To read a new screenshot from the Photo Stream with one push of button, you should add this directory in [Config]->[Config].  Also make sure to check [Sub-Folder].  Unless this box is checked the program won't look into sub-folders.

---

## 基本操作
通常モード:

    スクロール:    Shift+左ボタンドラッグ、または、二本指タッチ(タッチパネルのみ)
    ボックス選択:  左ボタンを押して、領域を選んでボタンを放す。
    単一選択:      左ボタンで選びたいものをクリック。
    選択追加/解除: Control+左ボタンクリック
    削除:          Deleteキー
    移動:          選択したものの上で左ボタンをクリックしてドラッグ。

## Basic Operations
Normal Mode:

    Scrolling:  Left-Button drag while press and holding a Shift key.  Or, two-finger touch (if it comes with a touch screen)
    Box Selection:  Left-button drag.
    Single Selection:  Left-button click.
    Add/Remove Selection:  Click on an item while the Control key is held down.
    Deletion:    Delete key or [Edit]->[Delete]
    Move:  Click on the selected item and drag.

---

## コントロールダイアログの操作
    上段左: フィールドの選択。
    矢印: 画面のスクロール
    画像を追加: ファイルダイアログで選んで画像を追加。
    違いをハイライト: チェックしておくと、選択した画像を移動するとき他の画像と重なる部分の違いをハイライト。複数選択時は最初の数枚のみ。
    Threshold: 違いをハイライトするとき、どのぐらい明るさが違うピクセルを違うと認識するかの閾値。
    新しいスクリーンショットを追加: あらかじめ登録したスクリーンショットディレクトリに新たに発生したスクリーンショットを一枚追加。
    コメントを追加: テキストコメントを追加。なお、複数行にするときは \n を入れると改行できる。
    位置微調整: 大雑把に位置あわせした後、最後の数ピクセルを、エラーが最小になるように微調整する。


## Control Dialog
    Top-Left:    Field selection.
    Arrows:     Scroll screen.
    Add Image:     Add an image selected by a file dialog.
    Highlight Diff:     If this box is checked, difference between the selected images and the other image will be highlighted.  If you have multiple selection, only first a few will be highlighted.
    Threshold:     RGB intensity threshold for highlighting diff.
    Add New Screenshot:  Add a new screenshot taken in the pre-configured screenshot directory.
    Add Comment: Add text comment.  You can make a multi-line comment by inserting \n .
    Make Adjustment: After roughly place an image, this button will make small movement so that the diff (average per pixel) is minimized.

---

## フィールドとワールドについて
ゲームには、大概ステージがある。ひとつのステージ内のマップは連続しているが、違うステージに移動するとき、マップが切り替わったりする。このプログラムでは、ひとつのステージを「フィールド」という単位で管理する。

また、このフィールドを集めたもの、ゲーム全体を「ワールド」と呼ぶ。ひとつのデータファイルがひとつのワールドに対応する。ステージを変えるたびに、新しいデータファイルに切り替える必要は無い。(半面、メモリは食うけど)

それぞれのフィールド上には、スクリーンショットとマークアップを貼り付けることができる。スクリーンショットは、そのままゲームのスクリーンショット。マークアップには二種類あって、線(矢印可)と、テキストを貼り付けることができる。マップを作っている途中、手に入るアイテムとか、あるいは、ワープがあるとかいう場合、マークアップを使ってメモを書き込むことができる。

スクリーンショットを追加するには、基本的にゲーム上でスクリーンショットを撮って、メインダイアログの「新しいスクリーンショットを追加」ボタンをクリックする。追加したスクリーンショットはスクリーンショット上でマウス左ボタンを押してドラッグすることで移動できる。あるいは、選択状態で矢印キーを押しても移動できる。

また、スクリーンショット同士の位置合わせを容易にするために、[違いをハイライト]することができる。メインダイアログ上で、このチェックボックスをオンにしておくと(デフォルトオン)、スクリーンショット同士で重なり合う部分で、色が指定の閾値以上違う部分を赤くハイライトする。

## Field and World
A game usually has multiple stages.  In this program, a stage is a unit called a "Field".

A collection of the fields, or entire game, is called a “World”.  One data file (.retromap format file) stores one world.  Therefore, you don't have to close a file and open a new one again when you switch between fields.  (Down side is it eats more memory.)

On each field, you can paste screenshots and mark ups.  A screenshot is called "Map Piece" in this program.  There are two types of mark ups, (1) text and (2) drawing.  By using mark ups, you can add a memo like the item you can get at a particular location in your map.

If you have configured the system and this program right, you can insert a new screenshot just by clicking on "Insert New Screenshot" button.

Neighboring screenshots should overlap a little bit so that you can adjust the location.  To facilitate this, the program highlights differences on the overlapping part.

---

## スクリーンショットについて
ゲーム自体にスクリーンショット機能がある場合は、それを使った方がいい。とくにエミュレータベースのもの。

ゲームのスクリーンショットには、マップを表示している範囲と、ステータス表示の範囲がある。マップ作製には、ステータス表示の部分は不要なので、トリムする必要がある。トリム範囲は、スクリーンショットを読み込んで選んだ状態で、[編集]->[トリム]を選ぶことで指定可能。スクリーンショットの周囲に4本のハンドルを表示するので、それをマウスでつまんで、ドラッグして範囲を指定できる。

スクリーンショットの配置には、移動の最小単位(ピクセル数)を指定することができる。レトロゲームだと、マップは16ピクセルとか8ピクセル単位でスクロールするものが多い。8ピクセルでスクロールすればスムーズスクロールだったんだよ、当時は。ザナドゥなんかだと40ピクセル単位、だったかな？50だっけ？とにかく、そういう場合、1ピクセル単位でスクリーンショットを移動して張り合わせるのは効率が悪くて、移動の最小単位を指定しておくと楽に位置合わせができる。最小単位は、ワールドごとの設定で、[ワールド]->[単位の指定]で指定可能。

## About Screenshots
If the game has its own screenshot function, it is better to use it rather than the operating system's screenshot functionality in general.

Probably the game uses some part of the window for showing status.  Those part are not needed for mapping.  So, those parts must be trimmed.  You can trim an image by [Edit]->[Trim].  You'll see four fingers around the image.  You can pick them and drag them to change the range for trimming.

You probably need to trim the same region for the subsequent screenshots.  So, you have an option to apply same trimming to the all new incoming images.  Or, you can apply to the one you selected only, or to all existing screenshots on the same field.

You can also specify the minimum unit that the screenshots can move.  Many retro games scrolls the map 8 pixels at a time or even 40 pixels at a time.  Then, you really don't want to align your bitmaps on those unit boundaries.  The images should snap to those unit boundaries.  To do so, you can select [World]->[Set Unit] to specify the unit.


---

## エミュレータとの連携について

なお、FM TOWNSエミュレータ「津軽」とFM77AVエミュレータ「陸奥」のクイックスクリーンショット機能には、デバッガで解析してマップ座標を解明すれば、その座標をスクリーンショットのファイル名にエンコードして出力する機能がある。その機能を使うと、ファイル名に$X=16$Y=32のような文字列が含まれていた場合、このツール内で指定した単位に、(16,32)を掛けた値の位置に新しいスクリーンショットを配置する。

デバッガを使ってメモリのどこにマップ左上座標が書かれているかを解析する必要があるものの、成功すれば、Quick Screenshotを取るたびに、どんどんマップができていく。なお、停止した状態でスクリーンショットを取る必要あり。歩きながらスクリーンショットを取ると、プレイヤーキャラは移動したけどまだ画面が書き換わる前にスクリーンショットを撮ってしまう場合があって、そうすると座標がずれる。

この機能、他のエミュレータ作者さんも対応してくれるといいんだけどな。


## Coordination with an Emulator Software

FM TOWNS Emulator "Tsugaru" and FM77AV Emulator "Mutsu" has quick-screenshot command, which saves a screenshot to a pre-specified directory with auto-generated file name.  You need to use debugger to find where the map coordinate is written, this is a very useful functionality for making a map.  For example, if you enable this feature, the file name of the screenshot will include something like $X=16$Y=32, in which case this program will place a new screenshot at (16*ux,32*uy) where ux and uy are the unit you specify in this program.

It takes some skill to use a debugger to find the memory location of the map coordinate, but if you find it, just take quick-screenshot and the map will be populated automatically.  Oh, one thing to be careful is take screenshot when the player character is not moving.  If you take a screenshot while moving, the program may have moved the player character, but may not have re-drawn the map, then the map coordinate and the screenshot you get may be off by some pixels.

I with other emulator developers also support this functionality.



--- 

## 3次元化
なお、このユーザインターフェースは、3次元データを扱うツールを作るために作ったものなので、ビューコントロールダイアログの回転ロックを解除すると、Shift + 右ボタンドラッグで、マップを三次元的に回転することができる。

まったく意味ないけど。

## Making it 3D
It is totally a useless feature of this program.  But, the GUI framework is originally made for editing 3D objects.  By un-checking the orientation lock on the view-control dialog, you can rotate the map by Shift + Rightbutton drag.