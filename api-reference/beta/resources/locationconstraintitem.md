---
title: Тип ресурсов locationConstraintItem
description: Условия, заданные клиентом в отношении расположения для проведения собрания.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 41b112da0ce62765432112dabbf999106b33379e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522906"
---
# <a name="locationconstraintitem-resource-type"></a><span data-ttu-id="45745-103">Тип ресурсов locationConstraintItem</span><span class="sxs-lookup"><span data-stu-id="45745-103">locationConstraintItem resource type</span></span>

<span data-ttu-id="45745-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45745-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45745-105">Условия, заданные клиентом в отношении расположения для проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="45745-105">The conditions stated by a client for the location of a meeting.</span></span>

<span data-ttu-id="45745-106">Тип, производный от [location](location.md).</span><span class="sxs-lookup"><span data-stu-id="45745-106">Derived from [location](location.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="45745-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="45745-107">JSON representation</span></span>

<span data-ttu-id="45745-108">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="45745-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="45745-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="45745-109">Properties</span></span>
| <span data-ttu-id="45745-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="45745-110">Property</span></span>     | <span data-ttu-id="45745-111">Тип</span><span class="sxs-lookup"><span data-stu-id="45745-111">Type</span></span>   |<span data-ttu-id="45745-112">Описание</span><span class="sxs-lookup"><span data-stu-id="45745-112">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="45745-113">address</span><span class="sxs-lookup"><span data-stu-id="45745-113">address</span></span> | [<span data-ttu-id="45745-114">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="45745-114">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="45745-115">Почтовый адрес расположения.</span><span class="sxs-lookup"><span data-stu-id="45745-115">The street address of the location.</span></span> |
| <span data-ttu-id="45745-116">coordinates</span><span class="sxs-lookup"><span data-stu-id="45745-116">coordinates</span></span> | [<span data-ttu-id="45745-117">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="45745-117">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="45745-118">Географические координаты и высота расположения.</span><span class="sxs-lookup"><span data-stu-id="45745-118">The geographic coordinates and elevation of the location.</span></span> |
| <span data-ttu-id="45745-119">displayName</span><span class="sxs-lookup"><span data-stu-id="45745-119">displayName</span></span>  | <span data-ttu-id="45745-120">String</span><span class="sxs-lookup"><span data-stu-id="45745-120">String</span></span> | <span data-ttu-id="45745-121">Имя, связанное с расположением.</span><span class="sxs-lookup"><span data-stu-id="45745-121">The name associated with the location.</span></span>                       |
| <span data-ttu-id="45745-122">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="45745-122">locationEmailAddress</span></span> | <span data-ttu-id="45745-123">String</span><span class="sxs-lookup"><span data-stu-id="45745-123">String</span></span> | <span data-ttu-id="45745-124">Необязательный адрес электронной почты для расположения.</span><span class="sxs-lookup"><span data-stu-id="45745-124">Optional email address of the location.</span></span> |
| <span data-ttu-id="45745-125">locationType</span><span class="sxs-lookup"><span data-stu-id="45745-125">locationType</span></span> | <span data-ttu-id="45745-126">locationType</span><span class="sxs-lookup"><span data-stu-id="45745-126">locationType</span></span> | <span data-ttu-id="45745-127">Тип расположения.</span><span class="sxs-lookup"><span data-stu-id="45745-127">The type of location.</span></span> <span data-ttu-id="45745-128">Возможные значения: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span><span class="sxs-lookup"><span data-stu-id="45745-128">Possible values are: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span></span> <span data-ttu-id="45745-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="45745-129">Read-only.</span></span>|
| <span data-ttu-id="45745-130">locationUri</span><span class="sxs-lookup"><span data-stu-id="45745-130">locationUri</span></span> | <span data-ttu-id="45745-131">String</span><span class="sxs-lookup"><span data-stu-id="45745-131">String</span></span> | <span data-ttu-id="45745-132">Необязательный URI, представляющий местоположение.</span><span class="sxs-lookup"><span data-stu-id="45745-132">Optional URI representing the location.</span></span> |
| <span data-ttu-id="45745-133">ресолвеаваилабилити</span><span class="sxs-lookup"><span data-stu-id="45745-133">resolveAvailability</span></span> | <span data-ttu-id="45745-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="45745-134">Boolean</span></span> | <span data-ttu-id="45745-p102">Если задано значение true и указанный ресурс занят, [findMeetingTimes](../api/user-findmeetingtimes.md) ищет свободный ресурс. Если задано значение false и указанный ресурс занят, **findMeetingTimes** возвращает ресурс с наиболее высоким приоритетом в кэше пользователя, не проверяя, свободен ли этот ресурс. Значение по умолчанию: true.</span><span class="sxs-lookup"><span data-stu-id="45745-p102">If set to true and the specified resource is busy, [findMeetingTimes](../api/user-findmeetingtimes.md) looks for another resource that is free. If set to false and the specified resource is busy, **findMeetingTimes** returns the resource best ranked in the user's cache without checking if it's free. Default is true.</span></span> |
| <span data-ttu-id="45745-138">uniqueId</span><span class="sxs-lookup"><span data-stu-id="45745-138">uniqueId</span></span> | <span data-ttu-id="45745-139">String</span><span class="sxs-lookup"><span data-stu-id="45745-139">String</span></span> | <span data-ttu-id="45745-140">Только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="45745-140">For internal use only.</span></span>|
| <span data-ttu-id="45745-141">uniqueIdType</span><span class="sxs-lookup"><span data-stu-id="45745-141">uniqueIdType</span></span> | <span data-ttu-id="45745-142">String</span><span class="sxs-lookup"><span data-stu-id="45745-142">String</span></span> | <span data-ttu-id="45745-143">Только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="45745-143">For internal use only.</span></span> |

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
