---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ShareAction
localization_priority: Normal
ms.openlocfilehash: 785a0a9ac9a2a1ecbd40c0d8ccae16dca9594fdf
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520538"
---
# <a name="shareaction-resource-type"></a><span data-ttu-id="9012a-102">Тип ресурса ShareAction</span><span class="sxs-lookup"><span data-stu-id="9012a-102">ShareAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9012a-103">Ресурс **ShareAction** содержит сведения о [действии][activity], в результате выполнения которого был предоставлен общий доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="9012a-103">The **ShareAction** resource provides information about an [activity][activity] that shared an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="9012a-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="9012a-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="9012a-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="9012a-105">Properties</span></span>

| <span data-ttu-id="9012a-106">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="9012a-106">Property name</span></span> | <span data-ttu-id="9012a-107">Тип</span><span class="sxs-lookup"><span data-stu-id="9012a-107">Type</span></span>                       | <span data-ttu-id="9012a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="9012a-108">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="9012a-109">recipients</span><span class="sxs-lookup"><span data-stu-id="9012a-109">recipients</span></span>    | <span data-ttu-id="9012a-110">Коллекция [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="9012a-110">[identitySet][] collection</span></span> | <span data-ttu-id="9012a-111">Удостоверения, к которым был предоставлен доступ элементу в результате выполнения этого действия.</span><span class="sxs-lookup"><span data-stu-id="9012a-111">The identities the item was shared with in this action.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="9012a-113">Замечания</span><span class="sxs-lookup"><span data-stu-id="9012a-113">Remarks</span></span>

<span data-ttu-id="9012a-114">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="9012a-114">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The ShareAction object provides information about who an item was shared to in a share action.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/ShareAction",
  "suppressions": [
    "Error: /api-reference/beta/resources/shareaction.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
