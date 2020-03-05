---
title: Тип ресурса Ранкедемаиладдресс
description: Представляет ранжированный адрес электронной почты.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: bdba5af83357737c77e3b5c441703e404f971587
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521280"
---
# <a name="rankedemailaddress-resource-type"></a><span data-ttu-id="52f2d-103">Тип ресурса Ранкедемаиладдресс</span><span class="sxs-lookup"><span data-stu-id="52f2d-103">rankedEmailAddress resource type</span></span>

<span data-ttu-id="52f2d-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="52f2d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52f2d-105">Представляет ранжированный адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="52f2d-105">Represents a ranked email address.</span></span>


## <a name="properties"></a><span data-ttu-id="52f2d-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="52f2d-106">Properties</span></span>
| <span data-ttu-id="52f2d-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="52f2d-107">Property</span></span>     | <span data-ttu-id="52f2d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="52f2d-108">Type</span></span>   |<span data-ttu-id="52f2d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="52f2d-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="52f2d-110">address</span><span class="sxs-lookup"><span data-stu-id="52f2d-110">address</span></span>|<span data-ttu-id="52f2d-111">string</span><span class="sxs-lookup"><span data-stu-id="52f2d-111">string</span></span>|<span data-ttu-id="52f2d-112">Адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="52f2d-112">The email address.</span></span>|
|<span data-ttu-id="52f2d-113">rank</span><span class="sxs-lookup"><span data-stu-id="52f2d-113">rank</span></span>|<span data-ttu-id="52f2d-114">double</span><span class="sxs-lookup"><span data-stu-id="52f2d-114">double</span></span>|<span data-ttu-id="52f2d-115">Ранг адреса электронной почты.</span><span class="sxs-lookup"><span data-stu-id="52f2d-115">The rank of the email address.</span></span> <span data-ttu-id="52f2d-116">В качестве ключа сортировки используется ранг, связанный с другими возвращенными результатами.</span><span class="sxs-lookup"><span data-stu-id="52f2d-116">A rank is used as a sort key, in relation to the other returned results.</span></span> <span data-ttu-id="52f2d-117">Более высокое значение соответствует более актуальному результату.</span><span class="sxs-lookup"><span data-stu-id="52f2d-117">A higher rank value corresponds to a more relevant result.</span></span> <span data-ttu-id="52f2d-118">Релевантность определяется сигналами связи, сотрудничества и рабочих отношений.</span><span class="sxs-lookup"><span data-stu-id="52f2d-118">Relevance is determined by communication, collaboration, and business relationship signals.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="52f2d-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="52f2d-119">JSON representation</span></span>

<span data-ttu-id="52f2d-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="52f2d-120">Here is a JSON representation of the resource.</span></span>

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
