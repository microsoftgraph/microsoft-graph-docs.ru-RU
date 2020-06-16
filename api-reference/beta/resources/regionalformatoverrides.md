---
title: Тип ресурса Регионалформатоверридес
description: Ресурс, представляющий региональные параметры форматирования для календарей, дат и времени.
localization_priority: Normal
author: jasonbro
ms.prod: settings
doc_type: resourcePageType
ms.openlocfilehash: add353f539cac8eb6bb0bc7997c7aaaeea450835
ms.sourcegitcommit: 3c8a92d89ac60a48cb63449976b1c3c2c6302281
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/16/2020
ms.locfileid: "44744230"
---
# <a name="regionalformatoverrides-resource-type"></a><span data-ttu-id="5a237-103">Тип ресурса Регионалформатоверридес</span><span class="sxs-lookup"><span data-stu-id="5a237-103">regionalFormatOverrides resource type</span></span>

<span data-ttu-id="5a237-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a237-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a237-105">Коллекция строк, представляющих переопределения форматирования для календарей, дат и времени.</span><span class="sxs-lookup"><span data-stu-id="5a237-105">A collection of strings representing formatting overrides for calendars, dates, and times.</span></span> 

## <a name="properties"></a><span data-ttu-id="5a237-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="5a237-106">Properties</span></span>

|<span data-ttu-id="5a237-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="5a237-107">Property</span></span>             |<span data-ttu-id="5a237-108">Тип</span><span class="sxs-lookup"><span data-stu-id="5a237-108">Type</span></span>                 |<span data-ttu-id="5a237-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5a237-109">Description</span></span>                                                    |
|---------------------|---------------------|---------------------------------------------------------------|
|<span data-ttu-id="5a237-110">calendar</span><span class="sxs-lookup"><span data-stu-id="5a237-110">calendar</span></span>             |<span data-ttu-id="5a237-111">String</span><span class="sxs-lookup"><span data-stu-id="5a237-111">String</span></span>               |<span data-ttu-id="5a237-112">Используемый календарь, например, григорианский календарь.</span><span class="sxs-lookup"><span data-stu-id="5a237-112">The calendar to use, e.g., Gregorian Calendar.</span></span><br><br><span data-ttu-id="5a237-113">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5a237-113">Returned by default.</span></span>|                   
|<span data-ttu-id="5a237-114">firstDayOfWeek</span><span class="sxs-lookup"><span data-stu-id="5a237-114">firstDayOfWeek</span></span>       |<span data-ttu-id="5a237-115">String</span><span class="sxs-lookup"><span data-stu-id="5a237-115">String</span></span>               |<span data-ttu-id="5a237-116">Первый день недели, который необходимо использовать, например, воскресенье.</span><span class="sxs-lookup"><span data-stu-id="5a237-116">The first day of the week to use, e.g., Sunday.</span></span><br><br><span data-ttu-id="5a237-117">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5a237-117">Returned by default.</span></span>|
|<span data-ttu-id="5a237-118">шортдатеформат</span><span class="sxs-lookup"><span data-stu-id="5a237-118">shortDateFormat</span></span>      |<span data-ttu-id="5a237-119">String</span><span class="sxs-lookup"><span data-stu-id="5a237-119">String</span></span>               |<span data-ttu-id="5a237-120">Краткий формат даты и времени, используемый для отображения дат.</span><span class="sxs-lookup"><span data-stu-id="5a237-120">The short date time format to be used for displaying dates.</span></span><br><br><span data-ttu-id="5a237-121">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5a237-121">Returned by default.</span></span>|
|<span data-ttu-id="5a237-122">лонгдатеформат</span><span class="sxs-lookup"><span data-stu-id="5a237-122">longDateFormat</span></span>       |<span data-ttu-id="5a237-123">String</span><span class="sxs-lookup"><span data-stu-id="5a237-123">String</span></span>               |<span data-ttu-id="5a237-124">Длинный формат даты и времени, используемый для отображения дат.</span><span class="sxs-lookup"><span data-stu-id="5a237-124">The long date time format to be used for displaying dates.</span></span><br><br><span data-ttu-id="5a237-125">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5a237-125">Returned by default.</span></span>|
|<span data-ttu-id="5a237-126">шорттимеформат</span><span class="sxs-lookup"><span data-stu-id="5a237-126">shortTimeFormat</span></span>      |<span data-ttu-id="5a237-127">String</span><span class="sxs-lookup"><span data-stu-id="5a237-127">String</span></span>               |<span data-ttu-id="5a237-128">Краткий формат времени, используемый для отображения времени.</span><span class="sxs-lookup"><span data-stu-id="5a237-128">The short time format to be used for displaying time.</span></span><br><br><span data-ttu-id="5a237-129">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5a237-129">Returned by default.</span></span>|
|<span data-ttu-id="5a237-130">лонгтимеформат</span><span class="sxs-lookup"><span data-stu-id="5a237-130">longTimeFormat</span></span>       |<span data-ttu-id="5a237-131">String</span><span class="sxs-lookup"><span data-stu-id="5a237-131">String</span></span>               |<span data-ttu-id="5a237-132">Длинный формат времени, используемый для отображения времени.</span><span class="sxs-lookup"><span data-stu-id="5a237-132">The long time format to be used for displaying time.</span></span><br><br><span data-ttu-id="5a237-133">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5a237-133">Returned by default.</span></span>|
|<span data-ttu-id="5a237-134">timeZone</span><span class="sxs-lookup"><span data-stu-id="5a237-134">timeZone</span></span>             |<span data-ttu-id="5a237-135">String</span><span class="sxs-lookup"><span data-stu-id="5a237-135">String</span></span>               |<span data-ttu-id="5a237-136">Часовой пояс, используемый для отображения времени.</span><span class="sxs-lookup"><span data-stu-id="5a237-136">The timezone to be used for displaying time.</span></span><br><br><span data-ttu-id="5a237-137">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5a237-137">Returned by default.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5a237-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5a237-138">JSON representation</span></span>

<span data-ttu-id="5a237-139">Ниже приведено определение ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5a237-139">The following is a JSON definition of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "",
  "@odata.type": "microsoft.graph.regionalFormatOverrides"
}-->

```json
{
    "calendar": "string",
    "firstDayOfWeek": "string",
    "shortDateFormat": "string",
    "longDateFormat": "string",
    "shortTimeFormat": "string",
    "longTimeFormat": "string",
    "timeZone": "string"
}
```
<!-- {
  "type": "#page.annotation",
  "description": "regionalFormatOverride resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
