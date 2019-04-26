---
title: Тип ресурса Шифтитем
description: Шифтитем представляет версию смены.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: fd5b3d224e60fc3f21b4d484952c7a2643b02407
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343040"
---
# <a name="shiftitem-resource-type"></a><span data-ttu-id="4fda3-103">Тип ресурса Шифтитем</span><span class="sxs-lookup"><span data-stu-id="4fda3-103">shiftItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4fda3-104">Представляет версию [смены](shift.md).</span><span class="sxs-lookup"><span data-stu-id="4fda3-104">Represents a version of a [shift](shift.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4fda3-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="4fda3-105">Properties</span></span>
| <span data-ttu-id="4fda3-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="4fda3-106">Property</span></span>                         | <span data-ttu-id="4fda3-107">Тип</span><span class="sxs-lookup"><span data-stu-id="4fda3-107">Type</span></span>                    | <span data-ttu-id="4fda3-108">Описание</span><span class="sxs-lookup"><span data-stu-id="4fda3-108">Description</span></span>                                                                             |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="4fda3-109">notes</span><span class="sxs-lookup"><span data-stu-id="4fda3-109">notes</span></span>               | <span data-ttu-id="4fda3-110">string</span><span class="sxs-lookup"><span data-stu-id="4fda3-110">string</span></span>                  | <span data-ttu-id="4fda3-111">Примечания для `shiftItem`.</span><span class="sxs-lookup"><span data-stu-id="4fda3-111">The notes for the `shiftItem`.</span></span>      |
| <span data-ttu-id="4fda3-112">displayName</span><span class="sxs-lookup"><span data-stu-id="4fda3-112">displayName</span></span>               | <span data-ttu-id="4fda3-113">string</span><span class="sxs-lookup"><span data-stu-id="4fda3-113">string</span></span>                  | <span data-ttu-id="4fda3-114">Имя файла `shiftItem`.</span><span class="sxs-lookup"><span data-stu-id="4fda3-114">The name of the `shiftItem`.</span></span> |
| <span data-ttu-id="4fda3-115">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4fda3-115">startDateTime</span></span>               | <span data-ttu-id="4fda3-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4fda3-116">DateTimeOffset</span></span>                  | <span data-ttu-id="4fda3-117">Дата и время начала для `shiftItem`.</span><span class="sxs-lookup"><span data-stu-id="4fda3-117">The start date and time for the `shiftItem`.</span></span> <span data-ttu-id="4fda3-118">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="4fda3-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4fda3-119">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="4fda3-119">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> <span data-ttu-id="4fda3-120">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4fda3-120">Required.</span></span> |
| <span data-ttu-id="4fda3-121">endDateTime</span><span class="sxs-lookup"><span data-stu-id="4fda3-121">endDateTime</span></span>               | <span data-ttu-id="4fda3-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4fda3-122">DateTimeOffset</span></span>                 | <span data-ttu-id="4fda3-123">Дата и время окончания для `shiftItem`.</span><span class="sxs-lookup"><span data-stu-id="4fda3-123">The end date and time for the `shiftItem`.</span></span> <span data-ttu-id="4fda3-124">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4fda3-124">Required.</span></span> <span data-ttu-id="4fda3-125">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="4fda3-125">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4fda3-126">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="4fda3-126">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="4fda3-127">theme</span><span class="sxs-lookup"><span data-stu-id="4fda3-127">theme</span></span> | <span data-ttu-id="4fda3-128">Счедулинтитисеме</span><span class="sxs-lookup"><span data-stu-id="4fda3-128">scheduleEntityTheme</span></span>   |  <span data-ttu-id="4fda3-129">Поддерживаемые цвета: белый; компонентов Интенсив цвет Розов желтый участка Даркблуе; Даркгрин; Даркпурпле; Даркпинк; Даркеллов.</span><span class="sxs-lookup"><span data-stu-id="4fda3-129">Supported colors: white; blue; green; purple; pink; yellow; gray; darkBlue; darkGreen; darkPurple; darkPink; darkYellow.</span></span> |
| <span data-ttu-id="4fda3-130">activities</span><span class="sxs-lookup"><span data-stu-id="4fda3-130">activities</span></span>    | <span data-ttu-id="4fda3-131">Коллекция [шифтактивити](shiftactivity.md)</span><span class="sxs-lookup"><span data-stu-id="4fda3-131">[shiftActivity](shiftactivity.md) collection</span></span>   | <span data-ttu-id="4fda3-132">Добавочная часть сдвига, в которой можно получить сведения о том, когда и где сотрудник наносится на свою смену.</span><span class="sxs-lookup"><span data-stu-id="4fda3-132">An incremental part of a shift which can cover details of when and where an employee is during their shift.</span></span> <span data-ttu-id="4fda3-133">Например, назначение или запланированный перерыв или обед.</span><span class="sxs-lookup"><span data-stu-id="4fda3-133">For example, an assignment or a scheduled break or lunch.</span></span> <span data-ttu-id="4fda3-134">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="4fda3-134">Required.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4fda3-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4fda3-135">JSON representation</span></span>

<span data-ttu-id="4fda3-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4fda3-136">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.shiftItem"
}-->
```json
{
  "displayName": "String",
  "notes": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "theme": "String",
  "activities": [{"@odata.type": "microsoft.graph.shiftActivity"}]
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
  "suppressions": []
}
-->
