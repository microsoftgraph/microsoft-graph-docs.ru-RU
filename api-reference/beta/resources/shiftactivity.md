---
title: Тип ресурса Шифтактивити
description: Представляет действие в смене.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 0a5b877c2c24d1764e9badb44dab1f25143c2dce
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657527"
---
# <a name="shiftactivity-resource-type"></a><span data-ttu-id="6aed7-103">Тип ресурса Шифтактивити</span><span class="sxs-lookup"><span data-stu-id="6aed7-103">shiftActivity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6aed7-104">Представляет действие в смене [](shift.md).</span><span class="sxs-lookup"><span data-stu-id="6aed7-104">Represents an activity in a [shift](shift.md).</span></span>

## <a name="properties"></a><span data-ttu-id="6aed7-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="6aed7-105">Properties</span></span>
| <span data-ttu-id="6aed7-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="6aed7-106">Property</span></span>                         | <span data-ttu-id="6aed7-107">Тип</span><span class="sxs-lookup"><span data-stu-id="6aed7-107">Type</span></span>                    | <span data-ttu-id="6aed7-108">Описание</span><span class="sxs-lookup"><span data-stu-id="6aed7-108">Description</span></span>                                                                                                                                                                        |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="6aed7-109">Предопл</span><span class="sxs-lookup"><span data-stu-id="6aed7-109">isPaid</span></span>               | `bool`                  | <span data-ttu-id="6aed7-110">Указывает, следует `microsoft.graph.user` ли платить за действие в течение этого периода `shift`.</span><span class="sxs-lookup"><span data-stu-id="6aed7-110">Indicates whether the `microsoft.graph.user` should be paid for the activity during their `shift`.</span></span> <span data-ttu-id="6aed7-111">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6aed7-111">Required.</span></span>    |
| <span data-ttu-id="6aed7-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="6aed7-112">startDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="6aed7-113">Дата и время начала для `shiftActivity`.</span><span class="sxs-lookup"><span data-stu-id="6aed7-113">The start date and time for the `shiftActivity`.</span></span> <span data-ttu-id="6aed7-114">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="6aed7-114">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6aed7-115">Например, полночь UTC 1 января 2014: "2014 – 01 – 01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="6aed7-115">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> <span data-ttu-id="6aed7-116">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6aed7-116">Required.</span></span> |
| <span data-ttu-id="6aed7-117">endDateTime</span><span class="sxs-lookup"><span data-stu-id="6aed7-117">endDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="6aed7-118">Дата и время окончания для `shiftActivity`.</span><span class="sxs-lookup"><span data-stu-id="6aed7-118">The end date and time for the `shiftActivity`.</span></span> <span data-ttu-id="6aed7-119">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="6aed7-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6aed7-120">Например, полночь UTC 1 января 2014: "2014 – 01 – 01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="6aed7-120">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> <span data-ttu-id="6aed7-121">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6aed7-121">Required.</span></span>    |
| <span data-ttu-id="6aed7-122">code</span><span class="sxs-lookup"><span data-stu-id="6aed7-122">code</span></span>               | `string`                  | <span data-ttu-id="6aed7-123">Определенный пользователем код для `shiftActivity`.</span><span class="sxs-lookup"><span data-stu-id="6aed7-123">Customer defined code for the `shiftActivity`.</span></span> <span data-ttu-id="6aed7-124">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6aed7-124">Required.</span></span>    |
| <span data-ttu-id="6aed7-125">displayName</span><span class="sxs-lookup"><span data-stu-id="6aed7-125">displayName</span></span>               | `string`                  | <span data-ttu-id="6aed7-126">Имя файла `shiftActivity`.</span><span class="sxs-lookup"><span data-stu-id="6aed7-126">The name of the `shiftActivity`.</span></span> <span data-ttu-id="6aed7-127">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="6aed7-127">Required.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="6aed7-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6aed7-128">JSON representation</span></span>

<span data-ttu-id="6aed7-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6aed7-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.shiftActivity"
}-->
```json
{
  "isPaid": true,
  "startDateTime": "2019-03-11T15:00:00Z",
  "endDateTime": "2019-03-11T15:15:00Z",
  "code": "",
  "displayName": "Lunch"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "shiftActivity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/shiftactivity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
