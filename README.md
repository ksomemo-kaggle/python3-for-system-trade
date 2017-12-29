# 「Python3ではじめるシステムトレード：環境構築と売買戦略」パンローリング社、森谷博之著

## プログラムコードを変更しました。

### 変更の理由(2017年12月30日現在)
#### 2017年7月にＡ、Ｂに対する処置としての変更を行っています。
#### A.2017年5月、米国Yahoo Financeの一時APIによる株価のダウンロードサービスの停止に対する処置。
米国Yahoo Financeはその後、サービスを開始いたしますが、内容にその前との相違がございます。

1. 以前はOpen High Low Closeは株価分割の調整を行っていませんでしたが、今は行っています。  
2．Adj Closeは依然と同様に株価分割と配当の調整がされています。  

#### B.pandasのデータ選択処理のツールとしてのixの廃止に対する処置  

#### C.2017年12月ごろより米国Google FinanceのAPIによる株価ダウンロードサービスのパフォーマンスの不安定性に対する処置。

本プログラムコードはwindows10でのみ動作確認を行っています。  
12章以降のプログラムコードを動かすためにはCQGとパンローリングまたは日本取引所グループから購入したティックデータの両方が必要です。ただし、パンローリングの購入者限定ダウンロードサービスを用いて、サンプルデータがダウンロード可能です。

## 「Python3ではじめるシステムトレード」easy_installについて

p.26からeasy_installの解説があり、monthdeltaのインストールを推薦していますが、現状ではpipを用いた方が簡単にインストールできます。

$ pip install monthdelta==1.0b

## pandas-dataradeerのインストールについて

p.28ではpandas-datareaderのインストール方法の記述がありますが、こちらもpipを用いて簡単に行うことができます。

$ pip install pandas-datareader

## 第12章の先物トレード戦略のパフォーマンのバックテストを2016年、2017年に延長
pan12-2015_2017.ipynbのファイルに2015年から2017年までのバックテストの結果を載せています。

