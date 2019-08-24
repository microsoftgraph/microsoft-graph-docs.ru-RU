---
title: Тип ресурса Чатактивитистатистикс
description: Представляет сведения о действиях в чате для пользователей.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 05003110c397932f27e700c119f3926b44fe7c31
ms.sourcegitcommit: 83a053067f6248fb49ec5d473738ab1555fb4295
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/24/2019
ms.locfileid: "36622644"
---
# <a name="chatactivitystatistics-resource-type"></a><span data-ttu-id="45b4e-103">Тип ресурса Чатактивитистатистикс</span><span class="sxs-lookup"><span data-stu-id="45b4e-103">chatActivityStatistics resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45b4e-104">Представляет данные о времени пользователя, затраченного на действия в чате, в Microsoft Teams или Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="45b4e-104">Represents data about the user's time spent in chat activities on Microsoft Teams or Skype for Business.</span></span> <span data-ttu-id="45b4e-105">Это основано на [активитистатистикс](../resources/activitystatistics.md).</span><span class="sxs-lookup"><span data-stu-id="45b4e-105">This is based on [activityStatistics](../resources/activitystatistics.md).</span></span>

## <a name="properties"></a><span data-ttu-id="45b4e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="45b4e-106">Properties</span></span>

| <span data-ttu-id="45b4e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="45b4e-107">Property</span></span>     | <span data-ttu-id="45b4e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="45b4e-108">Type</span></span>        | <span data-ttu-id="45b4e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="45b4e-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="45b4e-110">activity</span><span class="sxs-lookup"><span data-stu-id="45b4e-110">activity</span></span>|<span data-ttu-id="45b4e-111">аналитиксактивититипе</span><span class="sxs-lookup"><span data-stu-id="45b4e-111">analyticsActivityType</span></span>| <span data-ttu-id="45b4e-112">Действия чата, для которых возвращается статистика.</span><span class="sxs-lookup"><span data-stu-id="45b4e-112">Chat activity for which statistics are returned.</span></span>|
|<span data-ttu-id="45b4e-113">duration</span><span class="sxs-lookup"><span data-stu-id="45b4e-113">duration</span></span>|<span data-ttu-id="45b4e-114">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="45b4e-114">Duration</span></span>|<span data-ttu-id="45b4e-115">Общее количество часов, потраченных на беседы.</span><span class="sxs-lookup"><span data-stu-id="45b4e-115">Total hours spent on chats.</span></span> <span data-ttu-id="45b4e-116">Значение представляется в формате ISO 8601 для длительности.</span><span class="sxs-lookup"><span data-stu-id="45b4e-116">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="45b4e-117">endDate</span><span class="sxs-lookup"><span data-stu-id="45b4e-117">endDate</span></span>|<span data-ttu-id="45b4e-118">Date</span><span class="sxs-lookup"><span data-stu-id="45b4e-118">Date</span></span>|<span data-ttu-id="45b4e-119">Дата окончания действия чата.</span><span class="sxs-lookup"><span data-stu-id="45b4e-119">Date when the chat activity ended.</span></span> <span data-ttu-id="45b4e-120">Значение представлено в формате ISO 8601 для календарных дат.</span><span class="sxs-lookup"><span data-stu-id="45b4e-120">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="45b4e-121">Например, значение свойства может иметь значение "2019-07-04", которое соответствует формату ГГГГ – MM – DD.</span><span class="sxs-lookup"><span data-stu-id="45b4e-121">For example, the property value could be "2019-07-04" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="45b4e-122">id</span><span class="sxs-lookup"><span data-stu-id="45b4e-122">id</span></span>|<span data-ttu-id="45b4e-123">String</span><span class="sxs-lookup"><span data-stu-id="45b4e-123">String</span></span>| <span data-ttu-id="45b4e-124">Идентификатор, предназначенный только для чтения, для действия чата.</span><span class="sxs-lookup"><span data-stu-id="45b4e-124">Read-only ID for the chat activity.</span></span>|
|<span data-ttu-id="45b4e-125">startDate</span><span class="sxs-lookup"><span data-stu-id="45b4e-125">startDate</span></span>|<span data-ttu-id="45b4e-126">Дата</span><span class="sxs-lookup"><span data-stu-id="45b4e-126">Date</span></span>|<span data-ttu-id="45b4e-127">Дата начала действия чата.</span><span class="sxs-lookup"><span data-stu-id="45b4e-127">Date when the chat activity started.</span></span> <span data-ttu-id="45b4e-128">Значение представлено в формате ISO 8601 для календарных дат.</span><span class="sxs-lookup"><span data-stu-id="45b4e-128">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="45b4e-129">Например, значение свойства может иметь значение "2019-07-03", которое соответствует формату ГГГГ – MM – DD.</span><span class="sxs-lookup"><span data-stu-id="45b4e-129">For example, the property value could be "2019-07-03" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="45b4e-130">тимезонеусед</span><span class="sxs-lookup"><span data-stu-id="45b4e-130">timeZoneUsed</span></span>|<span data-ttu-id="45b4e-131">String.</span><span class="sxs-lookup"><span data-stu-id="45b4e-131">String</span></span>|<span data-ttu-id="45b4e-132">Часовой пояс, который пользователь задает в календаре Outlook для вычисления.</span><span class="sxs-lookup"><span data-stu-id="45b4e-132">The time zone that the user sets in Outlook calendar is used for the computation.</span></span> <span data-ttu-id="45b4e-133">Например, значение свойства может быть "тихоокеанское стандартное время".</span><span class="sxs-lookup"><span data-stu-id="45b4e-133">For example, the property value could be "Pacific Standard Time."</span></span>|
|<span data-ttu-id="45b4e-134">афтерхаурс</span><span class="sxs-lookup"><span data-stu-id="45b4e-134">afterHours</span></span>|<span data-ttu-id="45b4e-135">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="45b4e-135">Duration</span></span>|<span data-ttu-id="45b4e-136">Время, затраченное на беседы в нерабочее время, которое основано на параметре календаря Microsoft Outlook пользователя для рабочих часов.</span><span class="sxs-lookup"><span data-stu-id="45b4e-136">Time spent on chats outside of working hours, which is based on the user's Microsoft Outlook calendar setting for work hours.</span></span> <span data-ttu-id="45b4e-137">Значение представляется в формате ISO 8601 для длительности.</span><span class="sxs-lookup"><span data-stu-id="45b4e-137">The value is represented in ISO 8601 format for durations.</span></span> |

## <a name="relationships"></a><span data-ttu-id="45b4e-138">Отношения</span><span class="sxs-lookup"><span data-stu-id="45b4e-138">Relationships</span></span>

<span data-ttu-id="45b4e-139">Нет</span><span class="sxs-lookup"><span data-stu-id="45b4e-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="45b4e-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="45b4e-140">JSON representation</span></span>

<span data-ttu-id="45b4e-141">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="45b4e-141">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.activityStatistics",
  "keyProperty": "id", 
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chatActivityStatistics"
}-->

```json
{
  "activity": "string",
  "duration": "String (ISO 8601 duration)",
  "endDate": "String (ISO 8601)",
  "id": "String (identifier)",
  "startDate": "String (ISO 8601)",
  "timeZoneUsed": "String",
  "afterHours": "String (ISO 8601 duration)"
}

```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chatActivityStatistics resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

