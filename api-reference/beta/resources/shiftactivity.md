---
title: Тип ресурса Шифтактивити
description: Представляет действие в смене.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 0a5b877c2c24d1764e9badb44dab1f25143c2dce
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583785"
---
# <a name="shiftactivity-resource-type"></a><span data-ttu-id="121c4-103">Тип ресурса Шифтактивити</span><span class="sxs-lookup"><span data-stu-id="121c4-103">shiftActivity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="121c4-104">Представляет действие в смене [](shift.md).</span><span class="sxs-lookup"><span data-stu-id="121c4-104">Represents an activity in a [shift](shift.md).</span></span>

## <a name="properties"></a><span data-ttu-id="121c4-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="121c4-105">Properties</span></span>
| <span data-ttu-id="121c4-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="121c4-106">Property</span></span>                         | <span data-ttu-id="121c4-107">Тип</span><span class="sxs-lookup"><span data-stu-id="121c4-107">Type</span></span>                    | <span data-ttu-id="121c4-108">Описание</span><span class="sxs-lookup"><span data-stu-id="121c4-108">Description</span></span>                                                                                                                                                                        |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="121c4-109">Предопл</span><span class="sxs-lookup"><span data-stu-id="121c4-109">isPaid</span></span>               | `bool`                  | <span data-ttu-id="121c4-110">Указывает, следует `microsoft.graph.user` ли платить за действие в течение этого периода `shift`.</span><span class="sxs-lookup"><span data-stu-id="121c4-110">Indicates whether the `microsoft.graph.user` should be paid for the activity during their `shift`.</span></span> <span data-ttu-id="121c4-111">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="121c4-111">Required.</span></span>    |
| <span data-ttu-id="121c4-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="121c4-112">startDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="121c4-113">Дата и время начала для `shiftActivity`.</span><span class="sxs-lookup"><span data-stu-id="121c4-113">The start date and time for the `shiftActivity`.</span></span> <span data-ttu-id="121c4-114">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="121c4-114">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="121c4-115">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="121c4-115">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> <span data-ttu-id="121c4-116">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="121c4-116">Required.</span></span> |
| <span data-ttu-id="121c4-117">endDateTime</span><span class="sxs-lookup"><span data-stu-id="121c4-117">endDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="121c4-118">Дата и время окончания для `shiftActivity`.</span><span class="sxs-lookup"><span data-stu-id="121c4-118">The end date and time for the `shiftActivity`.</span></span> <span data-ttu-id="121c4-119">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="121c4-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="121c4-120">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="121c4-120">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> <span data-ttu-id="121c4-121">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="121c4-121">Required.</span></span>    |
| <span data-ttu-id="121c4-122">code</span><span class="sxs-lookup"><span data-stu-id="121c4-122">code</span></span>               | `string`                  | <span data-ttu-id="121c4-123">Определенный пользователем код для `shiftActivity`.</span><span class="sxs-lookup"><span data-stu-id="121c4-123">Customer defined code for the `shiftActivity`.</span></span> <span data-ttu-id="121c4-124">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="121c4-124">Required.</span></span>    |
| <span data-ttu-id="121c4-125">displayName</span><span class="sxs-lookup"><span data-stu-id="121c4-125">displayName</span></span>               | `string`                  | <span data-ttu-id="121c4-126">Имя файла `shiftActivity`.</span><span class="sxs-lookup"><span data-stu-id="121c4-126">The name of the `shiftActivity`.</span></span> <span data-ttu-id="121c4-127">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="121c4-127">Required.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="121c4-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="121c4-128">JSON representation</span></span>

<span data-ttu-id="121c4-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="121c4-129">Here is a JSON representation of the resource.</span></span>

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
