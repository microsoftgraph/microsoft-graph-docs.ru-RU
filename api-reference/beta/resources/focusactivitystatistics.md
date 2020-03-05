---
title: Тип ресурса Фокусактивитистатистикс
description: Представляет сведения об индивидуальных трудозатратах для пользователей
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 1c92225c0a95f49bd95b8c81abac70a0600f7cea
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42497995"
---
# <a name="focusactivitystatistics-resource-type"></a><span data-ttu-id="4b257-103">Тип ресурса Фокусактивитистатистикс</span><span class="sxs-lookup"><span data-stu-id="4b257-103">focusActivityStatistics resource type</span></span>

<span data-ttu-id="4b257-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4b257-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b257-105">Представляет данные о времени, доступном пользователю, для работы с фокусом.</span><span class="sxs-lookup"><span data-stu-id="4b257-105">Represents data about the user's time available for focus work.</span></span> <span data-ttu-id="4b257-106">Это основано на [активитистатистикс](../resources/activitystatistics.md).</span><span class="sxs-lookup"><span data-stu-id="4b257-106">This is based on [activityStatistics](../resources/activitystatistics.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4b257-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4b257-107">Properties</span></span>

| <span data-ttu-id="4b257-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b257-108">Property</span></span>     | <span data-ttu-id="4b257-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4b257-109">Type</span></span>        | <span data-ttu-id="4b257-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4b257-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4b257-111">activity</span><span class="sxs-lookup"><span data-stu-id="4b257-111">activity</span></span>|<span data-ttu-id="4b257-112">аналитиксактивититипе</span><span class="sxs-lookup"><span data-stu-id="4b257-112">analyticsActivityType</span></span>| <span data-ttu-id="4b257-113">Действие фокуса, для которого возвращается статистика.</span><span class="sxs-lookup"><span data-stu-id="4b257-113">Focus activity for which statistics are returned.</span></span>|
|<span data-ttu-id="4b257-114">duration</span><span class="sxs-lookup"><span data-stu-id="4b257-114">duration</span></span>|<span data-ttu-id="4b257-115">Длительность</span><span class="sxs-lookup"><span data-stu-id="4b257-115">Duration</span></span>|<span data-ttu-id="4b257-116">Общая сумма количества часов в фокусе, равная всем блокам времени по крайней мере в два последовательных часа, в календаре Microsoft Outlook пользователя без собрания с другими людьми в рабочем времени пользователя.</span><span class="sxs-lookup"><span data-stu-id="4b257-116">Total sum of focus hours, which is equal to all time blocks of at least two consecutive hours, in a user's Microsoft Outlook calendar without a meeting with other people within the user's set work hours.</span></span> <span data-ttu-id="4b257-117">Значение представляется в формате ISO 8601 для длительности.</span><span class="sxs-lookup"><span data-stu-id="4b257-117">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="4b257-118">endDate</span><span class="sxs-lookup"><span data-stu-id="4b257-118">endDate</span></span>|<span data-ttu-id="4b257-119">Date</span><span class="sxs-lookup"><span data-stu-id="4b257-119">Date</span></span>|<span data-ttu-id="4b257-120">Дата окончания действия фокуса.</span><span class="sxs-lookup"><span data-stu-id="4b257-120">Date when the focus activity ended.</span></span> <span data-ttu-id="4b257-121">Значение представлено в формате ISO 8601 для календарных дат.</span><span class="sxs-lookup"><span data-stu-id="4b257-121">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="4b257-122">Например, значение свойства может иметь значение "2019-07-04", которое соответствует формату ГГГГ – MM – DD.</span><span class="sxs-lookup"><span data-stu-id="4b257-122">For example, the property value could be "2019-07-04" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="4b257-123">id</span><span class="sxs-lookup"><span data-stu-id="4b257-123">id</span></span>|<span data-ttu-id="4b257-124">String</span><span class="sxs-lookup"><span data-stu-id="4b257-124">String</span></span>| <span data-ttu-id="4b257-125">Идентификатор, предназначенный только для чтения, для действия Focus.</span><span class="sxs-lookup"><span data-stu-id="4b257-125">Read-only ID for the focus activity.</span></span>|
|<span data-ttu-id="4b257-126">startDate</span><span class="sxs-lookup"><span data-stu-id="4b257-126">startDate</span></span>|<span data-ttu-id="4b257-127">Дата</span><span class="sxs-lookup"><span data-stu-id="4b257-127">Date</span></span>|<span data-ttu-id="4b257-128">Дата начала действия фокуса.</span><span class="sxs-lookup"><span data-stu-id="4b257-128">Date when the focus activity started.</span></span> <span data-ttu-id="4b257-129">Значение представлено в формате ISO 8601 для календарных дат.</span><span class="sxs-lookup"><span data-stu-id="4b257-129">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="4b257-130">Например, значение свойства может иметь значение "2019-07-03", которое соответствует формату ГГГГ – MM – DD.</span><span class="sxs-lookup"><span data-stu-id="4b257-130">For example, the property value could be "2019-07-03" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="4b257-131">тимезонеусед</span><span class="sxs-lookup"><span data-stu-id="4b257-131">timeZoneUsed</span></span>|<span data-ttu-id="4b257-132">String</span><span class="sxs-lookup"><span data-stu-id="4b257-132">String</span></span>|<span data-ttu-id="4b257-133">Часовой пояс, который пользователь задает в календаре Outlook для вычисления.</span><span class="sxs-lookup"><span data-stu-id="4b257-133">The time zone that the user sets in Outlook calendar is used for the computation.</span></span> <span data-ttu-id="4b257-134">Например, значение свойства может быть "тихоокеанское стандартное время".</span><span class="sxs-lookup"><span data-stu-id="4b257-134">For example, the property value could be "Pacific Standard Time."</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b257-135">Связи</span><span class="sxs-lookup"><span data-stu-id="4b257-135">Relationships</span></span>

<span data-ttu-id="4b257-136">Нет</span><span class="sxs-lookup"><span data-stu-id="4b257-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4b257-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4b257-137">JSON representation</span></span>

<span data-ttu-id="4b257-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4b257-138">The following is a JSON representation of the resource.</span></span>

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