---
author: daspek
description: Ресурс ShareAction содержит сведения о действии, в результате выполнения которого был предоставлен общий доступ к элементу.
ms.date: 09/14/2017
title: ShareAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 6d855b4c42a51e6ff9c9330f0a22e8076778d456
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48010194"
---
# <a name="shareaction-resource-type"></a><span data-ttu-id="db74e-103">Тип ресурса ShareAction</span><span class="sxs-lookup"><span data-stu-id="db74e-103">ShareAction resource type</span></span>

<span data-ttu-id="db74e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db74e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db74e-105">Ресурс **ShareAction** содержит сведения о [действии][activity], в результате выполнения которого был предоставлен общий доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="db74e-105">The **ShareAction** resource provides information about an [activity][activity] that shared an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="db74e-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="db74e-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="db74e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="db74e-107">Properties</span></span>

| <span data-ttu-id="db74e-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="db74e-108">Property name</span></span> | <span data-ttu-id="db74e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="db74e-109">Type</span></span>                       | <span data-ttu-id="db74e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="db74e-110">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="db74e-111">recipients</span><span class="sxs-lookup"><span data-stu-id="db74e-111">recipients</span></span>    | <span data-ttu-id="db74e-112">Коллекция [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="db74e-112">[identitySet][] collection</span></span> | <span data-ttu-id="db74e-113">Удостоверения, к которым был предоставлен доступ элементу в результате выполнения этого действия.</span><span class="sxs-lookup"><span data-stu-id="db74e-113">The identities the item was shared with in this action.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="db74e-115">Замечания</span><span class="sxs-lookup"><span data-stu-id="db74e-115">Remarks</span></span>

<span data-ttu-id="db74e-116">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="db74e-116">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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


