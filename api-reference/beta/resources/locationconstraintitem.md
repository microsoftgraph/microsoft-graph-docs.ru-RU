---
title: Тип ресурсов locationConstraintItem
description: Условия, заданные клиентом в отношении расположения для проведения собрания.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7063eb0a7aa437b51a2bfecb482012771297f766
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32578166"
---
# <a name="locationconstraintitem-resource-type"></a><span data-ttu-id="672b4-103">Тип ресурсов locationConstraintItem</span><span class="sxs-lookup"><span data-stu-id="672b4-103">locationConstraintItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="672b4-104">Условия, заданные клиентом в отношении расположения для проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="672b4-104">The conditions stated by a client for the location of a meeting.</span></span>

<span data-ttu-id="672b4-105">Тип, производный от [location](location.md).</span><span class="sxs-lookup"><span data-stu-id="672b4-105">Derived from [location](location.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="672b4-106">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="672b4-106">JSON representation</span></span>

<span data-ttu-id="672b4-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="672b4-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="672b4-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="672b4-108">Properties</span></span>
| <span data-ttu-id="672b4-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="672b4-109">Property</span></span>     | <span data-ttu-id="672b4-110">Тип</span><span class="sxs-lookup"><span data-stu-id="672b4-110">Type</span></span>   |<span data-ttu-id="672b4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="672b4-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="672b4-112">address</span><span class="sxs-lookup"><span data-stu-id="672b4-112">address</span></span> | [<span data-ttu-id="672b4-113">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="672b4-113">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="672b4-114">Почтовый адрес расположения.</span><span class="sxs-lookup"><span data-stu-id="672b4-114">The street address of the location.</span></span> |
| <span data-ttu-id="672b4-115">coordinates</span><span class="sxs-lookup"><span data-stu-id="672b4-115">coordinates</span></span> | [<span data-ttu-id="672b4-116">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="672b4-116">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="672b4-117">Географические координаты и высота расположения.</span><span class="sxs-lookup"><span data-stu-id="672b4-117">The geographic coordinates and elevation of the location.</span></span> |
| <span data-ttu-id="672b4-118">displayName</span><span class="sxs-lookup"><span data-stu-id="672b4-118">displayName</span></span>  | <span data-ttu-id="672b4-119">String</span><span class="sxs-lookup"><span data-stu-id="672b4-119">String</span></span> | <span data-ttu-id="672b4-120">Имя, связанное с расположением.</span><span class="sxs-lookup"><span data-stu-id="672b4-120">The name associated with the location.</span></span>                       |
| <span data-ttu-id="672b4-121">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="672b4-121">locationEmailAddress</span></span> | <span data-ttu-id="672b4-122">String</span><span class="sxs-lookup"><span data-stu-id="672b4-122">String</span></span> | <span data-ttu-id="672b4-123">Необязательный адрес электронной почты для расположения.</span><span class="sxs-lookup"><span data-stu-id="672b4-123">Optional email address of the location.</span></span> |
| <span data-ttu-id="672b4-124">locationType</span><span class="sxs-lookup"><span data-stu-id="672b4-124">locationType</span></span> | <span data-ttu-id="672b4-125">locationType</span><span class="sxs-lookup"><span data-stu-id="672b4-125">locationType</span></span> | <span data-ttu-id="672b4-126">Тип расположения.</span><span class="sxs-lookup"><span data-stu-id="672b4-126">The type of location.</span></span> <span data-ttu-id="672b4-127">Возможные значения: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span><span class="sxs-lookup"><span data-stu-id="672b4-127">Possible values are: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span></span> <span data-ttu-id="672b4-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="672b4-128">Read-only.</span></span>|
| <span data-ttu-id="672b4-129">locationUri</span><span class="sxs-lookup"><span data-stu-id="672b4-129">locationUri</span></span> | <span data-ttu-id="672b4-130">String</span><span class="sxs-lookup"><span data-stu-id="672b4-130">String</span></span> | <span data-ttu-id="672b4-131">Необязательный URI, представляющий местоположение.</span><span class="sxs-lookup"><span data-stu-id="672b4-131">Optional URI representing the location.</span></span> |
| <span data-ttu-id="672b4-132">Ресолвеаваилабилити</span><span class="sxs-lookup"><span data-stu-id="672b4-132">resolveAvailability</span></span> | <span data-ttu-id="672b4-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="672b4-133">Boolean</span></span> | <span data-ttu-id="672b4-p102">Если задано значение true и указанный ресурс занят, [findMeetingTimes](../api/user-findmeetingtimes.md) ищет свободный ресурс. Если задано значение false и указанный ресурс занят, **findMeetingTimes** возвращает ресурс с наиболее высоким приоритетом в кэше пользователя, не проверяя, свободен ли этот ресурс. Значение по умолчанию: true.</span><span class="sxs-lookup"><span data-stu-id="672b4-p102">If set to true and the specified resource is busy, [findMeetingTimes](../api/user-findmeetingtimes.md) looks for another resource that is free. If set to false and the specified resource is busy, **findMeetingTimes** returns the resource best ranked in the user's cache without checking if it's free. Default is true.</span></span> |
| <span data-ttu-id="672b4-137">uniqueId</span><span class="sxs-lookup"><span data-stu-id="672b4-137">uniqueId</span></span> | <span data-ttu-id="672b4-138">String</span><span class="sxs-lookup"><span data-stu-id="672b4-138">String</span></span> | <span data-ttu-id="672b4-139">Только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="672b4-139">For internal use only.</span></span>|
| <span data-ttu-id="672b4-140">uniqueIdType</span><span class="sxs-lookup"><span data-stu-id="672b4-140">uniqueIdType</span></span> | <span data-ttu-id="672b4-141">String</span><span class="sxs-lookup"><span data-stu-id="672b4-141">String</span></span> | <span data-ttu-id="672b4-142">Только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="672b4-142">For internal use only.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "locationConstraintItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/locationconstraintitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
