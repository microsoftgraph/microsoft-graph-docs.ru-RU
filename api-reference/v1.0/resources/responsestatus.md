---
title: Тип ресурса responseStatus
description: Состояние ответа к приглашению на собрание.
localization_priority: Normal
author: harini84
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 77adc43ef3485f7fcf42a8c1c77edc5d123a3424
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812662"
---
# <a name="responsestatus-resource-type"></a><span data-ttu-id="acd75-103">Тип ресурса responseStatus</span><span class="sxs-lookup"><span data-stu-id="acd75-103">responseStatus resource type</span></span>

<span data-ttu-id="acd75-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="acd75-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="acd75-105">Состояние ответа к приглашению на собрание.</span><span class="sxs-lookup"><span data-stu-id="acd75-105">The response status of a meeting request.</span></span>

## <a name="properties"></a><span data-ttu-id="acd75-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="acd75-106">Properties</span></span>

| <span data-ttu-id="acd75-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="acd75-107">Property</span></span> | <span data-ttu-id="acd75-108">Тип</span><span class="sxs-lookup"><span data-stu-id="acd75-108">Type</span></span>           | <span data-ttu-id="acd75-109">Описание</span><span class="sxs-lookup"><span data-stu-id="acd75-109">Description</span></span> |
|:---------|:---------------|:------------|
| <span data-ttu-id="acd75-110">response</span><span class="sxs-lookup"><span data-stu-id="acd75-110">response</span></span> | <span data-ttu-id="acd75-111">responseType</span><span class="sxs-lookup"><span data-stu-id="acd75-111">responseType</span></span>   | <span data-ttu-id="acd75-112">Тип ответа.</span><span class="sxs-lookup"><span data-stu-id="acd75-112">The response type.</span></span> <span data-ttu-id="acd75-113">Допустимые значения: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span><span class="sxs-lookup"><span data-stu-id="acd75-113">The possible values are: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span></span>
| <span data-ttu-id="acd75-114">time</span><span class="sxs-lookup"><span data-stu-id="acd75-114">time</span></span>     | <span data-ttu-id="acd75-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="acd75-115">DateTimeOffset</span></span> | <span data-ttu-id="acd75-p102">Дата и время возвращения ответа. Они представлены в формате ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="acd75-p102">The date and time that the response was returned. It uses ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>

## <a name="json-representation"></a><span data-ttu-id="acd75-119">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="acd75-119">JSON representation</span></span>

<span data-ttu-id="acd75-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="acd75-120">Here is a JSON representation of the resource</span></span>

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
