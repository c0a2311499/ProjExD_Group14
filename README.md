# こうかとん伝説（仮）
## 実行環境の必要条件
* python >= 3.10
* pygame >= 2.1

## ゲームの概要
* こうかとんを十字キーで操作しスペースキーでビームを発射、敵やその爆弾を打ち落としてスコアを稼いでいくゲームで、元あるこうかとん無双に機能を追加していくことでさらにゲーム感が増している。具体的にはこうかとんの体力や攻撃力、技を使うためのスキルポイントの追加、一定のスキルを取ることで挑戦可能なボス戦の追加、画面スクロールの追加をすることでゲーム感を増させている。このゲームはクリアを目指すというより、ハイスコアを目指すものである。

## ゲームの実装
### 共通基本機能
* 背景画像、こうかとん、こうかとんのビーム、敵のUFO、UFOの爆弾の描画
* こうかとんの各種スキルの実装
* スコアの描画

### 担当追加機能
* 画面の動き(担当：寺川　竣祐)：横スクロール、敵を右から表示させる機能の追加
* ライフゲージ（担当：川畑　しんのすけ）：こうかとんのライフゲージの追加
* ボス追加⓵（担当：濱口　莉奈）：通常画面からボス画面、ボス撃破後に通常画面への移動
* ボス追加⓶（担当：町田　拓斗）：ボスの性能を決めるクラスの作成
* ステータス変化（担当：萩原　颯人）：打ち落とした爆弾の色によって各種ステータスを変化

### ボス戦切り替え(担当 : 濱口莉奈)
* 1キーを押したときにボス戦に行くかどうかを確認するポップアップを表示。このときスコアが１００以上でないといけない。
* "Yes"を押したらボス戦の画面に切り替わり、"No"のときにゲームに戻る

### ToDo
- ポップアップを表示したときに画面で動いているゲームの一時停止
- フェードアウト処理
- YesやNoを選択したときに色を変える