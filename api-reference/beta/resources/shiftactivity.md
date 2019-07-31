---
title: Тип ресурса Шифтактивити
description: Представляет действие в смене.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 8acfb16235c90cf6067ad5fd6c5d8e82ae239f8d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965077"
---
# <a name="shiftactivity-resource-type"></a><span data-ttu-id="b9cbd-103">Тип ресурса Шифтактивити</span><span class="sxs-lookup"><span data-stu-id="b9cbd-103">shiftActivity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9cbd-104">Представляет действие в смене [](shift.md).</span><span class="sxs-lookup"><span data-stu-id="b9cbd-104">Represents an activity in a [shift](shift.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b9cbd-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="b9cbd-105">Properties</span></span>
| <span data-ttu-id="b9cbd-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="b9cbd-106">Property</span></span>                         | <span data-ttu-id="b9cbd-107">Тип</span><span class="sxs-lookup"><span data-stu-id="b9cbd-107">Type</span></span>                    | <span data-ttu-id="b9cbd-108">Описание</span><span class="sxs-lookup"><span data-stu-id="b9cbd-108">Description</span></span>                                                                                                                                                                        |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="b9cbd-109">Предопл</span><span class="sxs-lookup"><span data-stu-id="b9cbd-109">isPaid</span></span>               | `bool`                  | <span data-ttu-id="b9cbd-110">Указывает, следует `microsoft.graph.user` ли платить за действие в течение этого периода `shift`.</span><span class="sxs-lookup"><span data-stu-id="b9cbd-110">Indicates whether the `microsoft.graph.user` should be paid for the activity during their `shift`.</span></span> <span data-ttu-id="b9cbd-111">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="b9cbd-111">Required.</span></span>    |
| <span data-ttu-id="b9cbd-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b9cbd-112">startDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="b9cbd-113">Дата и время начала для `shiftActivity`.</span><span class="sxs-lookup"><span data-stu-id="b9cbd-113">The start date and time for the `shiftActivity`.</span></span> <span data-ttu-id="b9cbd-114">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="b9cbd-114">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b9cbd-115">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="b9cbd-115">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> <span data-ttu-id="b9cbd-116">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="b9cbd-116">Required.</span></span> |
| <span data-ttu-id="b9cbd-117">endDateTime</span><span class="sxs-lookup"><span data-stu-id="b9cbd-117">endDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="b9cbd-118">Дата и время окончания для `shiftActivity`.</span><span class="sxs-lookup"><span data-stu-id="b9cbd-118">The end date and time for the `shiftActivity`.</span></span> <span data-ttu-id="b9cbd-119">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="b9cbd-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b9cbd-120">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="b9cbd-120">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> <span data-ttu-id="b9cbd-121">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="b9cbd-121">Required.</span></span>    |
| <span data-ttu-id="b9cbd-122">code</span><span class="sxs-lookup"><span data-stu-id="b9cbd-122">code</span></span>               | `string`                  | <span data-ttu-id="b9cbd-123">Определенный пользователем код для `shiftActivity`.</span><span class="sxs-lookup"><span data-stu-id="b9cbd-123">Customer defined code for the `shiftActivity`.</span></span> <span data-ttu-id="b9cbd-124">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b9cbd-124">Required.</span></span>    |
| <span data-ttu-id="b9cbd-125">displayName</span><span class="sxs-lookup"><span data-stu-id="b9cbd-125">displayName</span></span>               | `string`                  | <span data-ttu-id="b9cbd-126">Имя файла `shiftActivity`.</span><span class="sxs-lookup"><span data-stu-id="b9cbd-126">The name of the `shiftActivity`.</span></span> <span data-ttu-id="b9cbd-127">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="b9cbd-127">Required.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="b9cbd-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b9cbd-128">JSON representation</span></span>

<span data-ttu-id="b9cbd-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b9cbd-129">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
