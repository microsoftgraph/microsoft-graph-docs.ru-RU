---
title: тип ресурса scoredEmailAddress
description: Представляет оцененный адрес электронной почты.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c16d9b2b6d88f651fa65375f0b8ea9418432cc73
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533808"
---
# <a name="scoredemailaddress-resource-type"></a><span data-ttu-id="e951c-103">тип ресурса scoredEmailAddress</span><span class="sxs-lookup"><span data-stu-id="e951c-103">scoredEmailAddress resource type</span></span>

<span data-ttu-id="e951c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e951c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e951c-105">Представляет оцененный адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="e951c-105">Represents a scored email address.</span></span>


## <a name="properties"></a><span data-ttu-id="e951c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e951c-106">Properties</span></span>
| <span data-ttu-id="e951c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e951c-107">Property</span></span>     | <span data-ttu-id="e951c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e951c-108">Type</span></span>   |<span data-ttu-id="e951c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e951c-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e951c-110">address</span><span class="sxs-lookup"><span data-stu-id="e951c-110">address</span></span>|<span data-ttu-id="e951c-111">string</span><span class="sxs-lookup"><span data-stu-id="e951c-111">string</span></span>|<span data-ttu-id="e951c-112">Адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="e951c-112">The email address.</span></span>|
|<span data-ttu-id="e951c-113">relevanceScore</span><span class="sxs-lookup"><span data-stu-id="e951c-113">relevanceScore</span></span>|<span data-ttu-id="e951c-114">double</span><span class="sxs-lookup"><span data-stu-id="e951c-114">double</span></span>|<span data-ttu-id="e951c-p101">Оценка релевантности адреса электронной почты. Оценка релевантности выступает в роли ключа сортировки по отношению к другим возвращаемым результатам. Более высокий показатель релевантности говорит о высокой степени соответствия результата. Релевантность определяется шаблонами общения и совместной работы пользователя, а также его бизнес-связями.</span><span class="sxs-lookup"><span data-stu-id="e951c-p101">The relevance score of the email address. A relevance score is used as a sort key, in relation to the other returned results. A higher relevance score value corresponds to a more relevant result. Relevance is determined by the user’s communication and collaboration patterns and business relationships.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e951c-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e951c-119">JSON representation</span></span>

<span data-ttu-id="e951c-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e951c-120">Here is a JSON representation of the resource.</span></span>

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
