# SpamMailDetector

## 概要
「セキュリティエンジニアのための機械学習」という参考書を読み、Androutsopoulosらによって収集されたデ\
ータセットを用いて、迷惑メール検出器を作成した。

## 説明
・http://www.aueb.gr/users/ion/data/lingspam_public.tar.gz にあるデータセットを使用する。
・データセットの中にあるpartt?というサブディレクトリには、spmsga*.txという名の迷惑メールとそれ以外\\
の正当なメールのファイルがあるので、リストに分類する。
・分類器にLightGBMを用いてoptunaによるハイパーパラメータチューニングを行い、その結果を利用して分類\\
モデルを訓練する。
・訓練したモデルを使い、正解率と混同行列を表示している。
