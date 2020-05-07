---
title: Тип ресурса Шифтактивити
description: Представляет действие в смене.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d03cf481ec0360aa6ef7c4ab544189b420b2081b
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154348"
---
# <a name="shiftactivity-resource-type"></a><span data-ttu-id="753a7-103">Тип ресурса Шифтактивити</span><span class="sxs-lookup"><span data-stu-id="753a7-103">shiftActivity resource type</span></span>

<span data-ttu-id="753a7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="753a7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="753a7-105">Представляет действие в [смене](shift.md).</span><span class="sxs-lookup"><span data-stu-id="753a7-105">Represents an activity in a [shift](shift.md).</span></span>

## <a name="properties"></a><span data-ttu-id="753a7-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="753a7-106">Properties</span></span>
| <span data-ttu-id="753a7-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="753a7-107">Property</span></span>                         | <span data-ttu-id="753a7-108">Тип</span><span class="sxs-lookup"><span data-stu-id="753a7-108">Type</span></span>                    | <span data-ttu-id="753a7-109">Описание</span><span class="sxs-lookup"><span data-stu-id="753a7-109">Description</span></span>                                                                                                                                                                        |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="753a7-110">Предопл</span><span class="sxs-lookup"><span data-stu-id="753a7-110">isPaid</span></span>               | `bool`                  | <span data-ttu-id="753a7-111">Указывает, следует `microsoft.graph.user` ли платить за действие в течение этого периода `shift`.</span><span class="sxs-lookup"><span data-stu-id="753a7-111">Indicates whether the `microsoft.graph.user` should be paid for the activity during their `shift`.</span></span> <span data-ttu-id="753a7-112">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="753a7-112">Required.</span></span>    |
| <span data-ttu-id="753a7-113">startDateTime</span><span class="sxs-lookup"><span data-stu-id="753a7-113">startDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="753a7-114">Дата и время начала для ресурса `shiftActivity`.</span><span class="sxs-lookup"><span data-stu-id="753a7-114">The start date and time for the `shiftActivity`.</span></span> <span data-ttu-id="753a7-115">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="753a7-115">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="753a7-116">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="753a7-116">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> <span data-ttu-id="753a7-117">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="753a7-117">Required.</span></span> |
| <span data-ttu-id="753a7-118">endDateTime</span><span class="sxs-lookup"><span data-stu-id="753a7-118">endDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="753a7-119">Дата и время окончания для ресурса `shiftActivity`.</span><span class="sxs-lookup"><span data-stu-id="753a7-119">The end date and time for the `shiftActivity`.</span></span> <span data-ttu-id="753a7-120">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="753a7-120">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="753a7-121">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="753a7-121">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> <span data-ttu-id="753a7-122">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="753a7-122">Required.</span></span>    |
| <span data-ttu-id="753a7-123">code</span><span class="sxs-lookup"><span data-stu-id="753a7-123">code</span></span>               | `string`                  | <span data-ttu-id="753a7-124">Определенный пользователем код для `shiftActivity`.</span><span class="sxs-lookup"><span data-stu-id="753a7-124">Customer defined code for the `shiftActivity`.</span></span> <span data-ttu-id="753a7-125">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="753a7-125">Required.</span></span>    |
| <span data-ttu-id="753a7-126">displayName</span><span class="sxs-lookup"><span data-stu-id="753a7-126">displayName</span></span>               | `string`                  | <span data-ttu-id="753a7-127">Имя ресурса `shiftActivity`.</span><span class="sxs-lookup"><span data-stu-id="753a7-127">The name of the `shiftActivity`.</span></span> <span data-ttu-id="753a7-128">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="753a7-128">Required.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="753a7-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="753a7-129">JSON representation</span></span>

<span data-ttu-id="753a7-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="753a7-130">Here is a JSON representation of the resource.</span></span>

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
