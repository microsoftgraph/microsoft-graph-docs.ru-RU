---
title: тип ресурса scoredEmailAddress
description: Представляет оцененный адрес электронной почты.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: b8cdcd7a0192bdd97bc096ce06514e75a7184f63
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034596"
---
# <a name="scoredemailaddress-resource-type"></a><span data-ttu-id="e39b9-103">тип ресурса scoredEmailAddress</span><span class="sxs-lookup"><span data-stu-id="e39b9-103">scoredEmailAddress resource type</span></span>

<span data-ttu-id="e39b9-104">Представляет оцененный адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="e39b9-104">Represents a scored email address.</span></span>


## <a name="properties"></a><span data-ttu-id="e39b9-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="e39b9-105">Properties</span></span>
| <span data-ttu-id="e39b9-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="e39b9-106">Property</span></span>     | <span data-ttu-id="e39b9-107">Тип</span><span class="sxs-lookup"><span data-stu-id="e39b9-107">Type</span></span>   |<span data-ttu-id="e39b9-108">Описание</span><span class="sxs-lookup"><span data-stu-id="e39b9-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e39b9-109">address</span><span class="sxs-lookup"><span data-stu-id="e39b9-109">address</span></span>|<span data-ttu-id="e39b9-110">string</span><span class="sxs-lookup"><span data-stu-id="e39b9-110">string</span></span>|<span data-ttu-id="e39b9-111">Адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="e39b9-111">The email address.</span></span>|
|<span data-ttu-id="e39b9-112">relevanceScore</span><span class="sxs-lookup"><span data-stu-id="e39b9-112">relevanceScore</span></span>|<span data-ttu-id="e39b9-113">double</span><span class="sxs-lookup"><span data-stu-id="e39b9-113">double</span></span>|<span data-ttu-id="e39b9-p101">Оценка релевантности адреса электронной почты. Оценка релевантности выступает в роли ключа сортировки по отношению к другим возвращаемым результатам. Более высокий показатель релевантности говорит о высокой степени соответствия результата. Релевантность определяется шаблонами общения и совместной работы пользователя, а также его бизнес-связями.</span><span class="sxs-lookup"><span data-stu-id="e39b9-p101">The relevance score of the email address. A relevance score is used as a sort key, in relation to the other returned results. A higher relevance score value corresponds to a more relevant result. Relevance is determined by the user’s communication and collaboration patterns and business relationships.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e39b9-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e39b9-118">JSON representation</span></span>

<span data-ttu-id="e39b9-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e39b9-119">Here is a JSON representation of the resource.</span></span>

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
