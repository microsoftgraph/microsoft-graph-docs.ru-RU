---
title: тип ресурса scoredEmailAddress
description: Представляет оцененный адрес электронной почты.
localization_priority: Normal
author: AAmatino
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 81fabe954a104663cfcd228bfc182549355bc3db
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806753"
---
# <a name="scoredemailaddress-resource-type"></a><span data-ttu-id="3aa97-103">тип ресурса scoredEmailAddress</span><span class="sxs-lookup"><span data-stu-id="3aa97-103">scoredEmailAddress resource type</span></span>

<span data-ttu-id="3aa97-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3aa97-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3aa97-105">Представляет оцененный адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="3aa97-105">Represents a scored email address.</span></span>


## <a name="properties"></a><span data-ttu-id="3aa97-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="3aa97-106">Properties</span></span>
| <span data-ttu-id="3aa97-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="3aa97-107">Property</span></span>     | <span data-ttu-id="3aa97-108">Тип</span><span class="sxs-lookup"><span data-stu-id="3aa97-108">Type</span></span>   |<span data-ttu-id="3aa97-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3aa97-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3aa97-110">address</span><span class="sxs-lookup"><span data-stu-id="3aa97-110">address</span></span>|<span data-ttu-id="3aa97-111">string</span><span class="sxs-lookup"><span data-stu-id="3aa97-111">string</span></span>|<span data-ttu-id="3aa97-112">Адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="3aa97-112">The email address.</span></span>|
|<span data-ttu-id="3aa97-113">relevanceScore</span><span class="sxs-lookup"><span data-stu-id="3aa97-113">relevanceScore</span></span>|<span data-ttu-id="3aa97-114">double</span><span class="sxs-lookup"><span data-stu-id="3aa97-114">double</span></span>|<span data-ttu-id="3aa97-p101">Оценка релевантности адреса электронной почты. Оценка релевантности выступает в роли ключа сортировки по отношению к другим возвращаемым результатам. Более высокий показатель релевантности говорит о высокой степени соответствия результата. Релевантность определяется шаблонами общения и совместной работы пользователя, а также его бизнес-связями.</span><span class="sxs-lookup"><span data-stu-id="3aa97-p101">The relevance score of the email address. A relevance score is used as a sort key, in relation to the other returned results. A higher relevance score value corresponds to a more relevant result. Relevance is determined by the user’s communication and collaboration patterns and business relationships.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3aa97-119">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3aa97-119">JSON representation</span></span>

<span data-ttu-id="3aa97-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3aa97-120">Here is a JSON representation of the resource.</span></span>

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
