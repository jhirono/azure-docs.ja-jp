---
title: Azure CLI サンプル スクリプト - 同じサブスクリプションのストレージ アカウントに VHD ファイルから管理ディスクを作成する | Microsoft Docs
description: Azure CLI サンプル スクリプト - 同じサブスクリプションのストレージ アカウントに VHD ファイルから管理ディスクを作成する
services: virtual-machines-linux
documentationcenter: storage
author: ramankumarlive
manager: kavithag
editor: tysonn
tags: azure-service-management
ms.assetid: ''
ms.service: virtual-machines-linux
ms.devlang: azurecli
ms.topic: sample
ms.tgt_pltfrm: vm-linux
ms.workload: infrastructure
ms.date: 05/19/2017
ms.author: ramankum
ms.custom: mvc
ms.openlocfilehash: 15a5e3e566b03f29f33c3f21aa6581a03b0abe2e
ms.sourcegitcommit: 8c3267c34fc46c681ea476fee87f5fb0bf858f9e
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/09/2018
ms.locfileid: "29851009"
---
# <a name="create-a-managed-disk-from-a-vhd-file-in-a-storage-account-in-the-same-subscription-with-cli"></a>CLI で同じサブスクリプションのストレージ アカウントに VHD ファイルから管理ディスクを作成する

このスクリプトは、同じサブスクリプションのストレージ アカウントに VHD ファイルから管理ディスクを作成します。 このスクリプトを使用して、特殊化された (汎用化/Sysprep されていない) VHD を管理対象 OS ディスクにインポートして仮想マシンを作成します。 または、このスクリプトを使用して、データ VHD を管理対象データ ディスクにインポートします。 


[!INCLUDE [sample-cli-install](../../../includes/sample-cli-install.md)]

[!INCLUDE [quickstarts-free-trial-note](../../../includes/quickstarts-free-trial-note.md)]

## <a name="sample-script"></a>サンプル スクリプト

[!code-azurecli[main](../../../cli_scripts/virtual-machine/create-managed-data-disks-from-vhd/create-managed-data-disks-from-vhd.sh "Create managed disk from VHD")]


## <a name="script-explanation"></a>スクリプトの説明

このスクリプトは、以下のコマンドを使って VHD から管理ディスクを作成します。 表内の各コマンドは、それぞれのドキュメントにリンクされています。

| コマンド | メモ |
|---|---|
| [az disk create](https://docs.microsoft.com/cli/azure/disk#az_disk_create) | 同じサブスクリプション内のストレージ アカウントに VHD の URI を使用して管理ディスクを作成する |

## <a name="next-steps"></a>次の手順

[管理ディスクを OS ディスクとして接続することで仮想マシンを作成する](./virtual-machines-linux-cli-sample-create-vm-from-managed-os-disks.md?toc=%2fcli%2fmodule%2ftoc.json)

Azure CLI の詳細については、[Azure CLI のドキュメント](https://docs.microsoft.com/cli/azure)のページをご覧ください。

その他の仮想マシンと管理ディスクの CLI サンプル スクリプトは、[Azure Linux VM のドキュメント](../../app-service/app-service-cli-samples.md?toc=%2fazure%2fvirtual-machines%2flinux%2ftoc.json)にあります。
