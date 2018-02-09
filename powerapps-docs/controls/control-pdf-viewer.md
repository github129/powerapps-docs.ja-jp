---
title: "PDF ビューアー コントロール: リファレンス | Microsoft Docs"
description: "各種プロパティとサンプルを含む PDF ビューアー コントロールに関する情報"
services: 
suite: powerapps
documentationcenter: na
author: fikaradz
manager: anneta
editor: 
tags: 
ms.service: powerapps
ms.devlang: na
ms.topic: article
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 10/25/2016
ms.author: fikaradz
ms.openlocfilehash: 8a67a071a19bae57f022fe960a0b29296b58cf5d
ms.sourcegitcommit: 68eee592c351688e5d0bd458f33a70be507fa53f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/29/2018
---
# <a name="pdf-viewer-control-in-powerapps"></a>PowerApps の PDF ビューアー コントロール
PDF ファイルの内容を表示するコントロールです。

## <a name="description"></a>説明
PDF ファイルのテキスト、グラフィック、他の内容を表示するには、この種類のコントロールを追加し、その **Document** プロパティに、表示するファイルの URL を二重引用符で囲んで設定します。

## <a name="limitations"></a>制限
PowerApps のセキュリティ アーキテクチャにより、PDF ビューアーでは HTTPS リンクのみがサポートされ、HTTP リンクはサポートされないことにご注意ください。  
制限の厳しい CORS 設定のサーバーに PDF ドキュメントがある場合、そのドキュメントはアプリ内で表示できない場合があります。  PowerApps でドキュメントを開けない場合は、外部ブラウザーでドキュメントを開くオプションがエンド ユーザーに表示されます。

## <a name="key-properties"></a>主要なプロパティ
**Document** – 二重引用符で囲んだ、PDF ファイルの URL です。

## <a name="additional-properties"></a>その他のプロパティ
**ActualZoom** – コントロールの実際の拡大率です。**Zoom** プロパティで要求された拡大率と異なる場合があります。

**[BorderColor](properties-color-border.md)** – コントロールの境界線の色です。

**[BorderStyle](properties-color-border.md)** – コントロールの境界線を **Solid** (実線)、**Dashed** (破線)、**Dotted** (点線)、**None** (なし) のいずれに指定します。

**[BorderThickness](properties-color-border.md)** – コントロールの境界線の太さです。

**CurrentFindText** – 使用されている現在の検索語です。

**CurrentPage** – 実際に表示されている PDF ファイルのページ番号です。

**[DisplayMode](properties-core.md)** – コントロールで、ユーザー入力を許可するか (**Edit**)、データの表示のみを許可するか (**View**)、許可しないか (**Disabled**) を設定します。

**[DisabledBorderColor](properties-color-border.md)** – コントロールの **[DisplayMode](properties-core.md)** プロパティが **Disabled** に設定されている場合のコントロールの境界線の色です。

**[Fill](properties-color-border.md)** – コントロールの背景色です。

**FindNext** – ドキュメントで **FindText** の次のインスタンスを検索します。

**FindPrevious** – ドキュメントで **FindText** の前のインスタンスを検索します。

**FindText** – ドキュメント内で検索する検索語です。

**[Height](properties-size-location.md)** – コントロールの上端と下端の距離です。

**[HoverBorderColor](properties-color-border.md)** – コントロール上にユーザーがマウス ポインターを重ねているときのコントロールの境界線の色です。

**[OnSelect](properties-core.md)** – ユーザーがコントロールをタップまたはクリックした場合のアプリの反応を指定します。

**OnStateChange** – コントロールの状態が変化したときのアプリの反応を指定します。

**[PaddingBottom](properties-size-location.md)** – コントロール内のテキストとそのコントロールの下端間の距離です。

**[PaddingLeft](properties-size-location.md)** – コントロール内のテキストとそのコントロールの左端間の距離です。

**[PaddingRight](properties-size-location.md)** – コントロール内のテキストとそのコントロールの右端間の距離です。

**[PaddingTop](properties-size-location.md)** – コントロール内のテキストとそのコントロールの上端間の距離です。

**Page** – 表示するページ番号です。

**PageCount** – ドキュメントのページ数です。

**[PressedBorderColor](properties-color-border.md)** – コントロールをユーザーがタップまたはクリックしたときのコントロールの境界線の色です。

**ShowControls** – オーディオ プレイヤーまたはビデオ プレイヤーに再生ボタンと音量スライダーなどを表示するかどうか、およびペン コントロールに描画、削除、クリアなどのアイコンを表示するかどうかを指定します。

**[Tooltip](properties-core.md)** – ユーザーがポインターをコントロールに合わせたときに表示される説明テキストです。

**[Visible](properties-core.md)** – コントロールを表示するか非表示にするかを指定します。

**[Width](properties-size-location.md)** – コントロールの左端と右端の間の距離です。

**[X](properties-size-location.md)** – コントロールの左端とその親コンテナー (親コンテナーがない場合は画面) の左端間の距離です。

**[Y](properties-size-location.md)** – コントロールの上端とその親コンテナー (親コンテナーがない場合は画面) の上端間の距離です。

**Zoom** – カメラからの画像、または PDF ビューアーでのファイルの表示を拡大する割合です。

## <a name="example"></a>例
* **PDF ビューアー** コントロールを追加し、その **Document** プロパティを、この例のように二重引用符で囲んだ PDF の URL に設定します。<br>
  **"http://www.who.int/gho/publications/world_health_statistics/EN_WHS2015_TOC.pdf?ua=1"**

    コントロールに PDF ファイルが表示されます。

    [コントロールの追加および構成](../add-configure-controls.md)についてはこちらをご覧ください。