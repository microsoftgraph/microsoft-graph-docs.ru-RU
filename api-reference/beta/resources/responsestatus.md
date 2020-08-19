---
title: Тип ресурса responseStatus
description: Состояние ответа к приглашению на собрание.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: harini84
ms.openlocfilehash: 4ab1c5e54112b5d51e3d88452e2ee0ddcb59f6dd
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811387"
---
# <a name="responsestatus-resource-type"></a><span data-ttu-id="72ed8-103">Тип ресурса responseStatus</span><span class="sxs-lookup"><span data-stu-id="72ed8-103">responseStatus resource type</span></span>

<span data-ttu-id="72ed8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72ed8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72ed8-105">Состояние ответа к приглашению на собрание.</span><span class="sxs-lookup"><span data-stu-id="72ed8-105">The response status of a meeting request.</span></span>

## <a name="properties"></a><span data-ttu-id="72ed8-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="72ed8-106">Properties</span></span>

| <span data-ttu-id="72ed8-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="72ed8-107">Property</span></span> | <span data-ttu-id="72ed8-108">Тип</span><span class="sxs-lookup"><span data-stu-id="72ed8-108">Type</span></span>           | <span data-ttu-id="72ed8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="72ed8-109">Description</span></span> |
|:---------|:---------------|:------------|
| <span data-ttu-id="72ed8-110">response</span><span class="sxs-lookup"><span data-stu-id="72ed8-110">response</span></span> | <span data-ttu-id="72ed8-111">String</span><span class="sxs-lookup"><span data-stu-id="72ed8-111">String</span></span>         | <span data-ttu-id="72ed8-112">Тип ответа.</span><span class="sxs-lookup"><span data-stu-id="72ed8-112">The response type.</span></span> <span data-ttu-id="72ed8-113">Возможные значения: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span><span class="sxs-lookup"><span data-stu-id="72ed8-113">Possible values are: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span></span>
| <span data-ttu-id="72ed8-114">time</span><span class="sxs-lookup"><span data-stu-id="72ed8-114">time</span></span>     | <span data-ttu-id="72ed8-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72ed8-115">DateTimeOffset</span></span> | <span data-ttu-id="72ed8-p102">Дата и время возвращения ответа. Они представлены в формате ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="72ed8-p102">The date and time that the response was returned. It uses ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>

## <a name="json-representation"></a><span data-ttu-id="72ed8-119">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="72ed8-119">JSON representation</span></span>

<span data-ttu-id="72ed8-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="72ed8-120">Here is a JSON representation of the resource</span></span>

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
