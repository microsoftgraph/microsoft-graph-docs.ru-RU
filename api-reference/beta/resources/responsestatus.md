---
title: Тип ресурса responseStatus
description: Состояние ответа к приглашению на собрание.
localization_priority: Normal
ms.openlocfilehash: 8ec4b5f74fa8d83369c23f829b34dfa0ed53a1a1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343579"
---
# <a name="responsestatus-resource-type"></a><span data-ttu-id="55b58-103">Тип ресурса responseStatus</span><span class="sxs-lookup"><span data-stu-id="55b58-103">responseStatus resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55b58-104">Состояние ответа к приглашению на собрание.</span><span class="sxs-lookup"><span data-stu-id="55b58-104">The response status of a meeting request.</span></span>

## <a name="properties"></a><span data-ttu-id="55b58-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="55b58-105">Properties</span></span>

| <span data-ttu-id="55b58-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="55b58-106">Property</span></span> | <span data-ttu-id="55b58-107">Тип</span><span class="sxs-lookup"><span data-stu-id="55b58-107">Type</span></span>           | <span data-ttu-id="55b58-108">Описание</span><span class="sxs-lookup"><span data-stu-id="55b58-108">Description</span></span> |
|:---------|:---------------|:------------|
| <span data-ttu-id="55b58-109">response</span><span class="sxs-lookup"><span data-stu-id="55b58-109">response</span></span> | <span data-ttu-id="55b58-110">String</span><span class="sxs-lookup"><span data-stu-id="55b58-110">String</span></span>         | <span data-ttu-id="55b58-111">Тип ответа.</span><span class="sxs-lookup"><span data-stu-id="55b58-111">The response type.</span></span> <span data-ttu-id="55b58-112">Возможные значения: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span><span class="sxs-lookup"><span data-stu-id="55b58-112">Possible values are: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span></span>
| <span data-ttu-id="55b58-113">time</span><span class="sxs-lookup"><span data-stu-id="55b58-113">time</span></span>     | <span data-ttu-id="55b58-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55b58-114">DateTimeOffset</span></span> | <span data-ttu-id="55b58-p102">Дата и время возвращения ответа. Они представлены в формате ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="55b58-p102">The date and time that the response was returned. It uses ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>

## <a name="json-representation"></a><span data-ttu-id="55b58-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="55b58-118">JSON representation</span></span>

<span data-ttu-id="55b58-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="55b58-119">Here is a JSON representation of the resource</span></span>

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
