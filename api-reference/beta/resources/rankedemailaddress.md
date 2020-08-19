---
title: Тип ресурса Ранкедемаиладдресс
description: Представляет ранжированный адрес электронной почты.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: AAmatino
ms.openlocfilehash: f0311b379d2768a2dc704730b7547334e5a64c97
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811422"
---
# <a name="rankedemailaddress-resource-type"></a><span data-ttu-id="4d690-103">Тип ресурса Ранкедемаиладдресс</span><span class="sxs-lookup"><span data-stu-id="4d690-103">rankedEmailAddress resource type</span></span>

<span data-ttu-id="4d690-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d690-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d690-105">Представляет ранжированный адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="4d690-105">Represents a ranked email address.</span></span>


## <a name="properties"></a><span data-ttu-id="4d690-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="4d690-106">Properties</span></span>
| <span data-ttu-id="4d690-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="4d690-107">Property</span></span>     | <span data-ttu-id="4d690-108">Тип</span><span class="sxs-lookup"><span data-stu-id="4d690-108">Type</span></span>   |<span data-ttu-id="4d690-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4d690-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4d690-110">address</span><span class="sxs-lookup"><span data-stu-id="4d690-110">address</span></span>|<span data-ttu-id="4d690-111">string</span><span class="sxs-lookup"><span data-stu-id="4d690-111">string</span></span>|<span data-ttu-id="4d690-112">Адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="4d690-112">The email address.</span></span>|
|<span data-ttu-id="4d690-113">rank</span><span class="sxs-lookup"><span data-stu-id="4d690-113">rank</span></span>|<span data-ttu-id="4d690-114">double</span><span class="sxs-lookup"><span data-stu-id="4d690-114">double</span></span>|<span data-ttu-id="4d690-115">Ранг адреса электронной почты.</span><span class="sxs-lookup"><span data-stu-id="4d690-115">The rank of the email address.</span></span> <span data-ttu-id="4d690-116">В качестве ключа сортировки используется ранг, связанный с другими возвращенными результатами.</span><span class="sxs-lookup"><span data-stu-id="4d690-116">A rank is used as a sort key, in relation to the other returned results.</span></span> <span data-ttu-id="4d690-117">Более высокое значение соответствует более актуальному результату.</span><span class="sxs-lookup"><span data-stu-id="4d690-117">A higher rank value corresponds to a more relevant result.</span></span> <span data-ttu-id="4d690-118">Релевантность определяется сигналами связи, сотрудничества и рабочих отношений.</span><span class="sxs-lookup"><span data-stu-id="4d690-118">Relevance is determined by communication, collaboration, and business relationship signals.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4d690-119">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4d690-119">JSON representation</span></span>

<span data-ttu-id="4d690-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4d690-120">Here is a JSON representation of the resource.</span></span>

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
