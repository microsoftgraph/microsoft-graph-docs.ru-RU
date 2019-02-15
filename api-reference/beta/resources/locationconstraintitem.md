---
title: Тип ресурсов locationConstraintItem
description: Условия, заданные клиентом в отношении расположения для проведения собрания.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 8e0b14096d8be66a6aab6d4e73cf0941d7db7b5c
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057003"
---
# <a name="locationconstraintitem-resource-type"></a><span data-ttu-id="b214d-103">Тип ресурсов locationConstraintItem</span><span class="sxs-lookup"><span data-stu-id="b214d-103">locationConstraintItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b214d-104">Условия, заданные клиентом в отношении расположения для проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="b214d-104">The conditions stated by a client for the location of a meeting.</span></span>

<span data-ttu-id="b214d-105">Производный от [локатиондатамодел](locationdatamodel.md).</span><span class="sxs-lookup"><span data-stu-id="b214d-105">Derived from [locationDataModel](locationdatamodel.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="b214d-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b214d-106">JSON representation</span></span>

<span data-ttu-id="b214d-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="b214d-107">Here is a JSON representation of the resource</span></span>

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
  "locationUri": "string"
}

```
## <a name="properties"></a><span data-ttu-id="b214d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b214d-108">Properties</span></span>
| <span data-ttu-id="b214d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b214d-109">Property</span></span>     | <span data-ttu-id="b214d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b214d-110">Type</span></span>   |<span data-ttu-id="b214d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b214d-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b214d-112">address</span><span class="sxs-lookup"><span data-stu-id="b214d-112">address</span></span> | [<span data-ttu-id="b214d-113">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="b214d-113">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="b214d-114">Почтовый адрес расположения.</span><span class="sxs-lookup"><span data-stu-id="b214d-114">The street address of the location.</span></span> |
| <span data-ttu-id="b214d-115">coordinates</span><span class="sxs-lookup"><span data-stu-id="b214d-115">coordinates</span></span> | [<span data-ttu-id="b214d-116">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="b214d-116">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="b214d-117">Географические координаты и высота расположения.</span><span class="sxs-lookup"><span data-stu-id="b214d-117">The geographic coordinates and elevation of the location.</span></span> |
| <span data-ttu-id="b214d-118">displayName</span><span class="sxs-lookup"><span data-stu-id="b214d-118">displayName</span></span>  | <span data-ttu-id="b214d-119">String</span><span class="sxs-lookup"><span data-stu-id="b214d-119">String</span></span> | <span data-ttu-id="b214d-120">Имя, связанное с расположением.</span><span class="sxs-lookup"><span data-stu-id="b214d-120">The name associated with the location.</span></span>                       |
| <span data-ttu-id="b214d-121">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="b214d-121">locationEmailAddress</span></span> | <span data-ttu-id="b214d-122">String</span><span class="sxs-lookup"><span data-stu-id="b214d-122">String</span></span> | <span data-ttu-id="b214d-123">Необязательный электронный адрес для расположения.</span><span class="sxs-lookup"><span data-stu-id="b214d-123">Optional email address of the location.</span></span> |
| <span data-ttu-id="b214d-124">locationUri</span><span class="sxs-lookup"><span data-stu-id="b214d-124">locationUri</span></span> | <span data-ttu-id="b214d-125">String</span><span class="sxs-lookup"><span data-stu-id="b214d-125">String</span></span> | <span data-ttu-id="b214d-126">Необязательный URI, представляющий местоположение.</span><span class="sxs-lookup"><span data-stu-id="b214d-126">Optional URI representing the location.</span></span> |
| <span data-ttu-id="b214d-127">resolveAvailability</span><span class="sxs-lookup"><span data-stu-id="b214d-127">resolveAvailability</span></span> | <span data-ttu-id="b214d-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="b214d-128">Boolean</span></span> | <span data-ttu-id="b214d-p101">Если задано значение true и указанный ресурс занят, [findMeetingTimes](../api/user-findmeetingtimes.md) ищет свободный ресурс. Если задано значение false и указанный ресурс занят, **findMeetingTimes** возвращает ресурс с наиболее высоким приоритетом в кэше пользователя, не проверяя, свободен ли этот ресурс. Значение по умолчанию: true.</span><span class="sxs-lookup"><span data-stu-id="b214d-p101">If set to true and the specified resource is busy, [findMeetingTimes](../api/user-findmeetingtimes.md) looks for another resource that is free. If set to false and the specified resource is busy, **findMeetingTimes** returns the resource best ranked in the user's cache without checking if it's free. Default is true.</span></span> |

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
