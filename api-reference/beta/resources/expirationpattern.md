---
title: Тип ресурса Експиратионпаттерн
description: Шаблон истечения срока действия в расписании запросов можно включить в запрос на назначение пакета Access и он присутствует в назначении пакета Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 62c49b7e725b923b95c514a7d3e955fed5fce46c
ms.sourcegitcommit: 01f73b4dce6f885da18d62fe800b387c286c7a8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/09/2020
ms.locfileid: "47413398"
---
# <a name="expirationpattern-resource-type"></a><span data-ttu-id="7384a-103">Тип ресурса Експиратионпаттерн</span><span class="sxs-lookup"><span data-stu-id="7384a-103">expirationPattern resource type</span></span>

<span data-ttu-id="7384a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7384a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7384a-105">В [управлении обслуживанием в Azure AD](entitlementmanagement-root.md)запрос на назначение пакета Access создается пользователем, желающим получить назначение пакета Access.</span><span class="sxs-lookup"><span data-stu-id="7384a-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment request is created by a user who wants to obtain an access package assignment.</span></span> <span data-ttu-id="7384a-106">Этот запрос может включать расписание, когда пользователь хочет назначить назначение.</span><span class="sxs-lookup"><span data-stu-id="7384a-106">This request can include a schedule for when the user would like to have an assignment.</span></span>  <span data-ttu-id="7384a-107">Назначение пакета Access, полученное в результате такого запроса, также имеет расписание.</span><span class="sxs-lookup"><span data-stu-id="7384a-107">An access package assignment that results from such a request also has a schedule.</span></span>  <span data-ttu-id="7384a-108">Поле истечения срока действия [рекуестсчедуле](requestschedule.md) указывает, когда истечет срок действия назначения пакета Access.</span><span class="sxs-lookup"><span data-stu-id="7384a-108">The expiration field of a [requestSchedule](requestschedule.md) indicates when the access package assignment should expire.</span></span>

## <a name="properties"></a><span data-ttu-id="7384a-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="7384a-109">Properties</span></span>

| <span data-ttu-id="7384a-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="7384a-110">Property</span></span>     | <span data-ttu-id="7384a-111">Тип</span><span class="sxs-lookup"><span data-stu-id="7384a-111">Type</span></span>        | <span data-ttu-id="7384a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="7384a-112">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7384a-113">endDateTime</span><span class="sxs-lookup"><span data-stu-id="7384a-113">endDateTime</span></span>|<span data-ttu-id="7384a-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7384a-114">DateTimeOffset</span></span>|<span data-ttu-id="7384a-115">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="7384a-115">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7384a-116">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="7384a-116">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="7384a-117">duration</span><span class="sxs-lookup"><span data-stu-id="7384a-117">duration</span></span>|<span data-ttu-id="7384a-118">Длительность</span><span class="sxs-lookup"><span data-stu-id="7384a-118">Duration</span></span>|<span data-ttu-id="7384a-119">Предполагаемая длительность доступа запрашивающего.</span><span class="sxs-lookup"><span data-stu-id="7384a-119">The requestor's desired duration of access.</span></span> <span data-ttu-id="7384a-120">Если это указано в запросе, endDateTime не должно присутствовать.</span><span class="sxs-lookup"><span data-stu-id="7384a-120">If specified in a request, endDateTime should not be present.</span></span>|
|<span data-ttu-id="7384a-121">type</span><span class="sxs-lookup"><span data-stu-id="7384a-121">type</span></span>|<span data-ttu-id="7384a-122">експиратионпаттернтипе</span><span class="sxs-lookup"><span data-stu-id="7384a-122">expirationPatternType</span></span>|<span data-ttu-id="7384a-123">Нужный тип шаблона срока действия запрашивающего.</span><span class="sxs-lookup"><span data-stu-id="7384a-123">The requestor's desired expiration pattern type.</span></span>|

### <a name="expirationpatterntype-values"></a><span data-ttu-id="7384a-124">значения Експиратионпаттернтипе</span><span class="sxs-lookup"><span data-stu-id="7384a-124">expirationPatternType values</span></span>

| <span data-ttu-id="7384a-125">Элемент</span><span class="sxs-lookup"><span data-stu-id="7384a-125">Member</span></span> | <span data-ttu-id="7384a-126">Значение</span><span class="sxs-lookup"><span data-stu-id="7384a-126">Value</span></span>| <span data-ttu-id="7384a-127">Описание</span><span class="sxs-lookup"><span data-stu-id="7384a-127">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="7384a-128">нотспеЦифиед</span><span class="sxs-lookup"><span data-stu-id="7384a-128">notSpecified</span></span>|<span data-ttu-id="7384a-129">нуль</span><span class="sxs-lookup"><span data-stu-id="7384a-129">0</span></span>|<span data-ttu-id="7384a-130">Расписание истечения срока действия не указано.</span><span class="sxs-lookup"><span data-stu-id="7384a-130">No expiration schedule was specified.</span></span>|
|<span data-ttu-id="7384a-131">неограниченный срок действия</span><span class="sxs-lookup"><span data-stu-id="7384a-131">noExpiration</span></span>|<span data-ttu-id="7384a-132">1,1</span><span class="sxs-lookup"><span data-stu-id="7384a-132">1</span></span>|<span data-ttu-id="7384a-133">Запрашивающая сторона не предоставила срок действия доступа.</span><span class="sxs-lookup"><span data-stu-id="7384a-133">The requestor did not wish the access to expire.</span></span>|
|<span data-ttu-id="7384a-134">афтердатетиме</span><span class="sxs-lookup"><span data-stu-id="7384a-134">afterDateTime</span></span>|<span data-ttu-id="7384a-135">2</span><span class="sxs-lookup"><span data-stu-id="7384a-135">2</span></span>|<span data-ttu-id="7384a-136">Срок действия доступа через указанную дату и время истечет.</span><span class="sxs-lookup"><span data-stu-id="7384a-136">Access will expire after a specified date and time.</span></span>|
|<span data-ttu-id="7384a-137">афтердуратион</span><span class="sxs-lookup"><span data-stu-id="7384a-137">afterDuration</span></span>|<span data-ttu-id="7384a-138">4</span><span class="sxs-lookup"><span data-stu-id="7384a-138">3</span></span>|<span data-ttu-id="7384a-139">Срок действия доступа истекает через указанное время относительно предоставления доступа.</span><span class="sxs-lookup"><span data-stu-id="7384a-139">Access will expire after a specified duration relative to access being granted.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7384a-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7384a-140">JSON representation</span></span>

<span data-ttu-id="7384a-141">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7384a-141">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.expirationPattern",
  "baseType": ""
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
