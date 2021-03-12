---
title: тип ресурса shiftActivity
description: Представляет действие в сдвиге.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 30552f0a5c856d0144fd231cda6b9e1aa825d97f
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721798"
---
# <a name="shiftactivity-resource-type"></a><span data-ttu-id="a4988-103">тип ресурса shiftActivity</span><span class="sxs-lookup"><span data-stu-id="a4988-103">shiftActivity resource type</span></span>

<span data-ttu-id="a4988-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4988-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4988-105">Представляет действие в [сдвиге.](shift.md)</span><span class="sxs-lookup"><span data-stu-id="a4988-105">Represents an activity in a [shift](shift.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a4988-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a4988-106">Properties</span></span>
| <span data-ttu-id="a4988-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a4988-107">Property</span></span>                         | <span data-ttu-id="a4988-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a4988-108">Type</span></span>                    | <span data-ttu-id="a4988-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a4988-109">Description</span></span>                                                                                                                                                                        |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="a4988-110">isPaid</span><span class="sxs-lookup"><span data-stu-id="a4988-110">isPaid</span></span>               | `bool`                  | <span data-ttu-id="a4988-111">Указывает, следует ли платить за действия во `microsoft.graph.user` время их `shift` .</span><span class="sxs-lookup"><span data-stu-id="a4988-111">Indicates whether the `microsoft.graph.user` should be paid for the activity during their `shift`.</span></span> <span data-ttu-id="a4988-112">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4988-112">Required.</span></span>    |
| <span data-ttu-id="a4988-113">startDateTime</span><span class="sxs-lookup"><span data-stu-id="a4988-113">startDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="a4988-114">Дата и время начала для ресурса `shiftActivity`.</span><span class="sxs-lookup"><span data-stu-id="a4988-114">The start date and time for the `shiftActivity`.</span></span> <span data-ttu-id="a4988-115">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="a4988-115">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a4988-116">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="a4988-116">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="a4988-117">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="a4988-117">Required.</span></span> |
| <span data-ttu-id="a4988-118">endDateTime</span><span class="sxs-lookup"><span data-stu-id="a4988-118">endDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="a4988-119">Дата и время окончания для ресурса `shiftActivity`.</span><span class="sxs-lookup"><span data-stu-id="a4988-119">The end date and time for the `shiftActivity`.</span></span> <span data-ttu-id="a4988-120">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="a4988-120">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a4988-121">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="a4988-121">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="a4988-122">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4988-122">Required.</span></span>    |
| <span data-ttu-id="a4988-123">code</span><span class="sxs-lookup"><span data-stu-id="a4988-123">code</span></span>               | `string`                  | <span data-ttu-id="a4988-124">Код, определенный клиентом `shiftActivity` для .</span><span class="sxs-lookup"><span data-stu-id="a4988-124">Customer defined code for the `shiftActivity`.</span></span> <span data-ttu-id="a4988-125">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4988-125">Required.</span></span>    |
| <span data-ttu-id="a4988-126">displayName</span><span class="sxs-lookup"><span data-stu-id="a4988-126">displayName</span></span>               | `string`                  | <span data-ttu-id="a4988-127">Имя ресурса `shiftActivity`.</span><span class="sxs-lookup"><span data-stu-id="a4988-127">The name of the `shiftActivity`.</span></span> <span data-ttu-id="a4988-128">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="a4988-128">Required.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="a4988-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a4988-129">JSON representation</span></span>

<span data-ttu-id="a4988-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a4988-130">Here is a JSON representation of the resource.</span></span>

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

