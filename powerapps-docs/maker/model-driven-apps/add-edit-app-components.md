---
title: PowerApps でのモデル駆動型アプリ コンポーネントの追加または編集のためのチュートリアル | MicrosoftDocs
description: PowerApps アプリ デザイナーを使用してコンポーネントを追加または編集
keywords: ''
ms.date: 03/30/2018
ms.service: crm-online
ms.custom: null
ms.topic: article
applies_to:
  - Dynamics 365 (online)
  - Dynamics 365 Version 9.x
  - PowerApps
author: Mattp123
ms.assetid: be93b9d7-f1c2-4ee7-8d7c-0f5c34dfa5f7
ms.author: matp
ms.reviewer: null
ms.suite: null
ms.tgt_pltfrm: null
caps.latest.revision: 17
topic-status: Drafting
search.audienceType:
  - maker
search.app:
  - PowerApps
  - D365CE
---

# <a name="tutorial-add-or-edit-model-driven-app-components-in-the-powerapps-app-designer"></a>チュートリアル: PowerApps アプリ デザイナーでのモデル駆動型アプリ コンポーネントの追加または編集

このチュートリアルでは、モデル駆動型アプリにコンポーネントを追加またはコンポーネントを削除する方法を説明します。 

モデル駆動型アプリは、さまざまなコンポーネントで構成されています。 アプリに追加することができるコンポーネントには、アーティファクトとエンティティ資産の 2 種類があります。 アプリデザイナーのコンテキストでは、エンティティ、ダッシュボード、およびビジネス プロセス フローは、すべてアプリのアーティファクトです。 エンティティ資産は、フォーム、ビュー、グラフ、およびダッシュボードで構成されます。  
  
アプリ デザイナーは、既定のソリューション内の既存のメタデータを参照してください。 フォーム、ビュー、グラフ、およびダッシュボードなどのコンポーネントを作成するために使用することができます。  
  
## <a name="app-designer-layout"></a>アプリ デザイナーのレイアウト  
 アプリ デザイナーには、2 つの主要部分があります。 左側は、アプリ コンポーネントを追加できるキャンバスです。  
  
![アプリ デザイナーのキャンバス](../model-driven-apps/media/app-designer-canvas-pane.png)

 右側は、コンポーネントを選択し、コンポーネントのプロパティを設定するために使用するタブです。  
 
 > [!div class="mx-imgBorder"]
 > ![アプリ デザイナーのコンポーネント](../model-driven-apps/media/app-designer-canvas-components-tab.png "アプリ デザイナーのコンポーネント")  
  
 キャンバスには、サイト マップ、業務プロセス フロー、ダッシュボードおよびエンティティの領域が表示されます。 ダッシュボードまたは業務プロセス フローを選択、またはサイト マップを構成するときは、これらのコンポーネントで使用されるエンティティがアプリ デザイナーによって自動的にキャンバスに追加されます。 これらのエンティティを作成した後に実行する必要があるのは、各エンティティを選択し、フォーム、ビュー、およびグラフなどの必須のエンティティ アセットを追加することです。
 
 また、**キャンバス上の検索**を使用してキャンバス上のコンポーネントを検索することができます。 **キャンバス上の検索**を選択するときは、右端のウィンドウ内のタブの右に新しい検索タブが開きます。   
 
 > [!div class="mx-imgBorder"]
 > ![キャンバス検索オプション](media/app-designer-search-tab.png "キャンバス検索")

## <a name="open-an-app"></a>アプリを開く
1. [PowerApps](https://web.powerapps.com/) にサインインします。 

2. **モデル駆動型** > **アプリ** を選択し、既存のアプリを選択するか **アプリの作成** を選択します。 アプリケーションの作成方法に関する説明については、「[アプリ デザイナーを使用してモデル駆動型アプリを作成または編集](create-edit-app.md#create-an-app)」を参照してください。

## <a name="add-an-artifact-entity-dashboard-or-business-process-flow"></a>アーティファクトを追加する (エンティティ、ダッシュボード、または業務プロセス フロー)  
 ダッシュボードまたは業務プロセス フローをアプリに追加すると、使用するエンティティがアプリに自動的に追加されます。 エンティティを追加すると、アセットのタイルが自動的に追加されます。 デザイナー キャンバスにアーティファクトを追加するには、2 つの方法があります。コマンド バーにある**追加**ボタン![デザイナーの [追加] ボタン](../model-driven-apps/media/dynamics365-designer-addbutton.PNG "デザイナーの [追加] ボタン")を使用するか、または**コンポーネント**タブのタイルを使用します。  
  
 このセクションでは、アプリへダッシュボードを追加する手順について説明します。 業務プロセス フローまたはエンティティの追加も同じ手順を使用します。  
  
1.  アプリデザイナーのキャンバスで、**ダッシュボード**タイルを選択します。  
  
     アプリ デザイナーのキャンバスには、右端のウィンドウに既定のソリューションで利用可能なダッシュボードが表示されます。  
  
    > [!TIP]
    >  または、次のいずれかを実行することもできます:  
    >   
    > - **追加**![デザイナーの [追加] ボタン](../model-driven-apps/media/dynamics365-designer-addbutton.PNG "デザイナーの [追加] ボタン") を選択してから、**ダッシュボード**を選択します。  
    > - **コンポーネント**タブの、**アーティファクト**の下で、**ダッシュボード**を選択します。  
  
2.  **検索**ボックスに、検索するダッシュボードの名前のいくつかのキーワードを入力します。  
  
     ダッシュボード リストでは、検索キーワードと一致する結果だけがフィルター処理されます。  
  
3.  ユーザーが選択したダッシュボードのみを使用する場合は、追加するダッシュボードのチェックボックスをオンにします。 以下の種類のダッシュボードから選択することができます。
    - **クラシック ダッシュボード**は Web アプリケーションおよび統一インターフェイス アプリケーションの両方に表示されます。
    - **対話型ダッシュボード**は統一インターフェイス アプリケーション上にのみ表示されます。 クライアント タイプのアプリを Web アプリケーションのアプリとして選択した場合、**対話型ダッシュボード**オプションは表示されません。

     これらのダッシュボードはアプリ デザイナー キャンバス上の**ダッシュボード**タイルに追加されます。 また、**ダッシュボード**タイルにはアプリに追加したダッシュボード数も表示されます。 ダッシュボードを選択しない場合、ダッシュボード数の代わりに**すべて**が表示され、すべてのダッシュボードはユーザーがアプリを使用するときに利用可能となります。  
  
     ダッシュボードで使用しているすべてのエンティティは、**エンティティ ビュー**領域にも追加されます。 たとえば、Customer Service 管理ダッシュボードを追加する場合は、サポート案件、権利、キュー アイテム エンティティがエンティティの表示領域に追加されます。 各エンティティに対して、そのアセットのタイルも追加されます。 これらのタイルを使用してフォーム、ビュー、およびグラフを追加することができます。 詳細: [PowerApps アプリ デザイナーでのアプリ コンポーネントの追加または編集](add-edit-app-components.md#bkmk_AddEntityAssets)   
  
    ![アプリ デザイナー キャンバスにエンティティを追加](../model-driven-apps/media/add-entity-app-designer-canvas.png "アプリ デザイナー キャンバスにエンティティを追加")  
  
4.  必要なダッシュボードが既定のソリューションに存在しない場合は、キャンバスの右の**コンポーネント**タブで、**新規作成**を選択してダッシュボードを作成します。  
  
     > [!div class="mx-imgBorder"]
     > ![アプリ デザイナーのコンポーネント タブに新しいリンクを作成](../model-driven-apps/media/app-designer-components-tab-create-new.png "アプリ デザイナーのコンポーネント タブに新しいリンクを作成")  
  
     ダッシュボード デザイナーが開きます。 詳細: [ダッシュボードの作成と編集](create-edit-dashboards.md)  
  
    > [!NOTE]
    > - 業務プロセス フロー、またはエンティティを追加する時は、**新規作成**オプションで対応するデザイナーを開きます。 業務プロセス フローまたはエンティティの作成の詳細については、「[業務プロセス フローの作成](/flow/create-business-process-flow)」と「[ユーザー定義エンティティの作成](https://docs.microsoft.com/powerapps/maker/common-data-service/data-platform-create-entity)」を参照してください。  
      
  
5.  アーティファクトの追加が完了したら、コマンドバーの**保存**を選択します。  
  
<a name="bkmk_AddEntityAssets"></a>   
## <a name="add-entity-assets-forms-views-charts-or-dashboards"></a>エンティティ資産 (フォーム、ビュー、グラフ、またはダッシュボード) の追加  
 アーティファクトを使用すると、フォーム、ビュー、グラフ、およびダッシュボードなどのエンティティ資産をアプリに追加することができます。
さらに、統一インターフェイス クライアントを使用する場合は、アプリにエンティティ ダッシュボード資産を追加することができます。  
  
 このセクションでは、アプリへダッシュボードを追加する手順について説明します。 アプリへのビュー、またはグラフの追加も同じ手順を使用します。  
  
1.  アプリ デザイナーのキャンバスで、フォームを追加するエンティティの**フォーム**タイルを選択します。  
  
     アプリ デザイナー キャンバスで、エンティティの行全体が選択されます。 右側に、指定されたエンティティに対するすべての既存のフォームが表示されます。  
  
    > [!NOTE]
    >  または、次のいずれかを実行することもできます:  
    >   
    > - **追加**![デザイナーの [追加] ボタン](../model-driven-apps/media/dynamics365-designer-addbutton.PNG "デザイナーの [追加] ボタン") を選択してから、**フォーム**を選択します。  
    > - **コンポーネント**タブで、**エンティティ資産**の下の、**フォーム**を選択します。  
  
    > [!TIP]
    >  アプリのために選択したすべてのエンティティでは、**コンポーネント**タブ上の**エンティティの選択**リスト内に**詳細オプション**ボタン (**...**) が表示されます。選択したエンティティにすべてのアセットを追加するには、**詳細オプション** (**...**) を選択してから、**すべての資産を追加**を選択します。  
  
2.  アプリのユーザーに対して使用できるフォームを指定する場合は、追加するフォームのチェック ボックスをオンにします。 フォームは、アプリのデータの表示方法と対話方法を定義します。 
 
     選択したエンティティのフォームタイルに、追加されたフォームの数が表示されます。  
  
     ![サポート案件エンティティのフォーム タイル](../model-driven-apps/media/add-forms-entity.png "サポート案件エンティティのフォーム タイル")  
  
     たとえば、エンティティのフォームを選択しない場合、エンド ユーザーがそのアプリを使用するときにそのエンティティのすべてのフォームが表示されます。 この動作は、ビューまたはグラフを選択しない場合の、ビューおよびグラフに似ています。 これにより、使用可能なすべてのコンポーネントを使用する必要がある場合に、ユーザーはアプリをすばやく作成することができます。アプリの設計中に各コンポーネントを選択する必要はありません。  

     ダッシュボードまたは業務プロセス フローが選択されない場合、アプリを使用するユーザーはすべてのダッシュボードと業務プロセス フローを使用することができます。
  
    > [!NOTE]
    > アプリを実行するには、追加する各エンティティには 1 つ以上のアクティブ フォームが必要です。 複数のフォームを選択した場合、ユーザーがアプリを実行するとき、既定のソリューションに表示される最初のアクティブなフォームォームが使用されます。  
  
3.  リストにない新しいフォームを追加する場合は、**新規作成**を選択します。  
  
     ドロップダウン リストで、作成するフォームの種類を選択します。  
  
    > [!NOTE]
    >  ドロップダウン リストは、フォームを追加する場合にのみ使用することができます。 ビュー、およびグラフに対しては使用できません。  
  
     フォーム デザイナーが開きます。 詳細: [フォームの作成および設計](create-design-forms.md)  
  
     ビュー、またはグラフを追加する時は、**新規作成**オプションで対応するデザイナーを開きます。 詳細: 「[ビューについて](create-edit-views.md)」と「[システム グラフの作成または編集](create-edit-system-chart.md)」  
  
    > [!NOTE]
    >  ビューを追加する場合は、ソリューション エクスプローラーの**ビュー**ノードの下にある一覧の共有ビューのみを参照できます。  
  
4. 下向き矢印 ![ドロップ ダウン アイコン](../model-driven-apps/media/drop-down-icon.png "下向き矢印") を選択してタイルを展開し、追加されたフォームのリストを表示します。  
  
     ![アプリ デザイナーで展開したフォーム タイル](../model-driven-apps/media/app-designer-expanded-form-tile.png "アプリ デザイナーで展開したフォーム タイル")  
  
5.  アプリにエンティティ ビュー、およびグラフを追加するには、上記の手順を繰り返します。  
  
6.  **保存**を選びます。  
  
## <a name="edit-or-remove-artifacts"></a>アーティファクトを編集、または削除する  
  
- ダッシュボードまたは業務プロセス フローを編集するには、下向き矢印 ![ドロップ ダウン アイコン](../model-driven-apps/media/drop-down-icon.png "下向き矢印") を選択してタイルを展開してから、編集するダッシュボードまたは業務プロセス フローに応じてサイト マップ デザイナー ボタン ![[サイト マップ デザイナーを開く] ボタン](../model-driven-apps/media/dynamics365-open-designer.PNG "[サイト マップ デザイナーを開く] ボタン") を選択します。  
  
     指定されたアーティファクトのデザイナーが開きます。  
  
- ダッシュボードまたは業務プロセス フローを削除するには、下向き矢印 ![ドロップ ダウン アイコン](../model-driven-apps/media/drop-down-icon.png "下向き矢印") を選択してタイルを展開し、削除するダッシュボードまたは業務プロセス フローを選択します。 コマンド バーで、**削除**を選択します。  

    ダッシュボードまたは業務プロセス フロー内を削除もう一つの方法は、**コンポーネント**タブの対応するチェック ボックスをクリアすることです。
  
- エンティティを編集または削除するには、エンティティ タイルを選択してから、コマンド バーで**編集**または**削除**を選択します。 エンティティを編集する場合は、変更することのできるエンティティのソリューション エクスプローラーが開きます。  
  
     コンポーネントを削除する別の方法は、ダッシュボード、業務プロセス フロー、またはエンティティ タイルを選択することです。 **コンポーネント**タブで、デザイナーから削除するアーティファクトのチェック ボックスをクリアします。  
  
    > [!NOTE]
    >  エンティティを変更 &mdash;エンティティの表示名または説明を変更するなど&mdash; すると、その変更がソリューション エクスプローラに公開されていない限り、変更はアプリ デザイナーに表示されません。  
  
## <a name="edit-or-remove-entity-assets"></a>エンティティアセットの編集、または削除  

### <a name="edit-entity-assets"></a>エンティティ アセットの編集
  
1. 下向き矢印 ![ドロップ ダウン アイコン](../model-driven-apps/media/drop-down-icon.png "下向き矢印") を選択してフォーム、ビュー、グラフ、またはダッシュボードのタイルを展開します。  
  
2. 編集するフォーム、ビュー、グラフ、またはダッシュボードを選択します。  
  
3. コマンド バーで、**編集**を選択します。

   または

   フォーム、ビュー、グラフ、またはダッシュボードの応じてサイト マップ デザイナー ボタン ![[サイト マップ デザイナーを開く] ボタン](../model-driven-apps/media/dynamics365-open-designer.PNG "[サイト マップ デザイナーを開く] ボタン") を選択します。  

### <a name="remove-entity-assets"></a>エンティティアセットの削除  

1. 下向き矢印 ![ドロップ ダウン アイコン](../model-driven-apps/media/drop-down-icon.png "下向き矢印") を選択してフォーム、ビュー、グラフ、またはダッシュボードのタイルを展開します。  
  
2. 編集するフォーム、ビュー、グラフ、またはダッシュボードを選択します。

3. コマンド バーで、**削除**を選択します。 

または、フォーム、ビュー、グラフ、またはダッシュボードのタイルを選択してから、**コンポーネント**タブで、デザイナーから削除する資産のチェック ボックスをクリアすることができます。  
  
## <a name="next-steps"></a>次のステップ  
 [アプリのサイト マップの作成](create-site-map-app.md) </br>  
 [アプリの検証と公開](validate-app.md)
