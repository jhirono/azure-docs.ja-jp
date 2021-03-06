---
title: クイック スタート - Azure SignalR サービス REST API | Microsoft Docs
description: Azure SignalR サービスの REST API を使用するためのクイック スタート。
services: signalr
documentationcenter: ''
author: sffamily
manager: cfowler
editor: ''
ms.assetid: ''
ms.service: signalr
ms.devlang: dotnet
ms.topic: quickstart
ms.tgt_pltfrm: ASP.NET
ms.workload: tbd
ms.date: 06/13/2018
ms.author: zhshang
ms.openlocfilehash: 36fb87d3255149c041c4288d13c54eaff8425e06
ms.sourcegitcommit: f6050791e910c22bd3c749c6d0f09b1ba8fccf0c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/25/2018
ms.locfileid: "50024353"
---
# <a name="quickstart-broadcast-real-time-messages-from-console-app"></a>クイック スタート: コンソール アプリからのリアルタイム メッセージのブロードキャスト

Azure SignalR サービスは、ブロードキャストなどのサーバーとクライアントの間の通信シナリオをサポートする [REST API](https://github.com/Azure/azure-signalr/blob/dev/docs/rest-api.md) を提供します。 REST API 呼び出しが可能な任意のプログラミング言語を選択できます。 接続されているすべてのクライアント、名前を指定したクライアント、またはクライアントのグループにメッセージを投稿することができます。

このクイック スタートでは、コマンド ライン アプリから接続されたクライアント アプリに C# でメッセージを送信する方法について学習します。

## <a name="prerequisites"></a>前提条件

このクイック スタートは、macOS、Windows、または Linux で実行できます。
* [.NET コア SDK](https://www.microsoft.com/net/download/core)
* 任意のテキスト エディターまたはコード エディター。


[!INCLUDE [quickstarts-free-trial-note](../../includes/quickstarts-free-trial-note.md)]


## <a name="sign-in-to-azure"></a>Azure へのサインイン

Azure アカウントで Azure Portal (<https://portal.azure.com/>) にサインインします。


[!INCLUDE [Create instance](includes/signalr-quickstart-create-instance.md)]

## <a name="clone-the-sample-application"></a>サンプル アプリケーションの複製

サービスのデプロイ中、コードの作成に切り替えましょう。 [GitHub からサンプル アプリ](https://github.com/aspnet/AzureSignalR-samples.git)を複製し、SignalR Service 接続文字列を設定し、アプリケーションをローカルで実行します。

1. git ターミナル ウィンドウを開きます。 サンプル プロジェクトを複製するフォルダーに移動します。

1. 次のコマンドを実行して、サンプル レポジトリを複製します。 このコマンドは、コンピューター上にサンプル アプリのコピーを作成します。

    ```bash
    git clone https://github.com/aspnet/AzureSignalR-samples.git
    ```

## <a name="build-and-run-the-sample"></a>サンプルのビルドと実行

このサンプルは、Azure SignalR サービスの使用方法を示すコンソール アプリです。 これには次の 2 つのモードがあります。

- サーバー モード: 単純なコマンドを使用して、Azure SignalR サービスの REST API を呼び出します。
- クライアント モード: Azure SignalR サービスに接続し、サーバーからメッセージを受信します。

また、Azure SignalR サービスで認証するアクセス トークンを生成する方法も記載されています。

### <a name="build-the-executable-file"></a>実行可能ファイルの作成

例として MacOS の osx.10.13 x64 を使用します。 他のプラットフォームで作成する方法については、[こちらを参照](https://docs.microsoft.com/dotnet/core/rid-catalog)してください。
```bash
cd AzureSignalR-samples/samples/Serverless/

dotnet publish -c Release -r osx.10.13-x64
```

### <a name="start-a-client"></a>クライアントを起動する

```bash
cd bin/Release/netcoreapp2.1/osx.10.13-x64/

Serverless client <ClientName> -c "<ConnectionString>" -h <HubName>
```

### <a name="start-a-server"></a>サーバーを起動する

```bash
cd bin/Release/netcoreapp2.1/osx.10.13-x64/

Serverless server -c "<ConnectionString>" -h <HubName>
```

## <a name="run-the-sample-without-publishing"></a>公開せずにサンプルを実行する

次のコマンドを実行して、サーバーまたはクライアントを開始することもできます

```bash
# Start a server
dotnet run -- server -c "<ConnectionString>" -h <HubName>

# Start a client
dotnet run -- client <ClientName> -c "<ConnectionString>" -h <HubName>
```

### <a name="use-user-secrets-to-specify-connection-string"></a>user-secrets を使用して接続文字列を指定する

サンプルのルート ディレクトリで`dotnet user-secrets set Azure:SignalR:ConnectionString "<ConnectionString>"`を実行することができます。 その後は、`-c "<ConnectionString>"` オプションが不要になります。

## <a name="usage"></a>使用法

サーバーが起動した後、コマンドを使用してメッセージを送信します

```
send user <User Id>
send users <User List>
send group <Group Name>
send groups <Group List>
broadcast
```

別のクライアント名を持つ複数のクライアントを開始できます。

## <a name="usage"> </a> サード パーティ サービスとの統合
Azure SignalR サービスを使用すると、サードパーティのサービスをシステムに統合することができます。
### <a name="usage"> </a> 技術仕様の定義
以下の表は、現段階でサポートされている全バージョンの REST API を示したものです。 特定のバージョンごとの定義ファイルも記載しています。

Version | API 状態 | Door | 固有
--- | --- | --- | ---
`1.0-preview` | 使用可能 | 5002 | [Swagger](https://github.com/Azure/azure-signalr/tree/dev/docs/swagger/v1-preview.json)
`1.0` | 使用可能 | 標準 | [Swagger](https://github.com/Azure/azure-signalr/tree/dev/docs/swagger/v1.json)

以下に示したのは、特定のバージョンごとに利用可能な API の一覧です。

API | `1.0-preview` | `1.0`
--- | --- | ---
[全員にブロードキャストする](#broadcast) | :heavy_check_mark: | :heavy_check_mark:
[グループにブロードキャストする](#broadcast-group) | :heavy_check_mark: | :heavy_check_mark:
一部のグループにブロードキャストする | :heavy_check_mark: (非推奨) | `N / A`
[特定のユーザーに送信する](#send-user) | :heavy_check_mark: | :heavy_check_mark:
一部のユーザーに送信する | :heavy_check_mark: (非推奨) | `N / A`
[ユーザーをグループに追加する](#add-user-to-group) | `N / A` | :heavy_check_mark:
[ユーザーをグループから削除する](#remove-user-from-group) | `N / A` | :heavy_check_mark:

<a name="broadcast"> </a>
### <a name="broadcast-to-everyone"></a>全員にブロードキャストする
Version | API HTTP メソッド | 要求 URL | 要求本文
--- | --- | --- | ---
`1.0-preview` | `POST` | `https://<instance-name>.service.signalr.net:5002/api/v1-preview/hub/<hub-name>` | `{"target": "<method-name>", "arguments": [...]}`
`1.0` | `POST` | `https://<instance-name>.service.signalr.net/api/v1/hubs/<hub-name>` | 同上

<a name="broadcast-group"> </a>
### <a name="broadcast-to-a-group"></a>グループにブロードキャストする
Version | API HTTP メソッド | 要求 URL | 要求本文
--- | --- | --- | ---
`1.0-preview` | `POST` | `https://<instance-name>.service.signalr.net:5002/api/v1-preview/hub/<hub-name>/group/<group-name>` | `{"target": "<method-name>", "arguments": [...]}`
`1.0` | `POST` | `https://<instance-name>.service.signalr.net/api/v1/hubs/<hub-name>/groups/<group-name>` | 同上

<a name="send-user"> </a>
### <a name="sending-to-specific-users"></a>特定のユーザーに送信する
Version | API HTTP メソッド | 要求 URL | 要求本文
--- | --- | --- | ---
`1.0-preview` | `POST` | `https://<instance-name>.service.signalr.net:5002/api/v1-preview/hub/<hub-name>/user/<user-id>` | `{"target": "<method-name>", "arguments": [...]}`
`1.0` | `POST` | `https://<instance-name>.service.signalr.net/api/v1/hubs/<hub-name>/users/<user-id>` | 同上

<a name="add-user-to-group"> </a>
### <a name="adding-a-user-to-a-group"></a>ユーザーをグループに追加する
Version | API HTTP メソッド | 要求 URL
--- | --- | ---
`1.0` | `PUT` | `https://<instance-name>.service.signalr.net/api/v1/hubs/<hub-name>/groups/<group-name>/users/<userid>`

<a name="remove-user-from-group"> </a>
### <a name="removing-a-user-from-a-group"></a>ユーザーをグループから削除する
Version | API HTTP メソッド | 要求 URL
--- | --- | ---
`1.0` | `DELETE` | `https://<instance-name>.service.signalr.net/api/v1/hubs/<hub-name>/groups/<group-name>/users/<userid>`

[!INCLUDE [Cleanup](includes/signalr-quickstart-cleanup.md)]
