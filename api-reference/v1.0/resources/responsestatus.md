---
title: Тип ресурса responseStatus
description: Состояние ответа к приглашению на собрание.
localization_priority: Normal
author: harini84
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 69aae664c21290d00505997d5ff84658620d67e8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47967214"
---
# <a name="responsestatus-resource-type"></a><span data-ttu-id="64178-103">Тип ресурса responseStatus</span><span class="sxs-lookup"><span data-stu-id="64178-103">responseStatus resource type</span></span>

<span data-ttu-id="64178-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64178-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="64178-105">Состояние ответа к приглашению на собрание.</span><span class="sxs-lookup"><span data-stu-id="64178-105">The response status of a meeting request.</span></span>

## <a name="properties"></a><span data-ttu-id="64178-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="64178-106">Properties</span></span>

| <span data-ttu-id="64178-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="64178-107">Property</span></span> | <span data-ttu-id="64178-108">Тип</span><span class="sxs-lookup"><span data-stu-id="64178-108">Type</span></span>           | <span data-ttu-id="64178-109">Описание</span><span class="sxs-lookup"><span data-stu-id="64178-109">Description</span></span> |
|:---------|:---------------|:------------|
| <span data-ttu-id="64178-110">response</span><span class="sxs-lookup"><span data-stu-id="64178-110">response</span></span> | <span data-ttu-id="64178-111">responseType</span><span class="sxs-lookup"><span data-stu-id="64178-111">responseType</span></span>   | <span data-ttu-id="64178-112">Тип ответа.</span><span class="sxs-lookup"><span data-stu-id="64178-112">The response type.</span></span> <span data-ttu-id="64178-113">Допустимые значения: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span><span class="sxs-lookup"><span data-stu-id="64178-113">The possible values are: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span></span>
| <span data-ttu-id="64178-114">time</span><span class="sxs-lookup"><span data-stu-id="64178-114">time</span></span>     | <span data-ttu-id="64178-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64178-115">DateTimeOffset</span></span> | <span data-ttu-id="64178-p102">Дата и время возвращения ответа. Они представлены в формате ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="64178-p102">The date and time that the response was returned. It uses ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>

## <a name="json-representation"></a><span data-ttu-id="64178-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="64178-119">JSON representation</span></span>

<span data-ttu-id="64178-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="64178-120">Here is a JSON representation of the resource</span></span>

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

