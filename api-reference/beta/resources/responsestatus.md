---
title: Тип ресурса responseStatus
description: Состояние ответа к приглашению на собрание.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: a28987d48aa7861a883ac93f53aca63ecaeab9d6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965385"
---
# <a name="responsestatus-resource-type"></a><span data-ttu-id="7dd20-103">Тип ресурса responseStatus</span><span class="sxs-lookup"><span data-stu-id="7dd20-103">responseStatus resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7dd20-104">Состояние ответа к приглашению на собрание.</span><span class="sxs-lookup"><span data-stu-id="7dd20-104">The response status of a meeting request.</span></span>

## <a name="properties"></a><span data-ttu-id="7dd20-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="7dd20-105">Properties</span></span>

| <span data-ttu-id="7dd20-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="7dd20-106">Property</span></span> | <span data-ttu-id="7dd20-107">Тип</span><span class="sxs-lookup"><span data-stu-id="7dd20-107">Type</span></span>           | <span data-ttu-id="7dd20-108">Описание</span><span class="sxs-lookup"><span data-stu-id="7dd20-108">Description</span></span> |
|:---------|:---------------|:------------|
| <span data-ttu-id="7dd20-109">response</span><span class="sxs-lookup"><span data-stu-id="7dd20-109">response</span></span> | <span data-ttu-id="7dd20-110">String</span><span class="sxs-lookup"><span data-stu-id="7dd20-110">String</span></span>         | <span data-ttu-id="7dd20-111">Тип ответа.</span><span class="sxs-lookup"><span data-stu-id="7dd20-111">The response type.</span></span> <span data-ttu-id="7dd20-112">Возможные значения: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span><span class="sxs-lookup"><span data-stu-id="7dd20-112">Possible values are: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span></span>
| <span data-ttu-id="7dd20-113">time</span><span class="sxs-lookup"><span data-stu-id="7dd20-113">time</span></span>     | <span data-ttu-id="7dd20-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7dd20-114">DateTimeOffset</span></span> | <span data-ttu-id="7dd20-p102">Дата и время возвращения ответа. Они представлены в формате ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="7dd20-p102">The date and time that the response was returned. It uses ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>

## <a name="json-representation"></a><span data-ttu-id="7dd20-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7dd20-118">JSON representation</span></span>

<span data-ttu-id="7dd20-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7dd20-119">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "responseStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
