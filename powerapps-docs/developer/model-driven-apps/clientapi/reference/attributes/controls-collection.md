---
title: コントロールコレクション (クライアントAPI参照) | MicrosoftDocs
description: 属性に関連付けられているコントロールへのアクセス方法について説明します。
ms.date: 10/31/2018
ms.service: crm-online
ms.topic: reference
applies_to: Dynamics 365 (online)
ms.assetid: d5f3c0c5-b267-42a8-82e8-8c4a1cda3752
author: KumarVivek
ms.author: kvivek
manager: amyla
search.audienceType:
  - developer
search.app:
  - PowerApps
  - D365CE
---
# <a name="controls-collection-client-api-reference"></a>コントロールコレクション (クライアントAPI参照)



コントロールコレクションを使用して、属性に関連付けられているコントロールにアクセスします。 

各属性はページに 1 回以上表示される場合があるため、コントロールのコレクションにはその属性表示のすべてのコントロールへのアクセスが用意されています。 属性がページの 1 つのフィールドのみを示す場合、このコレクションの長さは 1 です。 コントロール getName メソッドを使用するとき、最初のコントロールの名前は属性の名前と同じになります。 その属性のコントロールの 2 番目のインスタンスは **<attributeName>1** となります。 **<attributeName>+N**のパターンにより、特定の属性用フォームに追加された、各追加コントロールが指定されます。

フォームのヘッダーに業務プロセス フローのコントロールが表示される場合、業務プロセス フローに表示される各属性のために、さらにコントロールが追加されます。 これらのコントロールは、**header_process_<attribute name>** などの、一意の名前があります。

属性に関連付けられたコントロール上でアクションを実行するときは、そのコントロールがそのページ上に 1 回以上含まれる可能性があり、一般的に、属性の各コントロールのために同じアクションを実行する必要があることを考慮します。 これは、属性コントロールのコレクションを繰り返し、各コントロール上でアクションを実行することにより実行できます。

### <a name="related-topics"></a>関連トピック

[属性 (クライアントAPI参照) ](../attributes.md)

