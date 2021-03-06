---
title: regionalFormatOverrides resource type
description: Ресурс, представляющий переопределения региональных форматов для календарей, дат и времени.
localization_priority: Normal
author: jasonbro
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 2b4046ad8ec6b2d646d1dc2d93cbe7bed205cbad
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516071"
---
# <a name="regionalformatoverrides-resource-type"></a><span data-ttu-id="0f7a6-103">regionalFormatOverrides resource type</span><span class="sxs-lookup"><span data-stu-id="0f7a6-103">regionalFormatOverrides resource type</span></span>

<span data-ttu-id="0f7a6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f7a6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f7a6-105">Коллекция строк, представляющих переопределения форматирования для календарей, дат и времени.</span><span class="sxs-lookup"><span data-stu-id="0f7a6-105">A collection of strings representing formatting overrides for calendars, dates, and times.</span></span> 

## <a name="properties"></a><span data-ttu-id="0f7a6-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="0f7a6-106">Properties</span></span>

|<span data-ttu-id="0f7a6-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="0f7a6-107">Property</span></span>             |<span data-ttu-id="0f7a6-108">Тип</span><span class="sxs-lookup"><span data-stu-id="0f7a6-108">Type</span></span>                     |<span data-ttu-id="0f7a6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0f7a6-109">Description</span></span>                                                    |
|---------------------|-------------------------|---------------------------------------------------------------|
|<span data-ttu-id="0f7a6-110">calendar</span><span class="sxs-lookup"><span data-stu-id="0f7a6-110">calendar</span></span>             |<span data-ttu-id="0f7a6-111">String</span><span class="sxs-lookup"><span data-stu-id="0f7a6-111">String</span></span>                   |<span data-ttu-id="0f7a6-112">Календарь для использования, например, григорианский календарь.</span><span class="sxs-lookup"><span data-stu-id="0f7a6-112">The calendar to use, e.g., Gregorian Calendar.</span></span><br><br><span data-ttu-id="0f7a6-113">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="0f7a6-113">Returned by default.</span></span>|                   
|<span data-ttu-id="0f7a6-114">firstDayOfWeek</span><span class="sxs-lookup"><span data-stu-id="0f7a6-114">firstDayOfWeek</span></span>       |<span data-ttu-id="0f7a6-115">microsoft.graph.dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="0f7a6-115">microsoft.graph.dayOfWeek</span></span>|<span data-ttu-id="0f7a6-116">Первый день недели в использовании, например, воскресенье.</span><span class="sxs-lookup"><span data-stu-id="0f7a6-116">The first day of the week to use, e.g., Sunday.</span></span><br><br><span data-ttu-id="0f7a6-117">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="0f7a6-117">Returned by default.</span></span>|
|<span data-ttu-id="0f7a6-118">shortDateFormat</span><span class="sxs-lookup"><span data-stu-id="0f7a6-118">shortDateFormat</span></span>      |<span data-ttu-id="0f7a6-119">String</span><span class="sxs-lookup"><span data-stu-id="0f7a6-119">String</span></span>                   |<span data-ttu-id="0f7a6-120">Короткий формат времени даты, который будет использоваться для отображения дат.</span><span class="sxs-lookup"><span data-stu-id="0f7a6-120">The short date time format to be used for displaying dates.</span></span><br><br><span data-ttu-id="0f7a6-121">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="0f7a6-121">Returned by default.</span></span>|
|<span data-ttu-id="0f7a6-122">longDateFormat</span><span class="sxs-lookup"><span data-stu-id="0f7a6-122">longDateFormat</span></span>       |<span data-ttu-id="0f7a6-123">String</span><span class="sxs-lookup"><span data-stu-id="0f7a6-123">String</span></span>                   |<span data-ttu-id="0f7a6-124">Формат времени даты, используемый для отображения дат.</span><span class="sxs-lookup"><span data-stu-id="0f7a6-124">The long date time format to be used for displaying dates.</span></span><br><br><span data-ttu-id="0f7a6-125">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="0f7a6-125">Returned by default.</span></span>|
|<span data-ttu-id="0f7a6-126">shortTimeFormat</span><span class="sxs-lookup"><span data-stu-id="0f7a6-126">shortTimeFormat</span></span>      |<span data-ttu-id="0f7a6-127">String</span><span class="sxs-lookup"><span data-stu-id="0f7a6-127">String</span></span>                   |<span data-ttu-id="0f7a6-128">Короткий формат времени, который будет использоваться для отображения времени.</span><span class="sxs-lookup"><span data-stu-id="0f7a6-128">The short time format to be used for displaying time.</span></span><br><br><span data-ttu-id="0f7a6-129">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="0f7a6-129">Returned by default.</span></span>|
|<span data-ttu-id="0f7a6-130">longTimeFormat</span><span class="sxs-lookup"><span data-stu-id="0f7a6-130">longTimeFormat</span></span>       |<span data-ttu-id="0f7a6-131">String</span><span class="sxs-lookup"><span data-stu-id="0f7a6-131">String</span></span>                   |<span data-ttu-id="0f7a6-132">Формат длительного времени, который будет использоваться для отображения времени.</span><span class="sxs-lookup"><span data-stu-id="0f7a6-132">The long time format to be used for displaying time.</span></span><br><br><span data-ttu-id="0f7a6-133">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="0f7a6-133">Returned by default.</span></span>|
|<span data-ttu-id="0f7a6-134">timeZone</span><span class="sxs-lookup"><span data-stu-id="0f7a6-134">timeZone</span></span>             |<span data-ttu-id="0f7a6-135">String</span><span class="sxs-lookup"><span data-stu-id="0f7a6-135">String</span></span>                   |<span data-ttu-id="0f7a6-136">Часовой пояс, используемый для отображения времени.</span><span class="sxs-lookup"><span data-stu-id="0f7a6-136">The timezone to be used for displaying time.</span></span><br><br><span data-ttu-id="0f7a6-137">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="0f7a6-137">Returned by default.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0f7a6-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0f7a6-138">JSON representation</span></span>

<span data-ttu-id="0f7a6-139">Ниже приводится определение ресурса JSON.</span><span class="sxs-lookup"><span data-stu-id="0f7a6-139">The following is a JSON definition of the resource.</span></span>

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


