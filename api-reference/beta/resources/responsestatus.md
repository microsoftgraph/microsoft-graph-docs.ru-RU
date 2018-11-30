---
title: Тип ресурса responseStatus
description: Состояние ответа к приглашению на собрание.
ms.openlocfilehash: 9a6ddb26f018535682611152a69c2039f1c7f016
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077879"
---
# <a name="responsestatus-resource-type"></a><span data-ttu-id="9f864-103">Тип ресурса responseStatus</span><span class="sxs-lookup"><span data-stu-id="9f864-103">responseStatus resource type</span></span>

> <span data-ttu-id="9f864-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9f864-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9f864-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f864-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9f864-106">Состояние ответа к приглашению на собрание.</span><span class="sxs-lookup"><span data-stu-id="9f864-106">The response status of a meeting request.</span></span>

## <a name="properties"></a><span data-ttu-id="9f864-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="9f864-107">Properties</span></span>

| <span data-ttu-id="9f864-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="9f864-108">Property</span></span> | <span data-ttu-id="9f864-109">Тип</span><span class="sxs-lookup"><span data-stu-id="9f864-109">Type</span></span>           | <span data-ttu-id="9f864-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9f864-110">Description</span></span> |
|:---------|:---------------|:------------|
| <span data-ttu-id="9f864-111">response</span><span class="sxs-lookup"><span data-stu-id="9f864-111">response</span></span> | <span data-ttu-id="9f864-112">String</span><span class="sxs-lookup"><span data-stu-id="9f864-112">String</span></span>         | <span data-ttu-id="9f864-113">Тип ответа.</span><span class="sxs-lookup"><span data-stu-id="9f864-113">The response type.</span></span> <span data-ttu-id="9f864-114">Возможные значения: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span><span class="sxs-lookup"><span data-stu-id="9f864-114">Possible values are: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span></span>
| <span data-ttu-id="9f864-115">time</span><span class="sxs-lookup"><span data-stu-id="9f864-115">time</span></span>     | <span data-ttu-id="9f864-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f864-116">DateTimeOffset</span></span> | <span data-ttu-id="9f864-p103">Дата и время возвращения ответа. Они представлены в формате ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="9f864-p103">The date and time that the response was returned. It uses ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>

## <a name="json-representation"></a><span data-ttu-id="9f864-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9f864-120">JSON representation</span></span>

<span data-ttu-id="9f864-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9f864-121">Here is a JSON representation of the resource</span></span>

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
