---
title: тип ресурса scoredEmailAddress
description: Представляет оцененный адрес электронной почты.
localization_priority: Normal
ms.openlocfilehash: 740173e7d5f93dc875c08508bf73100727fdf415
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819476"
---
# <a name="scoredemailaddress-resource-type"></a><span data-ttu-id="2b5af-103">тип ресурса scoredEmailAddress</span><span class="sxs-lookup"><span data-stu-id="2b5af-103">scoredEmailAddress resource type</span></span>

<span data-ttu-id="2b5af-104">Представляет оцененный адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="2b5af-104">Represents a scored email address.</span></span>


## <a name="properties"></a><span data-ttu-id="2b5af-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="2b5af-105">Properties</span></span>
| <span data-ttu-id="2b5af-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="2b5af-106">Property</span></span>     | <span data-ttu-id="2b5af-107">Тип</span><span class="sxs-lookup"><span data-stu-id="2b5af-107">Type</span></span>   |<span data-ttu-id="2b5af-108">Описание</span><span class="sxs-lookup"><span data-stu-id="2b5af-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2b5af-109">address</span><span class="sxs-lookup"><span data-stu-id="2b5af-109">address</span></span>|<span data-ttu-id="2b5af-110">string</span><span class="sxs-lookup"><span data-stu-id="2b5af-110">string</span></span>|<span data-ttu-id="2b5af-111">Адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="2b5af-111">The email address.</span></span>|
|<span data-ttu-id="2b5af-112">relevanceScore</span><span class="sxs-lookup"><span data-stu-id="2b5af-112">relevanceScore</span></span>|<span data-ttu-id="2b5af-113">double</span><span class="sxs-lookup"><span data-stu-id="2b5af-113">double</span></span>|<span data-ttu-id="2b5af-p101">Оценка релевантности адреса электронной почты. Оценка релевантности выступает в роли ключа сортировки по отношению к другим возвращаемым результатам. Более высокий показатель релевантности говорит о высокой степени соответствия результата. Релевантность определяется шаблонами общения и совместной работы пользователя, а также его бизнес-связями.</span><span class="sxs-lookup"><span data-stu-id="2b5af-p101">The relevance score of the email address. A relevance score is used as a sort key, in relation to the other returned results. A higher relevance score value corresponds to a more relevant result. Relevance is determined by the user’s communication and collaboration patterns and business relationships.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2b5af-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2b5af-118">JSON representation</span></span>

<span data-ttu-id="2b5af-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2b5af-119">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scoredEmailAddress"
}-->

```json
{
  "address": "string",
  "relevanceScore": 1024.0
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "scoredEmailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
