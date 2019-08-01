---
title: Тип ресурса responseStatus
description: Состояние ответа к приглашению на собрание.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 03deeabfd789fe3e8912d5a431af21bc2c8e5256
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034666"
---
# <a name="responsestatus-resource-type"></a><span data-ttu-id="ba462-103">Тип ресурса responseStatus</span><span class="sxs-lookup"><span data-stu-id="ba462-103">responseStatus resource type</span></span>

<span data-ttu-id="ba462-104">Состояние ответа к приглашению на собрание.</span><span class="sxs-lookup"><span data-stu-id="ba462-104">The response status of a meeting request.</span></span>

## <a name="properties"></a><span data-ttu-id="ba462-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="ba462-105">Properties</span></span>

| <span data-ttu-id="ba462-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="ba462-106">Property</span></span> | <span data-ttu-id="ba462-107">Тип</span><span class="sxs-lookup"><span data-stu-id="ba462-107">Type</span></span>           | <span data-ttu-id="ba462-108">Описание</span><span class="sxs-lookup"><span data-stu-id="ba462-108">Description</span></span> |
|:---------|:---------------|:------------|
| <span data-ttu-id="ba462-109">response</span><span class="sxs-lookup"><span data-stu-id="ba462-109">response</span></span> | <span data-ttu-id="ba462-110">responseType</span><span class="sxs-lookup"><span data-stu-id="ba462-110">responseType</span></span>   | <span data-ttu-id="ba462-111">Тип ответа.</span><span class="sxs-lookup"><span data-stu-id="ba462-111">The response type.</span></span> <span data-ttu-id="ba462-112">Допустимые значения: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span><span class="sxs-lookup"><span data-stu-id="ba462-112">The possible values are: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span></span>
| <span data-ttu-id="ba462-113">time</span><span class="sxs-lookup"><span data-stu-id="ba462-113">time</span></span>     | <span data-ttu-id="ba462-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba462-114">DateTimeOffset</span></span> | <span data-ttu-id="ba462-p102">Дата и время возвращения ответа. Они представлены в формате ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="ba462-p102">The date and time that the response was returned. It uses ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>

## <a name="json-representation"></a><span data-ttu-id="ba462-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ba462-118">JSON representation</span></span>

<span data-ttu-id="ba462-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ba462-119">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.responseStatus"
}-->

```json
{
  "response": "String",
  "time": "String (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "responseStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
