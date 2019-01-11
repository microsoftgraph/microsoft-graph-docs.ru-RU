---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ShareAction
localization_priority: Normal
ms.openlocfilehash: 16bc590fcfe14f9ce7f6f1bbe38492225cce099c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828660"
---
# <a name="shareaction-resource-type"></a><span data-ttu-id="bdbfc-102">Тип ресурса ShareAction</span><span class="sxs-lookup"><span data-stu-id="bdbfc-102">ShareAction resource type</span></span>

> <span data-ttu-id="bdbfc-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bdbfc-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bdbfc-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bdbfc-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bdbfc-105">Ресурс **ShareAction** содержит сведения о [действии][activity], в результате выполнения которого был предоставлен общий доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="bdbfc-105">The **ShareAction** resource provides information about an [activity][activity] that shared an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="bdbfc-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="bdbfc-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="bdbfc-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="bdbfc-107">Properties</span></span>

| <span data-ttu-id="bdbfc-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="bdbfc-108">Property name</span></span> | <span data-ttu-id="bdbfc-109">Тип</span><span class="sxs-lookup"><span data-stu-id="bdbfc-109">Type</span></span>                       | <span data-ttu-id="bdbfc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bdbfc-110">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="bdbfc-111">recipients</span><span class="sxs-lookup"><span data-stu-id="bdbfc-111">recipients</span></span>    | <span data-ttu-id="bdbfc-112">Коллекция [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="bdbfc-112">[identitySet][] collection</span></span> | <span data-ttu-id="bdbfc-113">Удостоверения, к которым был предоставлен доступ элементу в результате выполнения этого действия.</span><span class="sxs-lookup"><span data-stu-id="bdbfc-113">The identities the item was shared with in this action.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="bdbfc-115">Замечания</span><span class="sxs-lookup"><span data-stu-id="bdbfc-115">Remarks</span></span>

<span data-ttu-id="bdbfc-116">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="bdbfc-116">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The ShareAction object provides information about who an item was shared to in a share action.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/ShareAction"
} -->
