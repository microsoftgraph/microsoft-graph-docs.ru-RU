---
title: Тип ресурса rankedEmailAddress
description: Представляет адрес ранжированных электронной почты.
ms.openlocfilehash: 9234f527ecba6dc83f2e4f80911442d4a083503a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081647"
---
# <a name="rankedemailaddress-resource-type"></a><span data-ttu-id="89aeb-103">Тип ресурса rankedEmailAddress</span><span class="sxs-lookup"><span data-stu-id="89aeb-103">rankedEmailAddress resource type</span></span>

> <span data-ttu-id="89aeb-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="89aeb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="89aeb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89aeb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="89aeb-106">Представляет адрес ранжированных электронной почты.</span><span class="sxs-lookup"><span data-stu-id="89aeb-106">Represents a ranked email address.</span></span>


## <a name="properties"></a><span data-ttu-id="89aeb-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="89aeb-107">Properties</span></span>
| <span data-ttu-id="89aeb-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="89aeb-108">Property</span></span>     | <span data-ttu-id="89aeb-109">Тип</span><span class="sxs-lookup"><span data-stu-id="89aeb-109">Type</span></span>   |<span data-ttu-id="89aeb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="89aeb-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="89aeb-111">address</span><span class="sxs-lookup"><span data-stu-id="89aeb-111">address</span></span>|<span data-ttu-id="89aeb-112">string</span><span class="sxs-lookup"><span data-stu-id="89aeb-112">string</span></span>|<span data-ttu-id="89aeb-113">Адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="89aeb-113">The email address.</span></span>|
|<span data-ttu-id="89aeb-114">rank</span><span class="sxs-lookup"><span data-stu-id="89aeb-114">rank</span></span>|<span data-ttu-id="89aeb-115">double</span><span class="sxs-lookup"><span data-stu-id="89aeb-115">double</span></span>|<span data-ttu-id="89aeb-116">Ранг адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="89aeb-116">The rank of the email address.</span></span> <span data-ttu-id="89aeb-117">Ранг используется в качестве ключа сортировки, при использовании возвращаемых результатов.</span><span class="sxs-lookup"><span data-stu-id="89aeb-117">A rank is used as a sort key, in relation to the other returned results.</span></span> <span data-ttu-id="89aeb-118">Более высокое значение соответствует более актуальному результату.</span><span class="sxs-lookup"><span data-stu-id="89aeb-118">A higher rank value corresponds to a more relevant result.</span></span> <span data-ttu-id="89aeb-119">Релевантность определяется сигналами связи, сотрудничества и рабочих отношений.</span><span class="sxs-lookup"><span data-stu-id="89aeb-119">Relevance is determined by communication, collaboration, and business relationship signals.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="89aeb-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="89aeb-120">JSON representation</span></span>

<span data-ttu-id="89aeb-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="89aeb-121">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "rankedEmailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
