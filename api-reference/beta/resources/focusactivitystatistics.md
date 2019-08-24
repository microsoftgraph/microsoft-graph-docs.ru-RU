---
title: Тип ресурса Фокусактивитистатистикс
description: Представляет сведения об индивидуальных трудозатратах для пользователей
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 11ca850dc7aa24c17f485eb628c7e574bbd4ff4c
ms.sourcegitcommit: 83a053067f6248fb49ec5d473738ab1555fb4295
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/24/2019
ms.locfileid: "36622609"
---
# <a name="focusactivitystatistics-resource-type"></a><span data-ttu-id="e1ea7-103">Тип ресурса Фокусактивитистатистикс</span><span class="sxs-lookup"><span data-stu-id="e1ea7-103">focusActivityStatistics resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1ea7-104">Представляет данные о времени, доступном пользователю, для работы с фокусом.</span><span class="sxs-lookup"><span data-stu-id="e1ea7-104">Represents data about the user's time available for focus work.</span></span> <span data-ttu-id="e1ea7-105">Это основано на [активитистатистикс](../resources/activitystatistics.md).</span><span class="sxs-lookup"><span data-stu-id="e1ea7-105">This is based on [activityStatistics](../resources/activitystatistics.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e1ea7-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e1ea7-106">Properties</span></span>

| <span data-ttu-id="e1ea7-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e1ea7-107">Property</span></span>     | <span data-ttu-id="e1ea7-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e1ea7-108">Type</span></span>        | <span data-ttu-id="e1ea7-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e1ea7-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e1ea7-110">activity</span><span class="sxs-lookup"><span data-stu-id="e1ea7-110">activity</span></span>|<span data-ttu-id="e1ea7-111">аналитиксактивититипе</span><span class="sxs-lookup"><span data-stu-id="e1ea7-111">analyticsActivityType</span></span>| <span data-ttu-id="e1ea7-112">Действие фокуса, для которого возвращается статистика.</span><span class="sxs-lookup"><span data-stu-id="e1ea7-112">Focus activity for which statistics are returned.</span></span>|
|<span data-ttu-id="e1ea7-113">duration</span><span class="sxs-lookup"><span data-stu-id="e1ea7-113">duration</span></span>|<span data-ttu-id="e1ea7-114">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="e1ea7-114">Duration</span></span>|<span data-ttu-id="e1ea7-115">Общая сумма количества часов в фокусе, равная всем блокам времени по крайней мере в два последовательных часа, в календаре Microsoft Outlook пользователя без собрания с другими людьми в рабочем времени пользователя.</span><span class="sxs-lookup"><span data-stu-id="e1ea7-115">Total sum of focus hours, which is equal to all time blocks of at least two consecutive hours, in a user's Microsoft Outlook calendar without a meeting with other people within the user's set work hours.</span></span> <span data-ttu-id="e1ea7-116">Значение представляется в формате ISO 8601 для длительности.</span><span class="sxs-lookup"><span data-stu-id="e1ea7-116">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="e1ea7-117">endDate</span><span class="sxs-lookup"><span data-stu-id="e1ea7-117">endDate</span></span>|<span data-ttu-id="e1ea7-118">Date</span><span class="sxs-lookup"><span data-stu-id="e1ea7-118">Date</span></span>|<span data-ttu-id="e1ea7-119">Дата окончания действия фокуса.</span><span class="sxs-lookup"><span data-stu-id="e1ea7-119">Date when the focus activity ended.</span></span> <span data-ttu-id="e1ea7-120">Значение представлено в формате ISO 8601 для календарных дат.</span><span class="sxs-lookup"><span data-stu-id="e1ea7-120">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="e1ea7-121">Например, значение свойства может иметь значение "2019-07-04", которое соответствует формату ГГГГ – MM – DD.</span><span class="sxs-lookup"><span data-stu-id="e1ea7-121">For example, the property value could be "2019-07-04" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="e1ea7-122">id</span><span class="sxs-lookup"><span data-stu-id="e1ea7-122">id</span></span>|<span data-ttu-id="e1ea7-123">String</span><span class="sxs-lookup"><span data-stu-id="e1ea7-123">String</span></span>| <span data-ttu-id="e1ea7-124">Идентификатор, предназначенный только для чтения, для действия Focus.</span><span class="sxs-lookup"><span data-stu-id="e1ea7-124">Read-only ID for the focus activity.</span></span>|
|<span data-ttu-id="e1ea7-125">startDate</span><span class="sxs-lookup"><span data-stu-id="e1ea7-125">startDate</span></span>|<span data-ttu-id="e1ea7-126">Дата</span><span class="sxs-lookup"><span data-stu-id="e1ea7-126">Date</span></span>|<span data-ttu-id="e1ea7-127">Дата начала действия фокуса.</span><span class="sxs-lookup"><span data-stu-id="e1ea7-127">Date when the focus activity started.</span></span> <span data-ttu-id="e1ea7-128">Значение представлено в формате ISO 8601 для календарных дат.</span><span class="sxs-lookup"><span data-stu-id="e1ea7-128">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="e1ea7-129">Например, значение свойства может иметь значение "2019-07-03", которое соответствует формату ГГГГ – MM – DD.</span><span class="sxs-lookup"><span data-stu-id="e1ea7-129">For example, the property value could be "2019-07-03" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="e1ea7-130">тимезонеусед</span><span class="sxs-lookup"><span data-stu-id="e1ea7-130">timeZoneUsed</span></span>|<span data-ttu-id="e1ea7-131">String.</span><span class="sxs-lookup"><span data-stu-id="e1ea7-131">String</span></span>|<span data-ttu-id="e1ea7-132">Часовой пояс, который пользователь задает в календаре Outlook для вычисления.</span><span class="sxs-lookup"><span data-stu-id="e1ea7-132">The time zone that the user sets in Outlook calendar is used for the computation.</span></span> <span data-ttu-id="e1ea7-133">Например, значение свойства может быть "тихоокеанское стандартное время".</span><span class="sxs-lookup"><span data-stu-id="e1ea7-133">For example, the property value could be "Pacific Standard Time."</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1ea7-134">Отношения</span><span class="sxs-lookup"><span data-stu-id="e1ea7-134">Relationships</span></span>

<span data-ttu-id="e1ea7-135">Нет</span><span class="sxs-lookup"><span data-stu-id="e1ea7-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e1ea7-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e1ea7-136">JSON representation</span></span>

<span data-ttu-id="e1ea7-137">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e1ea7-137">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.activityStatistics",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.focusActivityStatistics"
}--> 

```json
{
  "activity": "string",
  "duration": "String (ISO 8601 duration)",
  "endDate": "String (ISO 8601)",
  "id": "String (identifier)",
  "startDate": "String (ISO 8601)",
  "timeZoneUsed": "String"
  }
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "focusActivityStatistics resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->