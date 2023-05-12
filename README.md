# heart-failure-predict

このリポジトリには、心不全を予測するための機械学習モデルを示すJupyter Notebook (heart_failure_predict.ipynb) が含まれています。このノートブックでは、ランダムフォレストアルゴリズムを使用してモデルをトレーニングし、評価します。

# データセット
このプロジェクトで使用するデータセットは、2つのCSVファイル、train.csv と test.csv からなります。トレーニングデータセット (train.csv) には、以下のカラムが含まれています:

id: データエントリーのID
age: 患者の年齢
anaemia: 貧血の有無を示す (0 = いいえ, 1 = はい)
creatinine_phosphokinase: 血中のクレアチニンホスホキナーゼ酵素のレベル (mcg/L)
diabetes: 糖尿病の有無を示す (0 = いいえ, 1 = はい)
ejection_fraction: 心臓の収縮時に血液が心臓から排出される割合
high_blood_pressure: 高血圧の有無を示す (0 = いいえ, 1 = はい)
platelets: 血液中の血小板数 (kiloplatelets/mL)
serum_creatinine: 血液中の血清クレアチニンのレベル (mg/dL)
serum_sodium: 血液中の血清ナトリウムのレベル (mEq/L)
sex: 患者の性別 (0 = 女性, 1 = 男性)
smoking: 喫煙の有無を示す (0 = いいえ, 1 = はい)
time: 追跡期間 (日数)
target: 心不全のイベントが発生したかどうかを示す (0 = いいえ, 1 = はい)

# 使用方法
ノートブックを実行するには、次のライブラリが必要です:

pandas
scikit-learn
matplotlib

# 結果
ランダムフォレストをトレーニングした後、ノートブックではテストセットでモデルの性能を評価します。分類レポートと正解率がコンソールに出力されます:

              precision    recall  f1-score   support

           0       0.88      0.98      0.92       162
           1       0.80      0.42      0.55        38

    accuracy                           0.87       200
   macro avg       0.84      0.70      0.74       200
weighted avg       0.86      0.87      0.85       200

Accuracy: 0.87












