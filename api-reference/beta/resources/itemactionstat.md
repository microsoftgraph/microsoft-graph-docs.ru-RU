---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActionStat
localization_priority: Normal
ms.openlocfilehash: 39209671b63b991a8fb3ccf1c830c8557fce27c1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509639"
---
# <a name="itemactionstat-resource-type"></a><span data-ttu-id="92c14-102">Тип ресурса itemActionStat</span><span class="sxs-lookup"><span data-stu-id="92c14-102">itemActionStat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92c14-103">Ресурс **itemActionStat** статистические сведения о действия за период времени.</span><span class="sxs-lookup"><span data-stu-id="92c14-103">The **itemActionStat** resource provides aggregate details about an action over a period of time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="92c14-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="92c14-104">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.itemActionStat",
}-->

```json
{
  "actionCount": 123,
  "actorCount": 60
}
```

## <a name="properties"></a><span data-ttu-id="92c14-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="92c14-105">Properties</span></span>

| <span data-ttu-id="92c14-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="92c14-106">Property</span></span>    | <span data-ttu-id="92c14-107">Тип</span><span class="sxs-lookup"><span data-stu-id="92c14-107">Type</span></span>  | <span data-ttu-id="92c14-108">Описание</span><span class="sxs-lookup"><span data-stu-id="92c14-108">Description</span></span>
|:------------|:------|:-------------------------------------------------------
| <span data-ttu-id="92c14-109">actionCount</span><span class="sxs-lookup"><span data-stu-id="92c14-109">actionCount</span></span> | <span data-ttu-id="92c14-110">Int32</span><span class="sxs-lookup"><span data-stu-id="92c14-110">Int32</span></span> | <span data-ttu-id="92c14-111">Количество раз, когда действие, когда был выполнен.</span><span class="sxs-lookup"><span data-stu-id="92c14-111">The number of times the action took place.</span></span> <span data-ttu-id="92c14-112">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="92c14-112">Read-only.</span></span>
| <span data-ttu-id="92c14-113">actorCount</span><span class="sxs-lookup"><span data-stu-id="92c14-113">actorCount</span></span>  | <span data-ttu-id="92c14-114">Int32</span><span class="sxs-lookup"><span data-stu-id="92c14-114">Int32</span></span> | <span data-ttu-id="92c14-115">Количество уникальных субъекты, выполнившего действия.</span><span class="sxs-lookup"><span data-stu-id="92c14-115">The number of distinct actors that performed the action.</span></span> <span data-ttu-id="92c14-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="92c14-116">Read-only.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActionStat object provides aggregate details about an action over a period of time.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemActionStat",
  "suppressions": [
    "Error: /api-reference/beta/resources/itemactionstat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
