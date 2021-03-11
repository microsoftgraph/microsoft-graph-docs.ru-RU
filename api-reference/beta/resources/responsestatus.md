---
title: Тип ресурса responseStatus
description: Состояние ответа к приглашению на собрание.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: harini84
ms.openlocfilehash: 0ee9c70baa5cdea45868feb1517623081f2b62b2
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50718473"
---
# <a name="responsestatus-resource-type"></a><span data-ttu-id="1f37b-103">Тип ресурса responseStatus</span><span class="sxs-lookup"><span data-stu-id="1f37b-103">responseStatus resource type</span></span>

<span data-ttu-id="1f37b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f37b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f37b-105">Состояние ответа к приглашению на собрание.</span><span class="sxs-lookup"><span data-stu-id="1f37b-105">The response status of a meeting request.</span></span>

## <a name="properties"></a><span data-ttu-id="1f37b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="1f37b-106">Properties</span></span>

| <span data-ttu-id="1f37b-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="1f37b-107">Property</span></span> | <span data-ttu-id="1f37b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="1f37b-108">Type</span></span>           | <span data-ttu-id="1f37b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1f37b-109">Description</span></span> |
|:---------|:---------------|:------------|
| <span data-ttu-id="1f37b-110">response</span><span class="sxs-lookup"><span data-stu-id="1f37b-110">response</span></span> | <span data-ttu-id="1f37b-111">String</span><span class="sxs-lookup"><span data-stu-id="1f37b-111">String</span></span>         | <span data-ttu-id="1f37b-112">Тип ответа.</span><span class="sxs-lookup"><span data-stu-id="1f37b-112">The response type.</span></span> <span data-ttu-id="1f37b-113">Возможные значения: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span><span class="sxs-lookup"><span data-stu-id="1f37b-113">Possible values are: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span></span>
| <span data-ttu-id="1f37b-114">time</span><span class="sxs-lookup"><span data-stu-id="1f37b-114">time</span></span>     | <span data-ttu-id="1f37b-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f37b-115">DateTimeOffset</span></span> | <span data-ttu-id="1f37b-116">Дата и время возвращения ответа.</span><span class="sxs-lookup"><span data-stu-id="1f37b-116">The date and time that the response was returned.</span></span> <span data-ttu-id="1f37b-117">Они представлены в формате ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="1f37b-117">It uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1f37b-118">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="1f37b-118">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>

## <a name="json-representation"></a><span data-ttu-id="1f37b-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1f37b-119">JSON representation</span></span>

<span data-ttu-id="1f37b-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1f37b-120">Here is a JSON representation of the resource</span></span>

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


