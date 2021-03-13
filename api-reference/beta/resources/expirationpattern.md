---
title: тип ресурса expirationPattern
description: Шаблон истечения срока действия в расписании запросов может быть включен в запрос на назначение пакета доступа и присутствует в назначении пакета доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 250c01172e44d8ea5f3cdea94a9ac61a89a11c1b
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761411"
---
# <a name="expirationpattern-resource-type"></a><span data-ttu-id="88b81-103">тип ресурса expirationPattern</span><span class="sxs-lookup"><span data-stu-id="88b81-103">expirationPattern resource type</span></span>

<span data-ttu-id="88b81-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88b81-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88b81-105">В [управлении правами Azure AD](entitlementmanagement-root.md)запрос на назначение пакета доступа создается пользователем, который хочет получить назначение пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="88b81-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment request is created by a user who wants to obtain an access package assignment.</span></span> <span data-ttu-id="88b81-106">Этот запрос может включать расписание, когда пользователь хотел бы получить назначение.</span><span class="sxs-lookup"><span data-stu-id="88b81-106">This request can include a schedule for when the user would like to have an assignment.</span></span>  <span data-ttu-id="88b81-107">Назначение пакета доступа, которое является результатом такого запроса, также имеет расписание.</span><span class="sxs-lookup"><span data-stu-id="88b81-107">An access package assignment that results from such a request also has a schedule.</span></span>  <span data-ttu-id="88b81-108">Поле истечения срока действия [запросаSchedule](requestschedule.md) указывает, когда должно истекть назначение пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="88b81-108">The expiration field of a [requestSchedule](requestschedule.md) indicates when the access package assignment should expire.</span></span>

## <a name="properties"></a><span data-ttu-id="88b81-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="88b81-109">Properties</span></span>

| <span data-ttu-id="88b81-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="88b81-110">Property</span></span>     | <span data-ttu-id="88b81-111">Тип</span><span class="sxs-lookup"><span data-stu-id="88b81-111">Type</span></span>        | <span data-ttu-id="88b81-112">Описание</span><span class="sxs-lookup"><span data-stu-id="88b81-112">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="88b81-113">endDateTime</span><span class="sxs-lookup"><span data-stu-id="88b81-113">endDateTime</span></span>|<span data-ttu-id="88b81-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88b81-114">DateTimeOffset</span></span>|<span data-ttu-id="88b81-115">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="88b81-115">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="88b81-116">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="88b81-116">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="88b81-117">duration</span><span class="sxs-lookup"><span data-stu-id="88b81-117">duration</span></span>|<span data-ttu-id="88b81-118">Duration</span><span class="sxs-lookup"><span data-stu-id="88b81-118">Duration</span></span>|<span data-ttu-id="88b81-119">Желаемая продолжительность доступа запрашиваемого запроса.</span><span class="sxs-lookup"><span data-stu-id="88b81-119">The requestor's desired duration of access.</span></span> <span data-ttu-id="88b81-120">Если указан в запросе, endDateTime не должен присутствовать.</span><span class="sxs-lookup"><span data-stu-id="88b81-120">If specified in a request, endDateTime should not be present.</span></span>|
|<span data-ttu-id="88b81-121">type</span><span class="sxs-lookup"><span data-stu-id="88b81-121">type</span></span>|<span data-ttu-id="88b81-122">expirationPatternType</span><span class="sxs-lookup"><span data-stu-id="88b81-122">expirationPatternType</span></span>|<span data-ttu-id="88b81-123">Желаемый тип шаблона истечения срока действия запрашиваемого запроса.</span><span class="sxs-lookup"><span data-stu-id="88b81-123">The requestor's desired expiration pattern type.</span></span>|

### <a name="expirationpatterntype-values"></a><span data-ttu-id="88b81-124">значения expirationPatternType</span><span class="sxs-lookup"><span data-stu-id="88b81-124">expirationPatternType values</span></span>

| <span data-ttu-id="88b81-125">Элемент</span><span class="sxs-lookup"><span data-stu-id="88b81-125">Member</span></span> | <span data-ttu-id="88b81-126">Значение</span><span class="sxs-lookup"><span data-stu-id="88b81-126">Value</span></span>| <span data-ttu-id="88b81-127">Описание</span><span class="sxs-lookup"><span data-stu-id="88b81-127">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="88b81-128">notSpecified</span><span class="sxs-lookup"><span data-stu-id="88b81-128">notSpecified</span></span>|<span data-ttu-id="88b81-129">0</span><span class="sxs-lookup"><span data-stu-id="88b81-129">0</span></span>|<span data-ttu-id="88b81-130">Срок действия не указан.</span><span class="sxs-lookup"><span data-stu-id="88b81-130">No expiration schedule was specified.</span></span>|
|<span data-ttu-id="88b81-131">noExpiration</span><span class="sxs-lookup"><span data-stu-id="88b81-131">noExpiration</span></span>|<span data-ttu-id="88b81-132">1</span><span class="sxs-lookup"><span data-stu-id="88b81-132">1</span></span>|<span data-ttu-id="88b81-133">Запросчик не хотел, чтобы срок действия доступа истек.</span><span class="sxs-lookup"><span data-stu-id="88b81-133">The requestor did not wish the access to expire.</span></span>|
|<span data-ttu-id="88b81-134">afterDateTime</span><span class="sxs-lookup"><span data-stu-id="88b81-134">afterDateTime</span></span>|<span data-ttu-id="88b81-135">2 </span><span class="sxs-lookup"><span data-stu-id="88b81-135">2</span></span>|<span data-ttu-id="88b81-136">Срок доступа истекает после указанной даты и времени.</span><span class="sxs-lookup"><span data-stu-id="88b81-136">Access will expire after a specified date and time.</span></span>|
|<span data-ttu-id="88b81-137">afterDuration</span><span class="sxs-lookup"><span data-stu-id="88b81-137">afterDuration</span></span>|<span data-ttu-id="88b81-138">3 </span><span class="sxs-lookup"><span data-stu-id="88b81-138">3</span></span>|<span data-ttu-id="88b81-139">Срок доступа истекает после указанной продолжительности, относительно предоставленного доступа.</span><span class="sxs-lookup"><span data-stu-id="88b81-139">Access will expire after a specified duration relative to access being granted.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="88b81-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="88b81-140">JSON representation</span></span>

<span data-ttu-id="88b81-141">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="88b81-141">The following is a JSON representation of the resource.</span></span>

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


