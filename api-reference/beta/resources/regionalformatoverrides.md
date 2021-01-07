---
title: Тип ресурса regionalFormatOverrides
description: Ресурс, представляющий переопределения регионального форматирования для календарей, дат и времени.
localization_priority: Normal
author: jasonbro
ms.prod: settings
doc_type: resourcePageType
ms.openlocfilehash: 437b67f6a99017bb20096dbd20451b7662145cbd
ms.sourcegitcommit: 7732d20bd99a125118f7cea146c3f2416879f949
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/07/2021
ms.locfileid: "49777598"
---
# <a name="regionalformatoverrides-resource-type"></a><span data-ttu-id="b0c2c-103">Тип ресурса regionalFormatOverrides</span><span class="sxs-lookup"><span data-stu-id="b0c2c-103">regionalFormatOverrides resource type</span></span>

<span data-ttu-id="b0c2c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0c2c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0c2c-105">Коллекция строк, представляющих переопределения форматирования для календарей, дат и времени.</span><span class="sxs-lookup"><span data-stu-id="b0c2c-105">A collection of strings representing formatting overrides for calendars, dates, and times.</span></span> 

## <a name="properties"></a><span data-ttu-id="b0c2c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b0c2c-106">Properties</span></span>

|<span data-ttu-id="b0c2c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b0c2c-107">Property</span></span>             |<span data-ttu-id="b0c2c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b0c2c-108">Type</span></span>                 |<span data-ttu-id="b0c2c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b0c2c-109">Description</span></span>                                                    |
|---------------------|---------------------|---------------------------------------------------------------|
|<span data-ttu-id="b0c2c-110">calendar</span><span class="sxs-lookup"><span data-stu-id="b0c2c-110">calendar</span></span>             |<span data-ttu-id="b0c2c-111">String</span><span class="sxs-lookup"><span data-stu-id="b0c2c-111">String</span></span>               |<span data-ttu-id="b0c2c-112">Календарь, который необходимо использовать, например григорианский календарь.</span><span class="sxs-lookup"><span data-stu-id="b0c2c-112">The calendar to use, e.g., Gregorian Calendar.</span></span><br><br><span data-ttu-id="b0c2c-113">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b0c2c-113">Returned by default.</span></span>|                   
|<span data-ttu-id="b0c2c-114">firstDayOfWeek</span><span class="sxs-lookup"><span data-stu-id="b0c2c-114">firstDayOfWeek</span></span>       |<span data-ttu-id="b0c2c-115">String</span><span class="sxs-lookup"><span data-stu-id="b0c2c-115">String</span></span>               |<span data-ttu-id="b0c2c-116">Первый день недели, например воскресенье.</span><span class="sxs-lookup"><span data-stu-id="b0c2c-116">The first day of the week to use, e.g., Sunday.</span></span><br><br><span data-ttu-id="b0c2c-117">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b0c2c-117">Returned by default.</span></span>|
|<span data-ttu-id="b0c2c-118">shortDateFormat</span><span class="sxs-lookup"><span data-stu-id="b0c2c-118">shortDateFormat</span></span>      |<span data-ttu-id="b0c2c-119">String</span><span class="sxs-lookup"><span data-stu-id="b0c2c-119">String</span></span>               |<span data-ttu-id="b0c2c-120">Краткий формат даты и времени, используемый для отображения дат.</span><span class="sxs-lookup"><span data-stu-id="b0c2c-120">The short date time format to be used for displaying dates.</span></span><br><br><span data-ttu-id="b0c2c-121">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b0c2c-121">Returned by default.</span></span>|
|<span data-ttu-id="b0c2c-122">longDateFormat</span><span class="sxs-lookup"><span data-stu-id="b0c2c-122">longDateFormat</span></span>       |<span data-ttu-id="b0c2c-123">String</span><span class="sxs-lookup"><span data-stu-id="b0c2c-123">String</span></span>               |<span data-ttu-id="b0c2c-124">Длинный формат даты и времени, используемый для отображения дат.</span><span class="sxs-lookup"><span data-stu-id="b0c2c-124">The long date time format to be used for displaying dates.</span></span><br><br><span data-ttu-id="b0c2c-125">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b0c2c-125">Returned by default.</span></span>|
|<span data-ttu-id="b0c2c-126">shortTimeFormat</span><span class="sxs-lookup"><span data-stu-id="b0c2c-126">shortTimeFormat</span></span>      |<span data-ttu-id="b0c2c-127">String</span><span class="sxs-lookup"><span data-stu-id="b0c2c-127">String</span></span>               |<span data-ttu-id="b0c2c-128">Короткий формат времени, используемый для отображения времени.</span><span class="sxs-lookup"><span data-stu-id="b0c2c-128">The short time format to be used for displaying time.</span></span><br><br><span data-ttu-id="b0c2c-129">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b0c2c-129">Returned by default.</span></span>|
|<span data-ttu-id="b0c2c-130">longTimeFormat</span><span class="sxs-lookup"><span data-stu-id="b0c2c-130">longTimeFormat</span></span>       |<span data-ttu-id="b0c2c-131">String</span><span class="sxs-lookup"><span data-stu-id="b0c2c-131">String</span></span>               |<span data-ttu-id="b0c2c-132">Длинный формат времени, используемый для отображения времени.</span><span class="sxs-lookup"><span data-stu-id="b0c2c-132">The long time format to be used for displaying time.</span></span><br><br><span data-ttu-id="b0c2c-133">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b0c2c-133">Returned by default.</span></span>|
|<span data-ttu-id="b0c2c-134">timeZone</span><span class="sxs-lookup"><span data-stu-id="b0c2c-134">timeZone</span></span>             |<span data-ttu-id="b0c2c-135">String</span><span class="sxs-lookup"><span data-stu-id="b0c2c-135">String</span></span>               |<span data-ttu-id="b0c2c-136">Часовой пояс, используемый для отображения времени.</span><span class="sxs-lookup"><span data-stu-id="b0c2c-136">The timezone to be used for displaying time.</span></span><br><br><span data-ttu-id="b0c2c-137">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b0c2c-137">Returned by default.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b0c2c-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b0c2c-138">JSON representation</span></span>

<span data-ttu-id="b0c2c-139">Ниже приводится определение ресурса в JSON.</span><span class="sxs-lookup"><span data-stu-id="b0c2c-139">The following is a JSON definition of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
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


