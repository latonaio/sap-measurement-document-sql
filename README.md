# sap-measurement-document-sql
sap-measurement-document-sql は、主にエッジアプリケーションにおいて、SAPと連携された 計測伝票データ を保存するSQLテーブルを作成するためのレポジトリです。  
sap-measurement-document-sql は、そのままクラウド環境におけるアプリケーションにも、適用可能です。  

## 前提条件  
sap-measurement-document-sql は、SQL の SAP とのデータ連携にあたり、オンプレミス版である（＝クラウド版ではない）SAPS4HANA API の利用を前提としています。クラウド版APIを利用する場合は、ご注意ください。  
https://api.sap.com/api/OP_API_MEASUREMENTDOCUMENT_0001/overview  
本レポジトリ の sql設定ファイルの内容は、上記URL の API 仕様を前提としています。  

## sqlの設定ファイル
sap-measurement-document-sql には、sqlの設定ファイルとして、sqlの設定ファイルとして以下のsqlファイルが含まれています。  

* sap-measurement-document-sql-header-data.sql（SAP 計測伝票 - ヘッダ）

## MySQLのセットアップ / Kubernetesの設定 / SQLテーブルの作成方法
MySQLのセットアップ / Kubernetesの設定 / 具体的なSQLテーブルの作成方法、については、[mysql-kube](https://github.com/latonaio/mysql-kube)を参照ください。