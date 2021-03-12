---
title: Тип ресурса responseStatus
description: Состояние ответа к приглашению на собрание.
localization_priority: Normal
author: harini84
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 1aebaa2672b741798a2c6bbf95c8c9d966cabfd1
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722386"
---
# <a name="responsestatus-resource-type"></a><span data-ttu-id="ce3b4-103">Тип ресурса responseStatus</span><span class="sxs-lookup"><span data-stu-id="ce3b4-103">responseStatus resource type</span></span>

<span data-ttu-id="ce3b4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce3b4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ce3b4-105">Состояние ответа к приглашению на собрание.</span><span class="sxs-lookup"><span data-stu-id="ce3b4-105">The response status of a meeting request.</span></span>

## <a name="properties"></a><span data-ttu-id="ce3b4-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ce3b4-106">Properties</span></span>

| <span data-ttu-id="ce3b4-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="ce3b4-107">Property</span></span> | <span data-ttu-id="ce3b4-108">Тип</span><span class="sxs-lookup"><span data-stu-id="ce3b4-108">Type</span></span>           | <span data-ttu-id="ce3b4-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ce3b4-109">Description</span></span> |
|:---------|:---------------|:------------|
| <span data-ttu-id="ce3b4-110">response</span><span class="sxs-lookup"><span data-stu-id="ce3b4-110">response</span></span> | <span data-ttu-id="ce3b4-111">responseType</span><span class="sxs-lookup"><span data-stu-id="ce3b4-111">responseType</span></span>   | <span data-ttu-id="ce3b4-112">Тип ответа.</span><span class="sxs-lookup"><span data-stu-id="ce3b4-112">The response type.</span></span> <span data-ttu-id="ce3b4-113">Допустимые значения: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span><span class="sxs-lookup"><span data-stu-id="ce3b4-113">The possible values are: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span></span>
| <span data-ttu-id="ce3b4-114">time</span><span class="sxs-lookup"><span data-stu-id="ce3b4-114">time</span></span>     | <span data-ttu-id="ce3b4-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce3b4-115">DateTimeOffset</span></span> | <span data-ttu-id="ce3b4-116">Дата и время возвращения ответа.</span><span class="sxs-lookup"><span data-stu-id="ce3b4-116">The date and time that the response was returned.</span></span> <span data-ttu-id="ce3b4-117">Они представлены в формате ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="ce3b4-117">It uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ce3b4-118">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="ce3b4-118">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>

## <a name="json-representation"></a><span data-ttu-id="ce3b4-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ce3b4-119">JSON representation</span></span>

<span data-ttu-id="ce3b4-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ce3b4-120">Here is a JSON representation of the resource</span></span>

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

