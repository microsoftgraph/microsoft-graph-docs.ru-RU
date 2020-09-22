---
title: Тип ресурса Ранкедемаиладдресс
description: Представляет ранжированный адрес электронной почты.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: AAmatino
ms.openlocfilehash: 36215d545bb6d24fae4ef8cbca35a1c5210976bf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026409"
---
# <a name="rankedemailaddress-resource-type"></a><span data-ttu-id="3905c-103">Тип ресурса Ранкедемаиладдресс</span><span class="sxs-lookup"><span data-stu-id="3905c-103">rankedEmailAddress resource type</span></span>

<span data-ttu-id="3905c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3905c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3905c-105">Представляет ранжированный адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="3905c-105">Represents a ranked email address.</span></span>


## <a name="properties"></a><span data-ttu-id="3905c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="3905c-106">Properties</span></span>
| <span data-ttu-id="3905c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="3905c-107">Property</span></span>     | <span data-ttu-id="3905c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="3905c-108">Type</span></span>   |<span data-ttu-id="3905c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3905c-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3905c-110">address</span><span class="sxs-lookup"><span data-stu-id="3905c-110">address</span></span>|<span data-ttu-id="3905c-111">string</span><span class="sxs-lookup"><span data-stu-id="3905c-111">string</span></span>|<span data-ttu-id="3905c-112">Адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="3905c-112">The email address.</span></span>|
|<span data-ttu-id="3905c-113">rank</span><span class="sxs-lookup"><span data-stu-id="3905c-113">rank</span></span>|<span data-ttu-id="3905c-114">double</span><span class="sxs-lookup"><span data-stu-id="3905c-114">double</span></span>|<span data-ttu-id="3905c-115">Ранг адреса электронной почты.</span><span class="sxs-lookup"><span data-stu-id="3905c-115">The rank of the email address.</span></span> <span data-ttu-id="3905c-116">В качестве ключа сортировки используется ранг, связанный с другими возвращенными результатами.</span><span class="sxs-lookup"><span data-stu-id="3905c-116">A rank is used as a sort key, in relation to the other returned results.</span></span> <span data-ttu-id="3905c-117">Более высокое значение соответствует более актуальному результату.</span><span class="sxs-lookup"><span data-stu-id="3905c-117">A higher rank value corresponds to a more relevant result.</span></span> <span data-ttu-id="3905c-118">Релевантность определяется сигналами связи, сотрудничества и рабочих отношений.</span><span class="sxs-lookup"><span data-stu-id="3905c-118">Relevance is determined by communication, collaboration, and business relationship signals.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3905c-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3905c-119">JSON representation</span></span>

<span data-ttu-id="3905c-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3905c-120">Here is a JSON representation of the resource.</span></span>

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


