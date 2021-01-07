---
title: Тип ресурса expirationPattern
description: Шаблон срока действия в расписании запроса может быть включен в запрос на назначение пакета доступа и присутствует в назначении пакета доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5a6ae13816c3b59905ee66ad5d2d18f6a71270bd
ms.sourcegitcommit: 7732d20bd99a125118f7cea146c3f2416879f949
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/07/2021
ms.locfileid: "49777621"
---
# <a name="expirationpattern-resource-type"></a><span data-ttu-id="1d16e-103">Тип ресурса expirationPattern</span><span class="sxs-lookup"><span data-stu-id="1d16e-103">expirationPattern resource type</span></span>

<span data-ttu-id="1d16e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d16e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d16e-105">В [управлении правами Azure AD](entitlementmanagement-root.md)запрос на назначение пакета доступа создается пользователем, который хочет получить назначение пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="1d16e-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment request is created by a user who wants to obtain an access package assignment.</span></span> <span data-ttu-id="1d16e-106">Этот запрос может включать расписание для того, когда пользователь хочет получить назначение.</span><span class="sxs-lookup"><span data-stu-id="1d16e-106">This request can include a schedule for when the user would like to have an assignment.</span></span>  <span data-ttu-id="1d16e-107">Назначение пакета доступа, которое является результатом такого запроса, также имеет расписание.</span><span class="sxs-lookup"><span data-stu-id="1d16e-107">An access package assignment that results from such a request also has a schedule.</span></span>  <span data-ttu-id="1d16e-108">Поле окончания срока действия [requestSchedule](requestschedule.md) указывает, когда должен истечь срок действия назначения пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="1d16e-108">The expiration field of a [requestSchedule](requestschedule.md) indicates when the access package assignment should expire.</span></span>

## <a name="properties"></a><span data-ttu-id="1d16e-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="1d16e-109">Properties</span></span>

| <span data-ttu-id="1d16e-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="1d16e-110">Property</span></span>     | <span data-ttu-id="1d16e-111">Тип</span><span class="sxs-lookup"><span data-stu-id="1d16e-111">Type</span></span>        | <span data-ttu-id="1d16e-112">Описание</span><span class="sxs-lookup"><span data-stu-id="1d16e-112">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1d16e-113">endDateTime</span><span class="sxs-lookup"><span data-stu-id="1d16e-113">endDateTime</span></span>|<span data-ttu-id="1d16e-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d16e-114">DateTimeOffset</span></span>|<span data-ttu-id="1d16e-115">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="1d16e-115">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1d16e-116">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="1d16e-116">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="1d16e-117">duration</span><span class="sxs-lookup"><span data-stu-id="1d16e-117">duration</span></span>|<span data-ttu-id="1d16e-118">Длительность</span><span class="sxs-lookup"><span data-stu-id="1d16e-118">Duration</span></span>|<span data-ttu-id="1d16e-119">Желаемая продолжительность доступа запрашиваемого.</span><span class="sxs-lookup"><span data-stu-id="1d16e-119">The requestor's desired duration of access.</span></span> <span data-ttu-id="1d16e-120">Если указан в запросе, endDateTime не должен присутствовать.</span><span class="sxs-lookup"><span data-stu-id="1d16e-120">If specified in a request, endDateTime should not be present.</span></span>|
|<span data-ttu-id="1d16e-121">type</span><span class="sxs-lookup"><span data-stu-id="1d16e-121">type</span></span>|<span data-ttu-id="1d16e-122">expirationPatternType</span><span class="sxs-lookup"><span data-stu-id="1d16e-122">expirationPatternType</span></span>|<span data-ttu-id="1d16e-123">Желаемый тип шаблона истечения срока действия запросителем.</span><span class="sxs-lookup"><span data-stu-id="1d16e-123">The requestor's desired expiration pattern type.</span></span>|

### <a name="expirationpatterntype-values"></a><span data-ttu-id="1d16e-124">Значения expirationPatternType</span><span class="sxs-lookup"><span data-stu-id="1d16e-124">expirationPatternType values</span></span>

| <span data-ttu-id="1d16e-125">Элемент</span><span class="sxs-lookup"><span data-stu-id="1d16e-125">Member</span></span> | <span data-ttu-id="1d16e-126">Значение</span><span class="sxs-lookup"><span data-stu-id="1d16e-126">Value</span></span>| <span data-ttu-id="1d16e-127">Описание</span><span class="sxs-lookup"><span data-stu-id="1d16e-127">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="1d16e-128">notSpecified</span><span class="sxs-lookup"><span data-stu-id="1d16e-128">notSpecified</span></span>|<span data-ttu-id="1d16e-129">0</span><span class="sxs-lookup"><span data-stu-id="1d16e-129">0</span></span>|<span data-ttu-id="1d16e-130">Расписание окончания срока действия не задано.</span><span class="sxs-lookup"><span data-stu-id="1d16e-130">No expiration schedule was specified.</span></span>|
|<span data-ttu-id="1d16e-131">noExpiration</span><span class="sxs-lookup"><span data-stu-id="1d16e-131">noExpiration</span></span>|<span data-ttu-id="1d16e-132">1 </span><span class="sxs-lookup"><span data-stu-id="1d16e-132">1</span></span>|<span data-ttu-id="1d16e-133">Запросителем не хотелось, чтобы срок действия доступа истекал.</span><span class="sxs-lookup"><span data-stu-id="1d16e-133">The requestor did not wish the access to expire.</span></span>|
|<span data-ttu-id="1d16e-134">afterDateTime</span><span class="sxs-lookup"><span data-stu-id="1d16e-134">afterDateTime</span></span>|<span data-ttu-id="1d16e-135">2 </span><span class="sxs-lookup"><span data-stu-id="1d16e-135">2</span></span>|<span data-ttu-id="1d16e-136">Срок действия доступа истекает по истечении указанной даты и времени.</span><span class="sxs-lookup"><span data-stu-id="1d16e-136">Access will expire after a specified date and time.</span></span>|
|<span data-ttu-id="1d16e-137">afterDuration</span><span class="sxs-lookup"><span data-stu-id="1d16e-137">afterDuration</span></span>|<span data-ttu-id="1d16e-138">3 </span><span class="sxs-lookup"><span data-stu-id="1d16e-138">3</span></span>|<span data-ttu-id="1d16e-139">Срок действия доступа истекает по истечении указанного срока, относительно предоставленного доступа.</span><span class="sxs-lookup"><span data-stu-id="1d16e-139">Access will expire after a specified duration relative to access being granted.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1d16e-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1d16e-140">JSON representation</span></span>

<span data-ttu-id="1d16e-141">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1d16e-141">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.expirationPattern"
}-->

```json
{
    "endDateTime": "2020-09-10T23:06:53.307Z",
    "type": "afterDateTime"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "expirationPattern resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


