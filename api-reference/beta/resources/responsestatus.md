---
title: Тип ресурса responseStatus
description: Состояние ответа к приглашению на собрание.
localization_priority: Normal
ms.openlocfilehash: 270c432235b929af2cb55ff63e10397fea5f92fb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528076"
---
# <a name="responsestatus-resource-type"></a><span data-ttu-id="39003-103">Тип ресурса responseStatus</span><span class="sxs-lookup"><span data-stu-id="39003-103">responseStatus resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39003-104">Состояние ответа к приглашению на собрание.</span><span class="sxs-lookup"><span data-stu-id="39003-104">The response status of a meeting request.</span></span>

## <a name="properties"></a><span data-ttu-id="39003-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="39003-105">Properties</span></span>

| <span data-ttu-id="39003-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="39003-106">Property</span></span> | <span data-ttu-id="39003-107">Тип</span><span class="sxs-lookup"><span data-stu-id="39003-107">Type</span></span>           | <span data-ttu-id="39003-108">Описание</span><span class="sxs-lookup"><span data-stu-id="39003-108">Description</span></span> |
|:---------|:---------------|:------------|
| <span data-ttu-id="39003-109">response</span><span class="sxs-lookup"><span data-stu-id="39003-109">response</span></span> | <span data-ttu-id="39003-110">String</span><span class="sxs-lookup"><span data-stu-id="39003-110">String</span></span>         | <span data-ttu-id="39003-111">Тип ответа.</span><span class="sxs-lookup"><span data-stu-id="39003-111">The response type.</span></span> <span data-ttu-id="39003-112">Возможные значения: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span><span class="sxs-lookup"><span data-stu-id="39003-112">Possible values are: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span></span>
| <span data-ttu-id="39003-113">time</span><span class="sxs-lookup"><span data-stu-id="39003-113">time</span></span>     | <span data-ttu-id="39003-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39003-114">DateTimeOffset</span></span> | <span data-ttu-id="39003-p102">Дата и время возвращения ответа. Они представлены в формате ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="39003-p102">The date and time that the response was returned. It uses ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>

## <a name="json-representation"></a><span data-ttu-id="39003-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="39003-118">JSON representation</span></span>

<span data-ttu-id="39003-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="39003-119">Here is a JSON representation of the resource</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/responsestatus.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
