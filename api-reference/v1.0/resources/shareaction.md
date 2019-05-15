---
author: daspek
ms.author: dspektor
title: Тип ресурса shareAction
description: Объект shareAction предоставляет сведения о том, к которому был предоставлен общий доступ к элементу в действии Share.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: a61ec47aae94eb99c2a192c863127d18a80fc087
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970792"
---
# <a name="shareaction-resource-type"></a><span data-ttu-id="c5344-103">Тип ресурса shareAction</span><span class="sxs-lookup"><span data-stu-id="c5344-103">shareAction resource type</span></span>

<span data-ttu-id="c5344-104">Ресурс **shareAction** предоставляет сведения о [действии] [ activity] , в котором общий доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="c5344-104">The **shareAction** resource provides information about an [activity][activity] that shared an item.</span></span>

><span data-ttu-id="c5344-105">**Примечание:** Записи действий элементов в настоящее время доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="c5344-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="c5344-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c5344-106">Properties</span></span>

| <span data-ttu-id="c5344-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="c5344-107">Property name</span></span> | <span data-ttu-id="c5344-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c5344-108">Type</span></span>                       | <span data-ttu-id="c5344-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c5344-109">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="c5344-110">recipients</span><span class="sxs-lookup"><span data-stu-id="c5344-110">recipients</span></span>    | <span data-ttu-id="c5344-111">Коллекция [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="c5344-111">[identitySet][] collection</span></span> | <span data-ttu-id="c5344-112">Удостоверения, к которым был предоставлен доступ элементу в результате выполнения этого действия.</span><span class="sxs-lookup"><span data-stu-id="c5344-112">The identities the item was shared with in this action.</span></span>

[identitySet]: identityset.md

## <a name="json-representation"></a><span data-ttu-id="c5344-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c5344-114">JSON representation</span></span>

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
