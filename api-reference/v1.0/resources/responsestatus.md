---
title: Тип ресурса responseStatus
description: Состояние ответа к приглашению на собрание.
ms.openlocfilehash: 95f525bae387520888f006d6496a56dab9148145
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025309"
---
# <a name="responsestatus-resource-type"></a><span data-ttu-id="d973f-103">Тип ресурса responseStatus</span><span class="sxs-lookup"><span data-stu-id="d973f-103">responseStatus resource type</span></span>

<span data-ttu-id="d973f-104">Состояние ответа к приглашению на собрание.</span><span class="sxs-lookup"><span data-stu-id="d973f-104">The response status of a meeting request.</span></span>

## <a name="properties"></a><span data-ttu-id="d973f-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="d973f-105">Properties</span></span>

| <span data-ttu-id="d973f-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="d973f-106">Property</span></span> | <span data-ttu-id="d973f-107">Тип</span><span class="sxs-lookup"><span data-stu-id="d973f-107">Type</span></span>           | <span data-ttu-id="d973f-108">Описание</span><span class="sxs-lookup"><span data-stu-id="d973f-108">Description</span></span> |
|:---------|:---------------|:------------|
| <span data-ttu-id="d973f-109">response</span><span class="sxs-lookup"><span data-stu-id="d973f-109">response</span></span> | <span data-ttu-id="d973f-110">responseType</span><span class="sxs-lookup"><span data-stu-id="d973f-110">responseType</span></span>   | <span data-ttu-id="d973f-111">Тип ответа.</span><span class="sxs-lookup"><span data-stu-id="d973f-111">The response type.</span></span> <span data-ttu-id="d973f-112">Возможные значения: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span><span class="sxs-lookup"><span data-stu-id="d973f-112">The possible values are: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span></span>
| <span data-ttu-id="d973f-113">time</span><span class="sxs-lookup"><span data-stu-id="d973f-113">time</span></span>     | <span data-ttu-id="d973f-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d973f-114">DateTimeOffset</span></span> | <span data-ttu-id="d973f-p102">Дата и время возвращения ответа. Они представлены в формате ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="d973f-p102">The date and time that the response was returned. It uses ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>

## <a name="json-representation"></a><span data-ttu-id="d973f-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d973f-118">JSON representation</span></span>

<span data-ttu-id="d973f-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d973f-119">Here is a JSON representation of the resource</span></span>

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
