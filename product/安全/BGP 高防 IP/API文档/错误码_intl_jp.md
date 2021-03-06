[//]: # (chinagitpath:XXXXX)

## 機能説明

返された結果のエラーコードは、ユーザーがクラウドAPIを呼び出した結果を示します。codeが0の場合、呼び出しは成功します。それ以外の場合、呼び出しは失敗します。呼び出しが失敗した場合、ユーザーはパブリックエラーコードリストに基づいてエラーの原因を特定し、対処することができます。
例：

```
{
    "code": 5100
}
```

## エラーコードリスト

<table>
   <tr>
      <td>エラーコード</td>
      <td>説明</td>
      <td>対処方法</td>
   </tr>
   <tr>
      <td>4000</td>
      <td>リクエストパラメータが不正です</td>
      <td>必要なパラメータが欠落しているか、パラメータ値のフォーマットが正しくありません。具体的なエラー情報については、エラーの説明messageフィールドを参照してください。</td>
   </tr>
   <tr>
      <td>4100</td>
      <td>身元認証失敗</td>
       <td>通常、署名の計算が正しくなければ、身元認証が失敗します。文書の「<a href="https://cloud.tencent.com/document/api/213/6984">署名方法</a>」の部分を参照してください。</td>
   </tr>
   <tr>
      <td>4101</td>
      <td>APIへの不正アクセス</td>
      <td>サブアカウントは、メインアカウントによるAPIへのアクセスを許可されていません。APIの権限を有効化するには、メインアカウントの管理者に連絡してください。</td>
   </tr>
   <tr>
      <td>4102</td>
      <td>リソースへの不正アクセス</td>
      <td>サブアカウントは、メインアカウントによる特定のリソースへのアクセスを許可されていません。リソースの権限を有効化するには、メインアカウントの管理者に連絡してください。</td>
   </tr>
   <tr>
      <td>4103</td>
      <td>現在のAPIによって操作されているリソースへの不正アクセス</td>
      <td>サブアカウントは、APIによって操作されている特定のリソースにアクセスすることをメインアカウントによって許可されていません。リソースの権限を有効化するには、メインアカウントの管理者に連絡してください。</td>
   </tr>
   <tr>
      <td>4104</td>
      <td>暗号鍵が存在しない</td>
      <td>リクエストに使用された暗号鍵が存在しません。確認して再試行してください。</td>
   </tr>
   <tr>
      <td>4105</td>
      <td>tokenエラー</td>
      <td>tokenエラー。</td>
   </tr>
   <tr>
      <td>4106</td>
      <td>MFA検証失敗</td>
      <td>MFA検証失敗。</td>
   </tr>
   <tr>
      <td>4110</td>
      <td>他のCAM認証失敗</td>
      <td>他のCAM認証失敗。</td>
   </tr>
   <tr>
      <td>4300</td>
      <td>アクセス拒否</td>
      <td>アカウントがブロックされているか、APIの対応ユーザー範囲外です。</td>
   </tr>
   <tr>
      <td>4400</td>
      <td>割り当て量を超えた</td>
      <td>リクエスト数が割り当て量の制限を超えました。文書の「リクエスト割り当て量」の部分を参照してください。</td>
   </tr>
   <tr>
      <td>4500</td>
      <td>リプレイ攻撃</td>
      <td>リクエストのNonceおよびTimestampパラメータは、各リクエストがサーバー側で一度だけ実行されるようにするために使用されます。したがって、今回のNonceを前回のと同じにすることも、TimestampをTencentサーバーの時間から5分以上離れることもできません。</td>
   </tr>
   <tr>
      <td>4600</td>
      <td>プロトコルがサポートされていない</td>
      <td>プロトコルがサポートされていません。現在のAPIはHTTPSプロトコルのみをサポートし、HTTPプロトコルをサポートしません。</td>
   </tr>
   <tr>
      <td>5000</td>
      <td>リソースが存在しない</td>
      <td>リソースIDに対応するインスタンスが存在しないか、インスタンスが返されたか、他のユーザーのリソースにアクセスしています。</td>
   </tr>
   <tr>
      <td>5100</td>
      <td>リソース操作失敗</td>
      <td>リソースの操作に失敗しました。詳細については、エラーの説明messageフィールドを参照してください。後で再試行しますか、カスタマーサービスに連絡してください。</td>
   </tr>
   <tr>
      <td>5200</td>
      <td>リソース購入失敗</td>
      <td>リソース購入失敗。インスタンス構成がサポートされないか、リソース不足などの可能性があります。</td>
   </tr>
   <tr>
      <td>5300</td>
      <td>残高不足</td>
      <td>ユーザーアカウントの残高が購入またはアップグレードを完了するのに不十分です。</td>
   </tr>
   <tr>
      <td>5400</td>
      <td>一部実行成功</td>
      <td>一括操作が一部の実行にのみ成功しました。詳細については、メソッドの戻り値を参照してください。</td>
   </tr>
   <tr>
      <td>5500</td>
      <td>ユーザー資格審査未通過</td>
      <td>ユーザーの資格審査に合格していませんので、リソースを購入できません。</td>
   </tr>
   <tr>
      <td>6000</td>
      <td>サーバー内部エラー</td>
      <td>サーバーに内部エラーが発生しました。後で再試行しますか、カスタマーサービスに連絡してください。</td>
   </tr>
   <tr>
      <td>6100</td>
      <td>バージョンがサポートされていない</td>
      <td>このAPIはこのバージョンではサポートされていないか、メンテナンス状態です。注意：このエラーが発生した場合、まずAPIのドメイン名が正しいかを確認してください。モジュールによってドメイン名が異なる場合があります。</td>
   </tr>
   <tr>
      <td>6200</td>
      <td>APIに一時的にアクセスできない</td>
      <td>現在APIはメンテナンス状態なので、後で再試行してください。</td>
   </tr>
</table>

