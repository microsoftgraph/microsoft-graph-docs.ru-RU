---
title: тип ресурса scoredEmailAddress
description: Представляет оцененный адрес электронной почты.
ms.openlocfilehash: 9cdd33a6df9eefca0f7a00c5fe8b17832e0056d9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028476"
---
# <a name="scoredemailaddress-resource-type"></a><span data-ttu-id="fc27f-103">тип ресурса scoredEmailAddress</span><span class="sxs-lookup"><span data-stu-id="fc27f-103">scoredEmailAddress resource type</span></span>

<span data-ttu-id="fc27f-104">Представляет оцененный адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="fc27f-104">Represents a scored email address.</span></span>


## <a name="properties"></a><span data-ttu-id="fc27f-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="fc27f-105">Properties</span></span>
| <span data-ttu-id="fc27f-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="fc27f-106">Property</span></span>     | <span data-ttu-id="fc27f-107">Тип</span><span class="sxs-lookup"><span data-stu-id="fc27f-107">Type</span></span>   |<span data-ttu-id="fc27f-108">Описание</span><span class="sxs-lookup"><span data-stu-id="fc27f-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fc27f-109">address</span><span class="sxs-lookup"><span data-stu-id="fc27f-109">address</span></span>|<span data-ttu-id="fc27f-110">string</span><span class="sxs-lookup"><span data-stu-id="fc27f-110">string</span></span>|<span data-ttu-id="fc27f-111">Адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="fc27f-111">The email address.</span></span>|
|<span data-ttu-id="fc27f-112">relevanceScore</span><span class="sxs-lookup"><span data-stu-id="fc27f-112">relevanceScore</span></span>|<span data-ttu-id="fc27f-113">double</span><span class="sxs-lookup"><span data-stu-id="fc27f-113">double</span></span>|<span data-ttu-id="fc27f-p101">Оценка релевантности адреса электронной почты. Оценка релевантности выступает в роли ключа сортировки по отношению к другим возвращаемым результатам. Более высокий показатель релевантности говорит о высокой степени соответствия результата. Релевантность определяется шаблонами общения и совместной работы пользователя, а также его бизнес-связями.</span><span class="sxs-lookup"><span data-stu-id="fc27f-p101">The relevance score of the email address. A relevance score is used as a sort key, in relation to the other returned results. A higher relevance score value corresponds to a more relevant result. Relevance is determined by the user’s communication and collaboration patterns and business relationships.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fc27f-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fc27f-118">JSON representation</span></span>

<span data-ttu-id="fc27f-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fc27f-119">Here is a JSON representation of the resource.</span></span>

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
