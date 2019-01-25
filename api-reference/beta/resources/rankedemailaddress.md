---
title: Тип ресурса rankedEmailAddress
description: Представляет адрес ранжированных электронной почты.
localization_priority: Normal
ms.openlocfilehash: 938afc0de208fd3cdbd0cfec299d01ada9d4f592
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510010"
---
# <a name="rankedemailaddress-resource-type"></a><span data-ttu-id="0d82b-103">Тип ресурса rankedEmailAddress</span><span class="sxs-lookup"><span data-stu-id="0d82b-103">rankedEmailAddress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d82b-104">Представляет адрес ранжированных электронной почты.</span><span class="sxs-lookup"><span data-stu-id="0d82b-104">Represents a ranked email address.</span></span>


## <a name="properties"></a><span data-ttu-id="0d82b-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="0d82b-105">Properties</span></span>
| <span data-ttu-id="0d82b-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="0d82b-106">Property</span></span>     | <span data-ttu-id="0d82b-107">Тип</span><span class="sxs-lookup"><span data-stu-id="0d82b-107">Type</span></span>   |<span data-ttu-id="0d82b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="0d82b-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0d82b-109">address</span><span class="sxs-lookup"><span data-stu-id="0d82b-109">address</span></span>|<span data-ttu-id="0d82b-110">string</span><span class="sxs-lookup"><span data-stu-id="0d82b-110">string</span></span>|<span data-ttu-id="0d82b-111">Адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="0d82b-111">The email address.</span></span>|
|<span data-ttu-id="0d82b-112">rank</span><span class="sxs-lookup"><span data-stu-id="0d82b-112">rank</span></span>|<span data-ttu-id="0d82b-113">double</span><span class="sxs-lookup"><span data-stu-id="0d82b-113">double</span></span>|<span data-ttu-id="0d82b-114">Ранг адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="0d82b-114">The rank of the email address.</span></span> <span data-ttu-id="0d82b-115">Ранг используется в качестве ключа сортировки, при использовании возвращаемых результатов.</span><span class="sxs-lookup"><span data-stu-id="0d82b-115">A rank is used as a sort key, in relation to the other returned results.</span></span> <span data-ttu-id="0d82b-116">Более высокое значение соответствует более актуальному результату.</span><span class="sxs-lookup"><span data-stu-id="0d82b-116">A higher rank value corresponds to a more relevant result.</span></span> <span data-ttu-id="0d82b-117">Релевантность определяется сигналами связи, сотрудничества и рабочих отношений.</span><span class="sxs-lookup"><span data-stu-id="0d82b-117">Relevance is determined by communication, collaboration, and business relationship signals.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0d82b-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0d82b-118">JSON representation</span></span>

<span data-ttu-id="0d82b-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0d82b-119">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rankedEmailAddress"
}-->

```json
{
  "address": "string",
  "rank": 1024
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "rankedEmailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/rankedemailaddress.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
