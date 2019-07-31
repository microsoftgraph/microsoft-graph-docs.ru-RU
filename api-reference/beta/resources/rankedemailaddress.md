---
title: Тип ресурса Ранкедемаиладдресс
description: Представляет ранжированный адрес электронной почты.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: e29d5b2f2116050f9cea036df35ed6cc012c0e36
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965525"
---
# <a name="rankedemailaddress-resource-type"></a><span data-ttu-id="7d1e0-103">Тип ресурса Ранкедемаиладдресс</span><span class="sxs-lookup"><span data-stu-id="7d1e0-103">rankedEmailAddress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d1e0-104">Представляет ранжированный адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="7d1e0-104">Represents a ranked email address.</span></span>


## <a name="properties"></a><span data-ttu-id="7d1e0-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="7d1e0-105">Properties</span></span>
| <span data-ttu-id="7d1e0-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="7d1e0-106">Property</span></span>     | <span data-ttu-id="7d1e0-107">Тип</span><span class="sxs-lookup"><span data-stu-id="7d1e0-107">Type</span></span>   |<span data-ttu-id="7d1e0-108">Описание</span><span class="sxs-lookup"><span data-stu-id="7d1e0-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7d1e0-109">address</span><span class="sxs-lookup"><span data-stu-id="7d1e0-109">address</span></span>|<span data-ttu-id="7d1e0-110">string</span><span class="sxs-lookup"><span data-stu-id="7d1e0-110">string</span></span>|<span data-ttu-id="7d1e0-111">Адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="7d1e0-111">The email address.</span></span>|
|<span data-ttu-id="7d1e0-112">rank</span><span class="sxs-lookup"><span data-stu-id="7d1e0-112">rank</span></span>|<span data-ttu-id="7d1e0-113">double</span><span class="sxs-lookup"><span data-stu-id="7d1e0-113">double</span></span>|<span data-ttu-id="7d1e0-114">Ранг адреса электронной почты.</span><span class="sxs-lookup"><span data-stu-id="7d1e0-114">The rank of the email address.</span></span> <span data-ttu-id="7d1e0-115">В качестве ключа сортировки используется ранг, связанный с другими возвращенными результатами.</span><span class="sxs-lookup"><span data-stu-id="7d1e0-115">A rank is used as a sort key, in relation to the other returned results.</span></span> <span data-ttu-id="7d1e0-116">Более высокое значение соответствует более актуальному результату.</span><span class="sxs-lookup"><span data-stu-id="7d1e0-116">A higher rank value corresponds to a more relevant result.</span></span> <span data-ttu-id="7d1e0-117">Релевантность определяется сигналами связи, сотрудничества и рабочих отношений.</span><span class="sxs-lookup"><span data-stu-id="7d1e0-117">Relevance is determined by communication, collaboration, and business relationship signals.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7d1e0-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7d1e0-118">JSON representation</span></span>

<span data-ttu-id="7d1e0-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7d1e0-119">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
