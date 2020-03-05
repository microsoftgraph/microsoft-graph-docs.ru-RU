---
title: Тип ресурса Чатактивитистатистикс
description: Представляет сведения о действиях в чате для пользователей.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 4bcdde44c6bc2d674638e94b778d2a8f82b3c64c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507728"
---
# <a name="chatactivitystatistics-resource-type"></a><span data-ttu-id="2109e-103">Тип ресурса Чатактивитистатистикс</span><span class="sxs-lookup"><span data-stu-id="2109e-103">chatActivityStatistics resource type</span></span>

<span data-ttu-id="2109e-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2109e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2109e-105">Представляет данные о времени пользователя, затраченного на действия в чате, в Microsoft Teams или Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="2109e-105">Represents data about the user's time spent in chat activities on Microsoft Teams or Skype for Business.</span></span> <span data-ttu-id="2109e-106">Это основано на [активитистатистикс](../resources/activitystatistics.md).</span><span class="sxs-lookup"><span data-stu-id="2109e-106">This is based on [activityStatistics](../resources/activitystatistics.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2109e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2109e-107">Properties</span></span>

| <span data-ttu-id="2109e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2109e-108">Property</span></span>     | <span data-ttu-id="2109e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2109e-109">Type</span></span>        | <span data-ttu-id="2109e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2109e-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2109e-111">activity</span><span class="sxs-lookup"><span data-stu-id="2109e-111">activity</span></span>|<span data-ttu-id="2109e-112">аналитиксактивититипе</span><span class="sxs-lookup"><span data-stu-id="2109e-112">analyticsActivityType</span></span>| <span data-ttu-id="2109e-113">Действия чата, для которых возвращается статистика.</span><span class="sxs-lookup"><span data-stu-id="2109e-113">Chat activity for which statistics are returned.</span></span>|
|<span data-ttu-id="2109e-114">duration</span><span class="sxs-lookup"><span data-stu-id="2109e-114">duration</span></span>|<span data-ttu-id="2109e-115">Длительность</span><span class="sxs-lookup"><span data-stu-id="2109e-115">Duration</span></span>|<span data-ttu-id="2109e-116">Общее количество часов, потраченных на беседы.</span><span class="sxs-lookup"><span data-stu-id="2109e-116">Total hours spent on chats.</span></span> <span data-ttu-id="2109e-117">Значение представляется в формате ISO 8601 для длительности.</span><span class="sxs-lookup"><span data-stu-id="2109e-117">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="2109e-118">endDate</span><span class="sxs-lookup"><span data-stu-id="2109e-118">endDate</span></span>|<span data-ttu-id="2109e-119">Date</span><span class="sxs-lookup"><span data-stu-id="2109e-119">Date</span></span>|<span data-ttu-id="2109e-120">Дата окончания действия чата.</span><span class="sxs-lookup"><span data-stu-id="2109e-120">Date when the chat activity ended.</span></span> <span data-ttu-id="2109e-121">Значение представлено в формате ISO 8601 для календарных дат.</span><span class="sxs-lookup"><span data-stu-id="2109e-121">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="2109e-122">Например, значение свойства может иметь значение "2019-07-04", которое соответствует формату ГГГГ – MM – DD.</span><span class="sxs-lookup"><span data-stu-id="2109e-122">For example, the property value could be "2019-07-04" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="2109e-123">id</span><span class="sxs-lookup"><span data-stu-id="2109e-123">id</span></span>|<span data-ttu-id="2109e-124">String</span><span class="sxs-lookup"><span data-stu-id="2109e-124">String</span></span>| <span data-ttu-id="2109e-125">Идентификатор, предназначенный только для чтения, для действия чата.</span><span class="sxs-lookup"><span data-stu-id="2109e-125">Read-only ID for the chat activity.</span></span>|
|<span data-ttu-id="2109e-126">startDate</span><span class="sxs-lookup"><span data-stu-id="2109e-126">startDate</span></span>|<span data-ttu-id="2109e-127">Дата</span><span class="sxs-lookup"><span data-stu-id="2109e-127">Date</span></span>|<span data-ttu-id="2109e-128">Дата начала действия чата.</span><span class="sxs-lookup"><span data-stu-id="2109e-128">Date when the chat activity started.</span></span> <span data-ttu-id="2109e-129">Значение представлено в формате ISO 8601 для календарных дат.</span><span class="sxs-lookup"><span data-stu-id="2109e-129">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="2109e-130">Например, значение свойства может иметь значение "2019-07-03", которое соответствует формату ГГГГ – MM – DD.</span><span class="sxs-lookup"><span data-stu-id="2109e-130">For example, the property value could be "2019-07-03" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="2109e-131">тимезонеусед</span><span class="sxs-lookup"><span data-stu-id="2109e-131">timeZoneUsed</span></span>|<span data-ttu-id="2109e-132">String</span><span class="sxs-lookup"><span data-stu-id="2109e-132">String</span></span>|<span data-ttu-id="2109e-133">Часовой пояс, который пользователь задает в календаре Outlook для вычисления.</span><span class="sxs-lookup"><span data-stu-id="2109e-133">The time zone that the user sets in Outlook calendar is used for the computation.</span></span> <span data-ttu-id="2109e-134">Например, значение свойства может быть "тихоокеанское стандартное время".</span><span class="sxs-lookup"><span data-stu-id="2109e-134">For example, the property value could be "Pacific Standard Time."</span></span>|
|<span data-ttu-id="2109e-135">афтерхаурс</span><span class="sxs-lookup"><span data-stu-id="2109e-135">afterHours</span></span>|<span data-ttu-id="2109e-136">Длительность</span><span class="sxs-lookup"><span data-stu-id="2109e-136">Duration</span></span>|<span data-ttu-id="2109e-137">Время, затраченное на беседы в нерабочее время, которое основано на параметре календаря Microsoft Outlook пользователя для рабочих часов.</span><span class="sxs-lookup"><span data-stu-id="2109e-137">Time spent on chats outside of working hours, which is based on the user's Microsoft Outlook calendar setting for work hours.</span></span> <span data-ttu-id="2109e-138">Значение представляется в формате ISO 8601 для длительности.</span><span class="sxs-lookup"><span data-stu-id="2109e-138">The value is represented in ISO 8601 format for durations.</span></span> |

## <a name="relationships"></a><span data-ttu-id="2109e-139">Связи</span><span class="sxs-lookup"><span data-stu-id="2109e-139">Relationships</span></span>

<span data-ttu-id="2109e-140">Нет</span><span class="sxs-lookup"><span data-stu-id="2109e-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2109e-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2109e-141">JSON representation</span></span>

<span data-ttu-id="2109e-142">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2109e-142">The following is a JSON representation of the resource.</span></span>

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

