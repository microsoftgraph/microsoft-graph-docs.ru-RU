---
author: daspek
ms.author: dspektor
title: Тип ресурса shareAction
description: Объект shareAction предоставляет сведения о том, к которому был предоставлен общий доступ к элементу в действии Share.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 73b847bbd9608a7647f3895e8d67fff9dbdc9a68
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034351"
---
# <a name="shareaction-resource-type"></a><span data-ttu-id="9f3f0-103">Тип ресурса shareAction</span><span class="sxs-lookup"><span data-stu-id="9f3f0-103">shareAction resource type</span></span>

<span data-ttu-id="9f3f0-104">Ресурс **shareAction** предоставляет сведения о [действии][activity] , в котором общий доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="9f3f0-104">The **shareAction** resource provides information about an [activity][activity] that shared an item.</span></span>

><span data-ttu-id="9f3f0-105">**Примечание:** Записи действий элементов в настоящее время доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="9f3f0-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="9f3f0-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="9f3f0-106">Properties</span></span>

| <span data-ttu-id="9f3f0-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="9f3f0-107">Property name</span></span> | <span data-ttu-id="9f3f0-108">Тип</span><span class="sxs-lookup"><span data-stu-id="9f3f0-108">Type</span></span>                       | <span data-ttu-id="9f3f0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9f3f0-109">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="9f3f0-110">recipients</span><span class="sxs-lookup"><span data-stu-id="9f3f0-110">recipients</span></span>    | <span data-ttu-id="9f3f0-111">Коллекция [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="9f3f0-111">[identitySet][] collection</span></span> | <span data-ttu-id="9f3f0-112">Удостоверения, к которым был предоставлен доступ элементу в результате выполнения этого действия.</span><span class="sxs-lookup"><span data-stu-id="9f3f0-112">The identities the item was shared with in this action.</span></span>

[identitySet]: identityset.md

## <a name="json-representation"></a><span data-ttu-id="9f3f0-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9f3f0-114">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.shareAction"
}-->

```json
{
  "recipients": [{"@odata.type": "microsoft.graph.identitySet"}]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The shareAction object provides information about who an item was shared to in a share action.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/shareAction",
  "suppressions": []
}
-->
