---
title: Тип ресурса responseStatus
description: Состояние ответа к приглашению на собрание.
localization_priority: Normal
ms.openlocfilehash: 110b0eb158043b9573deb3e3ced792119bfa91a7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579284"
---
# <a name="responsestatus-resource-type"></a><span data-ttu-id="c77fb-103">Тип ресурса responseStatus</span><span class="sxs-lookup"><span data-stu-id="c77fb-103">responseStatus resource type</span></span>

<span data-ttu-id="c77fb-104">Состояние ответа к приглашению на собрание.</span><span class="sxs-lookup"><span data-stu-id="c77fb-104">The response status of a meeting request.</span></span>

## <a name="properties"></a><span data-ttu-id="c77fb-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="c77fb-105">Properties</span></span>

| <span data-ttu-id="c77fb-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="c77fb-106">Property</span></span> | <span data-ttu-id="c77fb-107">Тип</span><span class="sxs-lookup"><span data-stu-id="c77fb-107">Type</span></span>           | <span data-ttu-id="c77fb-108">Описание</span><span class="sxs-lookup"><span data-stu-id="c77fb-108">Description</span></span> |
|:---------|:---------------|:------------|
| <span data-ttu-id="c77fb-109">response</span><span class="sxs-lookup"><span data-stu-id="c77fb-109">response</span></span> | <span data-ttu-id="c77fb-110">responseType</span><span class="sxs-lookup"><span data-stu-id="c77fb-110">responseType</span></span>   | <span data-ttu-id="c77fb-111">Тип ответа.</span><span class="sxs-lookup"><span data-stu-id="c77fb-111">The response type.</span></span> <span data-ttu-id="c77fb-112">Возможные `None`значения:, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`,. `NotResponded`</span><span class="sxs-lookup"><span data-stu-id="c77fb-112">The possible values are: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span></span>
| <span data-ttu-id="c77fb-113">time</span><span class="sxs-lookup"><span data-stu-id="c77fb-113">time</span></span>     | <span data-ttu-id="c77fb-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c77fb-114">DateTimeOffset</span></span> | <span data-ttu-id="c77fb-p102">Дата и время возвращения ответа. Они представлены в формате ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="c77fb-p102">The date and time that the response was returned. It uses ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>

## <a name="json-representation"></a><span data-ttu-id="c77fb-118">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c77fb-118">JSON representation</span></span>

<span data-ttu-id="c77fb-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c77fb-119">Here is a JSON representation of the resource</span></span>

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
