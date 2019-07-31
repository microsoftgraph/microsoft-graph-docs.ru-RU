---
title: Тип ресурсов locationConstraintItem
description: Условия, заданные клиентом в отношении расположения для проведения собрания.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d7202f5ba52b1d3331c954e4c6a937d9bc36ae23
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966988"
---
# <a name="locationconstraintitem-resource-type"></a><span data-ttu-id="24fd6-103">Тип ресурсов locationConstraintItem</span><span class="sxs-lookup"><span data-stu-id="24fd6-103">locationConstraintItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24fd6-104">Условия, заданные клиентом в отношении расположения для проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="24fd6-104">The conditions stated by a client for the location of a meeting.</span></span>

<span data-ttu-id="24fd6-105">Тип, производный от [location](location.md).</span><span class="sxs-lookup"><span data-stu-id="24fd6-105">Derived from [location](location.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="24fd6-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="24fd6-106">JSON representation</span></span>

<span data-ttu-id="24fd6-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="24fd6-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  
  ],
  "@odata.type": "microsoft.graph.locationConstraintItem"
}-->

```json
{
  "resolveAvailability": true,
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "coordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "displayName": "string",
  "locationEmailAddress": "string",
  "locationType": "string",
  "locationUri": "string",
  "uniqueId": "string",
  "uniqueIdType": "string"
}

```
## <a name="properties"></a><span data-ttu-id="24fd6-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="24fd6-108">Properties</span></span>
| <span data-ttu-id="24fd6-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="24fd6-109">Property</span></span>     | <span data-ttu-id="24fd6-110">Тип</span><span class="sxs-lookup"><span data-stu-id="24fd6-110">Type</span></span>   |<span data-ttu-id="24fd6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="24fd6-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="24fd6-112">address</span><span class="sxs-lookup"><span data-stu-id="24fd6-112">address</span></span> | [<span data-ttu-id="24fd6-113">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="24fd6-113">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="24fd6-114">Почтовый адрес расположения.</span><span class="sxs-lookup"><span data-stu-id="24fd6-114">The street address of the location.</span></span> |
| <span data-ttu-id="24fd6-115">coordinates</span><span class="sxs-lookup"><span data-stu-id="24fd6-115">coordinates</span></span> | [<span data-ttu-id="24fd6-116">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="24fd6-116">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="24fd6-117">Географические координаты и высота расположения.</span><span class="sxs-lookup"><span data-stu-id="24fd6-117">The geographic coordinates and elevation of the location.</span></span> |
| <span data-ttu-id="24fd6-118">displayName</span><span class="sxs-lookup"><span data-stu-id="24fd6-118">displayName</span></span>  | <span data-ttu-id="24fd6-119">String</span><span class="sxs-lookup"><span data-stu-id="24fd6-119">String</span></span> | <span data-ttu-id="24fd6-120">Имя, связанное с расположением.</span><span class="sxs-lookup"><span data-stu-id="24fd6-120">The name associated with the location.</span></span>                       |
| <span data-ttu-id="24fd6-121">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="24fd6-121">locationEmailAddress</span></span> | <span data-ttu-id="24fd6-122">String</span><span class="sxs-lookup"><span data-stu-id="24fd6-122">String</span></span> | <span data-ttu-id="24fd6-123">Необязательный адрес электронной почты для расположения.</span><span class="sxs-lookup"><span data-stu-id="24fd6-123">Optional email address of the location.</span></span> |
| <span data-ttu-id="24fd6-124">locationType</span><span class="sxs-lookup"><span data-stu-id="24fd6-124">locationType</span></span> | <span data-ttu-id="24fd6-125">locationType</span><span class="sxs-lookup"><span data-stu-id="24fd6-125">locationType</span></span> | <span data-ttu-id="24fd6-126">Тип расположения.</span><span class="sxs-lookup"><span data-stu-id="24fd6-126">The type of location.</span></span> <span data-ttu-id="24fd6-127">Возможные значения: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span><span class="sxs-lookup"><span data-stu-id="24fd6-127">Possible values are: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span></span> <span data-ttu-id="24fd6-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="24fd6-128">Read-only.</span></span>|
| <span data-ttu-id="24fd6-129">locationUri</span><span class="sxs-lookup"><span data-stu-id="24fd6-129">locationUri</span></span> | <span data-ttu-id="24fd6-130">String</span><span class="sxs-lookup"><span data-stu-id="24fd6-130">String</span></span> | <span data-ttu-id="24fd6-131">Необязательный URI, представляющий местоположение.</span><span class="sxs-lookup"><span data-stu-id="24fd6-131">Optional URI representing the location.</span></span> |
| <span data-ttu-id="24fd6-132">Ресолвеаваилабилити</span><span class="sxs-lookup"><span data-stu-id="24fd6-132">resolveAvailability</span></span> | <span data-ttu-id="24fd6-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="24fd6-133">Boolean</span></span> | <span data-ttu-id="24fd6-p102">Если задано значение true и указанный ресурс занят, [findMeetingTimes](../api/user-findmeetingtimes.md) ищет свободный ресурс. Если задано значение false и указанный ресурс занят, **findMeetingTimes** возвращает ресурс с наиболее высоким приоритетом в кэше пользователя, не проверяя, свободен ли этот ресурс. Значение по умолчанию: true.</span><span class="sxs-lookup"><span data-stu-id="24fd6-p102">If set to true and the specified resource is busy, [findMeetingTimes](../api/user-findmeetingtimes.md) looks for another resource that is free. If set to false and the specified resource is busy, **findMeetingTimes** returns the resource best ranked in the user's cache without checking if it's free. Default is true.</span></span> |
| <span data-ttu-id="24fd6-137">uniqueId</span><span class="sxs-lookup"><span data-stu-id="24fd6-137">uniqueId</span></span> | <span data-ttu-id="24fd6-138">String</span><span class="sxs-lookup"><span data-stu-id="24fd6-138">String</span></span> | <span data-ttu-id="24fd6-139">Только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="24fd6-139">For internal use only.</span></span>|
| <span data-ttu-id="24fd6-140">uniqueIdType</span><span class="sxs-lookup"><span data-stu-id="24fd6-140">uniqueIdType</span></span> | <span data-ttu-id="24fd6-141">String</span><span class="sxs-lookup"><span data-stu-id="24fd6-141">String</span></span> | <span data-ttu-id="24fd6-142">Только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="24fd6-142">For internal use only.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "locationConstraintItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
