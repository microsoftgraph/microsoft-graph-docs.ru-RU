---
author: daspek
description: Ресурс ShareAction содержит сведения о действии, в результате выполнения которого был предоставлен общий доступ к элементу.
ms.date: 09/14/2017
title: ShareAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 10eb5b870a5ecd80f4a064d1dca496f216bf241d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965168"
---
# <a name="shareaction-resource-type"></a><span data-ttu-id="560a2-103">Тип ресурса ShareAction</span><span class="sxs-lookup"><span data-stu-id="560a2-103">ShareAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="560a2-104">Ресурс **ShareAction** содержит сведения о [действии][activity], в результате выполнения которого был предоставлен общий доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="560a2-104">The **ShareAction** resource provides information about an [activity][activity] that shared an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="560a2-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="560a2-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="560a2-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="560a2-106">Properties</span></span>

| <span data-ttu-id="560a2-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="560a2-107">Property name</span></span> | <span data-ttu-id="560a2-108">Тип</span><span class="sxs-lookup"><span data-stu-id="560a2-108">Type</span></span>                       | <span data-ttu-id="560a2-109">Описание</span><span class="sxs-lookup"><span data-stu-id="560a2-109">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="560a2-110">recipients</span><span class="sxs-lookup"><span data-stu-id="560a2-110">recipients</span></span>    | <span data-ttu-id="560a2-111">Коллекция [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="560a2-111">[identitySet][] collection</span></span> | <span data-ttu-id="560a2-112">Удостоверения, к которым был предоставлен доступ элементу в результате выполнения этого действия.</span><span class="sxs-lookup"><span data-stu-id="560a2-112">The identities the item was shared with in this action.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="560a2-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="560a2-114">Remarks</span></span>

<span data-ttu-id="560a2-115">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="560a2-115">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The ShareAction object provides information about who an item was shared to in a share action.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/ShareAction",
  "suppressions": []
}
-->
