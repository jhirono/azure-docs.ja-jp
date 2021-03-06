---
title: 要約 - Azure Functions とサーバーレス プラットフォームのセキュリティ
description: Azure Functions とサーバーレス プラットフォームのセキュリティに関するホワイト ペーパーの要約。
author: TomShinder
ms.author: TomSh
ms.date: 06/21/2018
ms.topic: article
ms.service: security
ms.openlocfilehash: 8f5f600b0680b85d760e72b8e177ae247e41ac6b
ms.sourcegitcommit: 5892c4e1fe65282929230abadf617c0be8953fd9
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/29/2018
ms.locfileid: "37133520"
---
# <a name="azure-functions-and-serverless-platform-security"></a>Azure Functions とサーバーレス プラットフォームのセキュリティ
## <a name="abstract"></a>要約
ほとんどの企業では、サーバーを管理するために多大なリソースと時間を必要とするため、追加のコストが発生します。 より少ないリソースを使用してサーバーを管理できれば、企業は優れたアプリケーションの構築に注力することができます。  

サーバーレス コンピューティングがその助けになります。アプリの実行とスケールのために必要なインフラストラクチャを、お客様の代わりにサーバーレス コンピューティングが管理するためです。 サーバーレス コンピューティングは、サーバー、インフラストラクチャ、オペレーティング システムを抽象化したものです。 サーバーレス コンピューティングは、すべてクラウド内でほぼリアルタイムで発生するイベントやトリガーに反応することで駆動されます。 

フル マネージド サービスのため、サーバー管理と容量計画は開発者には見えません。 サーバーレス フレームワークは、Azure Functions を使用してサーバーレス アプリケーションを開発およびデプロイするのに役立ちます。 これは、関数とイベントで構成された高度なイベント駆動型のサーバーレス アーキテクチャを構築するのに役立つ、構造と自動化を提供するコマンド ライン インターフェイス (CLI) です。 Azure 関数は、マイクロ サービスのように、デプロイの独立した単位です。 これはクラウドにデプロイされる単なるコードであり、ほとんどの場合は単一のジョブを実行するために記述します。

その利点にもかかわらず、サーバーレス セキュリティには独自のリスク要因があり、これに対処する必要があります。 サーバーレス アプローチでは、新たなセキュリティ上の懸念は生じませんが、既存のセキュリティ上の懸念へのアプローチが必要です。 このホワイト ペーパーでは、これらのセキュリティ上の問題に焦点を当てています。 
* サーバーレス プラットフォームの利点
* サーバーレス コンピューティングにおけるセキュリティの問題
* Azure のコンテキストにおける重大なセキュリティの問題と軽減策
* Microsoft サーバーレス プラットフォームのセキュリティ保護

[ホワイト ペーパーをダウンロードする](https://gallery.technet.microsoft.com/Azure-Functions-and-c6449f8d/file/202175/1/Microsoft%20Serverless%20Platform.pdf)

