---
title: 言語サポート - Translator Text API
titleSuffix: Azure Cognitive Services
description: Microsoft Translator Text API でサポートされる自然言語の一覧。
services: cognitive-services
author: Jann-Skotdal
manager: cgronlun
ms.service: cognitive-services
ms.component: translator-text
ms.topic: article
ms.date: 09/25/2018
ms.author: v-jansko
ms.openlocfilehash: 222e37e38772b82e9d9849e3a955b865d43d3c63
ms.sourcegitcommit: 5c00e98c0d825f7005cb0f07d62052aff0bc0ca8
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/24/2018
ms.locfileid: "49957396"
---
# <a name="language-and-region-support-for-the-translator-text-api"></a>Translator Text API の言語と地域のサポート

Translator Text API では、テキスト対テキストの翻訳について、以下の言語をサポートしています。 Neural Machine Translation (NMT) は、AI を使用する高品質機械翻訳の新しい標準で、ニューラル システムが使用できる場合に Translator Text API の V3 を使用して既定で提供されます。 "generalnn" カテゴリを使用する V2 のニューラル機械翻訳が使用可能です。

[機械翻訳の詳細](https://www.microsoft.com/translator/mt.aspx)

| Language    | 翻訳の種類 |言語コード |
|:----------- |:-------:|:-------------:|
| アフリカーンス語      | 統計 |`af`          |
| アラビア語      | ニューラル | `ar`          |
| アラビア語、レバント    | ニューラル | `apc`
| バングラ語      | ニューラル |`bn`          |
| ボスニア語 (ラテン)      | 統計 |`bs`          |
| ブルガリア語     |  ニューラル |`bg`          |
| 広東語 (繁体字)      | 統計 |`yue`          |
| カタルニア語      | 統計 |`ca`          |
| 中国語 (簡体字)        |  ニューラル |`zh-Hans`          |
| 中国語 (繁体字)        |  ニューラル |`zh-Hant`          |
| クロアチア語      | ニューラル |`hr`          |
| チェコ語        |  ニューラル |`cs`          |
| デンマーク語        |  ニューラル |`da`          |
| オランダ語        |  ニューラル |`nl`          |
| 英語       |  ニューラル |`en`          |
| エストニア語      | ニューラル |`et`          |
| フィジー語      | 統計 |`fj`          |
| フィリピン語      | 統計 |`fil`          |
| フィンランド語      | ニューラル |`fi`          |
| フランス語        |  ニューラル |`fr`          |
| ドイツ語       |  ニューラル |`de`          |
| ギリシャ語      | ニューラル |`el`          |
| ハイチ クレオール語      | 統計 |`ht`          |
| ヘブライ語      | ニューラル |`he`          |
| ヒンディー語        |  ニューラル |`hi`          |
| ミャオ語      | 統計 |`mww`          |
| ハンガリー語      | ニューラル |`hu`          |
| アイスランド語      |  ニューラル |`is`           |
| インドネシア語      | 統計 |`id`          |
| イタリア語        |  ニューラル |`it`          |
| 日本語        |  ニューラル |`ja`          |
| スワヒリ語      | 統計 |`sw`          |
| クリンゴン語      | 統計 |`tlh`          |
| クリンゴン語 (plqaD)      | 統計 |`tlh-Qaak`          |
| 韓国語        |  ニューラル |`ko`          |
| ラトビア語      | ニューラル |`lv`          |
| リトアニア語      | ニューラル |`lt`          |
| マダガスカル語      | 統計 |`mg`          |
| マレー語      | 統計 |`ms`          |
| マルタ人      | 統計 |`mt`          |
| ノルウェー語        |  ニューラル |`nb`          |
| ペルシャ語      | 統計 |`fa`          |
| ポーランド語        |  ニューラル |`pl`          |
| ポルトガル語        |  ニューラル |`pt`          |
| オトミ語      | 統計 |`otq`          |
| ルーマニア語        |  ニューラル |`ro`          |
| ロシア語        |  ニューラル |`ru`          |
| サモア語      | 統計 |`sm`          |
| セルビア語 (キリル文字)      | 統計 |`sr-Cyrl`          |
| セルビア語 (ラテン)      | 統計 |`sr-Latn`          |
| スロバキア語     | ニューラル |`sk`          |
| スロベニア語      | ニューラル |`sl`          |
| スペイン語        |  ニューラル |`es`          |
| スウェーデン語        |  ニューラル |`sv`          |
| タヒチ語      | 統計 |`ty`          |
| タミール語      | 統計 |`ta`          |
| テルグ語   | ニューラル   | `te` |
| タイ語      | ニューラル |`th`          |
| トンガ語      | 統計 |`to`          |
| トルコ語       |  ニューラル |`tr`          |
| ウクライナ語      | ニューラル |`uk`          |
| ウルドゥー語      | 統計 |`ur`          |
| ベトナム語      | ニューラル |`vi`          |
| ウェールズ語      | ニューラル |`cy`          |
| ユカテコ語      | 統計 |`yua`          |

## <a name="transliteration"></a>音訳

音訳メソッドは、以下の言語をサポートします。 "ソース言語/ターゲット言語"、"<-->" は、ソース言語あるいはターゲット言語、または記載されているスクリプトのどちらにも音訳できることを示しています。 "-->" は、言語が、あるスクリプトから一方向のみに音訳できることを示しています。

| Language    | 言語コード | スクリプト | ソース言語/ターゲット言語 | スクリプト|
|:----------- |:-------------:|:-------------:|:-------------:|:-------------:|
| アラビア語 | ar | アラビア語 | <--> | ラテン語 |
|バングラ語  | bn | ベンガル語 | <--> | ラテン語 |
| 中国語 (簡体字) | zh-Hans | 中国語 (簡体字) | <--> | ラテン語 |
| 中国語 (簡体字) | zh-Hans | 中国語 (簡体字) | <--> | 中国語 (繁体字) |
| 中国語 (繁体字) | zh-Hant | 中国語 (繁体字) | <--> | ラテン語 |
| 中国語 (繁体字) | zh-Hant | 中国語 (繁体字) | <--> | 中国語 (簡体字) |
| グジャラート語 | gu  | グジャラート語 | --> | ラテン語 |
| ヘブライ語 | he | ヘブライ語 | <--> | ラテン語 |
| ヒンディー語 | hi | デーヴァナーガリー | <--> | ラテン語 |
| 日本語 | ja | 日本語 | <--> | ラテン語 |
| カンナダ語 | kn | カンナダ語 | --> | ラテン語 |
| マラヤーラム語 | ml | マラヤーラム語 | --> | ラテン語 |
| マラーティー語 | mr | デーヴァナーガリー | --> | ラテン語 |
| オリヤー語 | or | オリヤー語 | <--> | ラテン語 |
| パンジャーブ語 | pa | グルムキー文字 | <--> | ラテン語  |
| セルビア語 (キリル文字) | sr-Cyrl | キリル文字  | --> | ラテン語 |
| セルビア語 (ラテン) | sr-Latn | ラテン語 | --> | キリル文字 |
| タミール語 | ta | タミール語 | --> | ラテン語 |
| テルグ語 | te | テルグ語 | --> | ラテン語 |
| タイ語 | th | タイ語 | <--> | ラテン語 |

## <a name="dictionary"></a>Dictionary

辞書では、Lookup および Examples メソッドを使用して、以下の言語と英語間で双方向の翻訳がサポートされています。

| Language    | 言語コード |
|:----------- |:-------------:|
| アフリカーンス語      | `af`          |
| アラビア語       | `ar`          |
| バングラ語      | `bn`          |
| ボスニア語 (ラテン)      | `bs`          |
| ブルガリア語      | `bg`          |
| カタルニア語      | `ca`          |
| 中国語 (簡体字)      | `zh-Hans`          |
| クロアチア語      | `hr`          |
| チェコ語      | `cs`          |
| デンマーク語      | `da`          |
| オランダ語      | `nl`          |
| エストニア語      | `et`          |
| フィンランド語      | `fi`          |
| フランス語      | `fr`          |
| ドイツ語      | `de`          |
| ギリシャ語      | `el`          |
| ハイチ クレオール語      | `ht`          |
| ヘブライ語      | `he`          |
| ヒンディー語      | `hi`          |
| ミャオ語      | `mww`          |
| ハンガリー語      | `hu`          |
| アイスランド語    | `is`  |
| インドネシア語      | `id`          |
| イタリア語      | `it`          |
| 日本語      | `ja`          |
| スワヒリ語      | `sw`          |
| クリンゴン語      | `tlh`          |
| 韓国語      | `ko`          |
| ラトビア語      | `lv`          |
| リトアニア語      | `lt`          |
| マレー語      | `ms`          |
| マルタ語      | `mt`          |
| ノルウェー語      | `nb`          |
| ペルシャ語      | `fa`          |
| ポーランド語      | `pl`          |
| ポルトガル語      | `pt`          |
| ルーマニア語      | `ro`          |
| ロシア語      | `ru`          |
| セルビア語 (ラテン)      | `sr-Latn`          |
| スロバキア語     | `sk`          |
| スロベニア語      | `sl`          |
| スペイン語      | `es`          |
| スウェーデン語      | `sv`          |
| タミール語      | `ta`          |
| タイ語      | `th`          |
| トルコ語      | `tr`          |
| ウクライナ語      | `uk`          |
| ウルドゥー語      | `ur`          |
| ベトナム語      | `vi`          |
| ウェールズ語      | `cy`          |

## <a name="languages-detected-by-the-detect-method"></a>Detect メソッドによって検知される言語

以下の言語を Detect メソッドによって検出できます。 Detect メソッドは、Microsoft Translator が翻訳できない言語を検知できます。

| Language    |
|:----------- |
| アフリカーンス語 |
| アルバニア語 |
| アラビア語 |
| バスク語 |
| ベラルーシ語 |
| ブルガリア語 |
| カタルニア語 |
| 中国語 |
| 中国語 (簡体字) |
| 中国語 (繁体字) |
| クロアチア語 |
| チェコ語 |
| デンマーク語 |
| オランダ語 |
| 英語 |
| エスペラント語 |
| エストニア語 |
| フィンランド語 |
| フランス語 |
| ガリシア語 |
| ドイツ語 |
| ギリシャ語 |
| ハイチ クレオール語 |
| ヘブライ語 |
| ヒンディー語 |
| ハンガリー語 |
| アイスランド語 |
| インドネシア語 |
| アイルランド語 |
| イタリア語 |
| 日本語 |
| 韓国語 |
| クルド語 (アラビア文字) |
| クルド語 (ラテン文字) |
| ラテン語 |
| ラトビア語 |
| リトアニア語 |
| マケドニア語 |
| マレー語 |
| マルタ語 |
| ノルウェー語 |
| ノルウェー語 (ニーノシュク) |
| パシュトウ語 |
| ペルシャ語 |
| ポーランド語 |
| ポルトガル語 |
| ルーマニア語 |
| ロシア語 |
| セルビア語 (キリル文字) |
| セルビア語 (ラテン) |
| スロバキア語 |
| スロベニア語 |
| ソマリ語 |
| スペイン語 |
| スワヒリ語 |
| スウェーデン語 |
| タガログ語 |
| テルグ語 |
| タイ語 |
| トルコ語 |
| ウクライナ語 |
| ウルドゥー語 |
| ウズベク語 (キリル) |
| ウズベク語 (ラテン) |
| ベトナム語 |
| ウェールズ語 |
| イディッシュ語 |

## <a name="access-the-list-programmatically"></a>プログラミングによるリストへのアクセス

V3.0 Text API の Languages 操作を使用すると、サポート対象言語のリストにプログラミングを使用してアクセスできます。 機能、言語コード、英語またはサポートされている言語での言語名を条件にリストを表示できます。 リストは、新しい言語が使用できるようになると、Microsoft Translator サービスによって自動的に更新されます。

[Languages 操作の参照ドキュメント](reference/v3-0-languages.md)

## <a name="access-the-list-on-the-microsoft-translator-website"></a>Microsoft Translator Web サイトのリストにアクセスする

Microsoft Translator Web サイトでは、Translator Text および Speech API でサポートされているすべての言語を簡単に検索できます。 このリストには、言語コードなどの開発者向け情報は含まれていません。

[言語リストを見る](https://www.microsoft.com/translator/languages.aspx)
