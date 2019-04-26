---
title: Тип ресурса Ранкедемаиладдресс
description: Представляет ранжированный адрес электронной почты.
localization_priority: Normal
ms.openlocfilehash: 0c92f46c587b4f615b640e47b8d82a33aefc5e50
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344111"
---
# <a name="rankedemailaddress-resource-type"></a><span data-ttu-id="8b58f-103">Тип ресурса Ранкедемаиладдресс</span><span class="sxs-lookup"><span data-stu-id="8b58f-103">rankedEmailAddress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b58f-104">Представляет ранжированный адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="8b58f-104">Represents a ranked email address.</span></span>


## <a name="properties"></a><span data-ttu-id="8b58f-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="8b58f-105">Properties</span></span>
| <span data-ttu-id="8b58f-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="8b58f-106">Property</span></span>     | <span data-ttu-id="8b58f-107">Тип</span><span class="sxs-lookup"><span data-stu-id="8b58f-107">Type</span></span>   |<span data-ttu-id="8b58f-108">Описание</span><span class="sxs-lookup"><span data-stu-id="8b58f-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8b58f-109">address</span><span class="sxs-lookup"><span data-stu-id="8b58f-109">address</span></span>|<span data-ttu-id="8b58f-110">string</span><span class="sxs-lookup"><span data-stu-id="8b58f-110">string</span></span>|<span data-ttu-id="8b58f-111">Адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="8b58f-111">The email address.</span></span>|
|<span data-ttu-id="8b58f-112">rank</span><span class="sxs-lookup"><span data-stu-id="8b58f-112">rank</span></span>|<span data-ttu-id="8b58f-113">double</span><span class="sxs-lookup"><span data-stu-id="8b58f-113">double</span></span>|<span data-ttu-id="8b58f-114">Ранг адреса электронной почты.</span><span class="sxs-lookup"><span data-stu-id="8b58f-114">The rank of the email address.</span></span> <span data-ttu-id="8b58f-115">В качестве ключа сортировки используется ранг, связанный с другими возвращенными результатами.</span><span class="sxs-lookup"><span data-stu-id="8b58f-115">A rank is used as a sort key, in relation to the other returned results.</span></span> <span data-ttu-id="8b58f-116">Более высокое значение соответствует более актуальному результату.</span><span class="sxs-lookup"><span data-stu-id="8b58f-116">A higher rank value corresponds to a more relevant result.</span></span> <span data-ttu-id="8b58f-117">Релевантность определяется сигналами связи, сотрудничества и рабочих отношений.</span><span class="sxs-lookup"><span data-stu-id="8b58f-117">Relevance is determined by communication, collaboration, and business relationship signals.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8b58f-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8b58f-118">JSON representation</span></span>

<span data-ttu-id="8b58f-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8b58f-119">Here is a JSON representation of the resource.</span></span>

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
