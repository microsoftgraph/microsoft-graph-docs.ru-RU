---
title: Тип ресурса Шифтактивити
description: Представляет действие в смене.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 24946630e9bc3ae9ba418f5c322ab212c022d6d1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343098"
---
# <a name="shiftactivity-resource-type"></a><span data-ttu-id="0827f-103">Тип ресурса Шифтактивити</span><span class="sxs-lookup"><span data-stu-id="0827f-103">shiftActivity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0827f-104">Представляет действие в смене [](shift.md).</span><span class="sxs-lookup"><span data-stu-id="0827f-104">Represents an activity in a [shift](shift.md).</span></span>

## <a name="properties"></a><span data-ttu-id="0827f-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="0827f-105">Properties</span></span>
| <span data-ttu-id="0827f-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="0827f-106">Property</span></span>                         | <span data-ttu-id="0827f-107">Тип</span><span class="sxs-lookup"><span data-stu-id="0827f-107">Type</span></span>                    | <span data-ttu-id="0827f-108">Описание</span><span class="sxs-lookup"><span data-stu-id="0827f-108">Description</span></span>                                                                                                                                                                        |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="0827f-109">Предопл</span><span class="sxs-lookup"><span data-stu-id="0827f-109">isPaid</span></span>               | `bool`                  | <span data-ttu-id="0827f-110">Указывает, следует `microsoft.graph.user` ли платить за действие в течение этого периода `shift`.</span><span class="sxs-lookup"><span data-stu-id="0827f-110">Indicates whether the `microsoft.graph.user` should be paid for the activity during their `shift`.</span></span> <span data-ttu-id="0827f-111">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0827f-111">Required.</span></span>    |
| <span data-ttu-id="0827f-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="0827f-112">startDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="0827f-113">Дата и время начала для `shiftActivity`.</span><span class="sxs-lookup"><span data-stu-id="0827f-113">The start date and time for the `shiftActivity`.</span></span> <span data-ttu-id="0827f-114">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="0827f-114">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0827f-115">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="0827f-115">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> <span data-ttu-id="0827f-116">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0827f-116">Required.</span></span> |
| <span data-ttu-id="0827f-117">endDateTime</span><span class="sxs-lookup"><span data-stu-id="0827f-117">endDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="0827f-118">Дата и время окончания для `shiftActivity`.</span><span class="sxs-lookup"><span data-stu-id="0827f-118">The end date and time for the `shiftActivity`.</span></span> <span data-ttu-id="0827f-119">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="0827f-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0827f-120">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="0827f-120">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> <span data-ttu-id="0827f-121">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0827f-121">Required.</span></span>    |
| <span data-ttu-id="0827f-122">code</span><span class="sxs-lookup"><span data-stu-id="0827f-122">code</span></span>               | `string`                  | <span data-ttu-id="0827f-123">Определенный пользователем код для `shiftActivity`.</span><span class="sxs-lookup"><span data-stu-id="0827f-123">Customer defined code for the `shiftActivity`.</span></span> <span data-ttu-id="0827f-124">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0827f-124">Required.</span></span>    |
| <span data-ttu-id="0827f-125">displayName</span><span class="sxs-lookup"><span data-stu-id="0827f-125">displayName</span></span>               | `string`                  | <span data-ttu-id="0827f-126">Имя файла `shiftActivity`.</span><span class="sxs-lookup"><span data-stu-id="0827f-126">The name of the `shiftActivity`.</span></span> <span data-ttu-id="0827f-127">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="0827f-127">Required.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="0827f-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0827f-128">JSON representation</span></span>

<span data-ttu-id="0827f-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0827f-129">Here is a JSON representation of the resource.</span></span>

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
