---

copyright:years: 2017
lastupdated: "2017-08-07"

---

{:new_window: target="\_blank"}
{:shortdesc: .shortdesc}
{:screen: .screen}
{:codeblock: .codeblock}
{:pre: .pre}


# データ・バックアップ
{: #back_up}

以下の情報を読んで、{{site.data.keyword.iot_full}} のデータ・バックアップ・ストラテジーを確認してください。

## バックアップされるのはどのようなタイプのデータですか? 

{{site.data.keyword.iot_short_notm}} の現在のストラテジーでは、以下のタイプのクライアント・データがバックアップされます。

- 組織情報
- デバイス情報
- API キーとトークン
- ユーザー情報
- デバイス管理要求のすべてのレコード (開始された要求の履歴や要求の現在の状態など)
- カスタム・デバイス管理要求バンドルの定義

## バックアップされないのはどのようなタイプのデータですか? 

{{site.data.keyword.iot_short_notm}} では、以下のタイプのデータはバックアップされません。

- デバイス・イベント
- メッセージの一時的な状態 (処理中のデータなど)
- 分析のルールやアラートの構成
- デバイス管理要求で送受信された MQTT メッセージ

## データ・バックアップの頻度と保管場所は?

データ・バックアップの頻度は 24 時間ごとです。

メインの {{site.data.keyword.iot_short_notm}} サービスのデータがオフサイトで保管されています。予備のデータを保管することによって、重大インシデントの発生時にサービスのリストアが可能になります。データのリストアが必要になった場合は、クライアントに連絡が入ります。全データが暗号化されており、該当する国や地域のデータ保護要件に準拠しています。

データ・バックアップのために現在使用されているオフサイト・ロケーションは以下のとおりです。

 ロケーション| バックアップ・ロケーション                      
------------- | -------------
Bluemix 米国南部 (ダラス)| ワシントン
Bluemix 英国 (ロンドン) | フランクフルト
Bluemix ドイツ (フランクフルト) | ロンドン
Bluemix Dedicated | {{site.data.keyword.iot_short_notm}} Dedicated 注文時のお客様の要請による

**注:** 今後、データ・プライバシーに関する法律に合わせてロケーションが変更されることもあります。例えば、EU から英国が離脱した場合にデータ主権のルールがどんな影響を受けるか、といったこともからんでくるかもしれません。
