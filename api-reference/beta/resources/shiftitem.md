---
title: Тип ресурса Шифтитем
description: Шифтитем представляет версию смены.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 7ff829ca0f43124404b4b99b048c9919368b6009
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657709"
---
# <a name="shiftitem-resource-type"></a><span data-ttu-id="d26ad-103">Тип ресурса Шифтитем</span><span class="sxs-lookup"><span data-stu-id="d26ad-103">shiftItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d26ad-104">Представляет версию [смены](shift.md).</span><span class="sxs-lookup"><span data-stu-id="d26ad-104">Represents a version of a [shift](shift.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d26ad-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="d26ad-105">Properties</span></span>
| <span data-ttu-id="d26ad-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="d26ad-106">Property</span></span>                         | <span data-ttu-id="d26ad-107">Тип</span><span class="sxs-lookup"><span data-stu-id="d26ad-107">Type</span></span>                    | <span data-ttu-id="d26ad-108">Описание</span><span class="sxs-lookup"><span data-stu-id="d26ad-108">Description</span></span>                                                                             |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="d26ad-109">notes</span><span class="sxs-lookup"><span data-stu-id="d26ad-109">notes</span></span>               | `string`                  | <span data-ttu-id="d26ad-110">Примечания для `shiftItem`.</span><span class="sxs-lookup"><span data-stu-id="d26ad-110">The notes for the `shiftItem`.</span></span>      |
| <span data-ttu-id="d26ad-111">displayName</span><span class="sxs-lookup"><span data-stu-id="d26ad-111">displayName</span></span>               | `string`                  | <span data-ttu-id="d26ad-112">Имя файла `shiftItem`.</span><span class="sxs-lookup"><span data-stu-id="d26ad-112">The name of the `shiftItem`.</span></span> |
| <span data-ttu-id="d26ad-113">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d26ad-113">startDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="d26ad-114">Дата и время начала для `shiftItem`.</span><span class="sxs-lookup"><span data-stu-id="d26ad-114">The start date and time for the `shiftItem`.</span></span> <span data-ttu-id="d26ad-115">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="d26ad-115">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d26ad-116">Например, полночь UTC 1 января 2014: "2014 – 01 – 01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="d26ad-116">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> <span data-ttu-id="d26ad-117">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d26ad-117">Required.</span></span> |
| <span data-ttu-id="d26ad-118">endDateTime</span><span class="sxs-lookup"><span data-stu-id="d26ad-118">endDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="d26ad-119">Дата и время окончания для `shiftItem`.</span><span class="sxs-lookup"><span data-stu-id="d26ad-119">The end date and time for the `shiftItem`.</span></span> <span data-ttu-id="d26ad-120">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d26ad-120">Required.</span></span> <span data-ttu-id="d26ad-121">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="d26ad-121">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d26ad-122">Например, полночь UTC 1 января 2014: "2014 – 01 – 01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="d26ad-122">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="d26ad-123">theme</span><span class="sxs-lookup"><span data-stu-id="d26ad-123">theme</span></span> | `enum`   |    |  |  | <span data-ttu-id="d26ad-124">Поддерживаемые цвета: белый; компонентов Интенсив цвет Розов желтый участка Даркблуе; Даркгрин; Даркпурпле; Даркпинк; Даркеллов.</span><span class="sxs-lookup"><span data-stu-id="d26ad-124">Supported colors: white; blue; green; purple; pink; yellow; gray; darkBlue; darkGreen; darkPurple; darkPink; darkYellow.</span></span> |
| <span data-ttu-id="d26ad-125">activities</span><span class="sxs-lookup"><span data-stu-id="d26ad-125">activities</span></span>    | `collection([shiftActivity](shiftactivity.md))`    | <span data-ttu-id="d26ad-126">Добавочная часть сдвига, в которой можно получить сведения о том, когда и где сотрудник наносится на свою смену.</span><span class="sxs-lookup"><span data-stu-id="d26ad-126">An incremental part of a shift which can cover details of when and where an employee is during their shift.</span></span> <span data-ttu-id="d26ad-127">Например, назначение или запланированный перерыв или обед.</span><span class="sxs-lookup"><span data-stu-id="d26ad-127">For example, an assignment or a scheduled break or lunch.</span></span> <span data-ttu-id="d26ad-128">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="d26ad-128">Required.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d26ad-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d26ad-129">JSON representation</span></span>

<span data-ttu-id="d26ad-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d26ad-130">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.shiftItem"
}-->
```json
{
  "displayName": "Day shift",
  "notes": "Please do inventory as part of your shift.",
  "startDateTime": "2019-03-11T15:00:00Z",
  "endDateTime": "2019-03-12T00:00:00Z",
  "theme": "blue",
  "activities": [
    {
      "isPaid": true,
      "startDateTime": "2019-03-11T15:00:00Z",
      "endDateTime": "2019-03-11T15:15:00Z",
      "code": "",
      "displayName": "Lunch"
    }
  ]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "shiftItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/shiftitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
