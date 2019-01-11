---
title: Тип ресурсов locationConstraintItem
description: Условия, заданные клиентом в отношении расположения для проведения собрания.
localization_priority: Normal
ms.openlocfilehash: 4c44a97a3ed0d5bcf56204fab1527c7e4b58455d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874084"
---
# <a name="locationconstraintitem-resource-type"></a><span data-ttu-id="bc7fd-103">Тип ресурсов locationConstraintItem</span><span class="sxs-lookup"><span data-stu-id="bc7fd-103">locationConstraintItem resource type</span></span>

> <span data-ttu-id="bc7fd-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bc7fd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bc7fd-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc7fd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bc7fd-106">Условия, заданные клиентом в отношении расположения для проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="bc7fd-106">The conditions stated by a client for the location of a meeting.</span></span>

<span data-ttu-id="bc7fd-107">Тип, производный от [location](location.md).</span><span class="sxs-lookup"><span data-stu-id="bc7fd-107">Derived from [location](location.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="bc7fd-108">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bc7fd-108">JSON representation</span></span>

<span data-ttu-id="bc7fd-109">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="bc7fd-109">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="bc7fd-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="bc7fd-110">Properties</span></span>
| <span data-ttu-id="bc7fd-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="bc7fd-111">Property</span></span>     | <span data-ttu-id="bc7fd-112">Тип</span><span class="sxs-lookup"><span data-stu-id="bc7fd-112">Type</span></span>   |<span data-ttu-id="bc7fd-113">Описание</span><span class="sxs-lookup"><span data-stu-id="bc7fd-113">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bc7fd-114">address</span><span class="sxs-lookup"><span data-stu-id="bc7fd-114">address</span></span> | [<span data-ttu-id="bc7fd-115">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="bc7fd-115">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="bc7fd-116">Почтовый адрес расположения.</span><span class="sxs-lookup"><span data-stu-id="bc7fd-116">The street address of the location.</span></span> |
| <span data-ttu-id="bc7fd-117">coordinates</span><span class="sxs-lookup"><span data-stu-id="bc7fd-117">coordinates</span></span> | [<span data-ttu-id="bc7fd-118">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="bc7fd-118">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="bc7fd-119">Географические координаты и высота расположения.</span><span class="sxs-lookup"><span data-stu-id="bc7fd-119">The geographic coordinates and elevation of the location.</span></span> |
| <span data-ttu-id="bc7fd-120">displayName</span><span class="sxs-lookup"><span data-stu-id="bc7fd-120">displayName</span></span>  | <span data-ttu-id="bc7fd-121">String</span><span class="sxs-lookup"><span data-stu-id="bc7fd-121">String</span></span> | <span data-ttu-id="bc7fd-122">Имя, связанное с расположением.</span><span class="sxs-lookup"><span data-stu-id="bc7fd-122">The name associated with the location.</span></span>                       |
| <span data-ttu-id="bc7fd-123">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="bc7fd-123">locationEmailAddress</span></span> | <span data-ttu-id="bc7fd-124">String</span><span class="sxs-lookup"><span data-stu-id="bc7fd-124">String</span></span> | <span data-ttu-id="bc7fd-125">Необязательный электронный адрес для расположения.</span><span class="sxs-lookup"><span data-stu-id="bc7fd-125">Optional email address of the location.</span></span> |
| <span data-ttu-id="bc7fd-126">locationUri</span><span class="sxs-lookup"><span data-stu-id="bc7fd-126">locationUri</span></span> | <span data-ttu-id="bc7fd-127">Строка</span><span class="sxs-lookup"><span data-stu-id="bc7fd-127">String</span></span> | <span data-ttu-id="bc7fd-128">Необязательный URI, представляющий местоположение.</span><span class="sxs-lookup"><span data-stu-id="bc7fd-128">Optional URI representing the location.</span></span> |
| <span data-ttu-id="bc7fd-129">resolveAvailability</span><span class="sxs-lookup"><span data-stu-id="bc7fd-129">resolveAvailability</span></span> | <span data-ttu-id="bc7fd-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc7fd-130">Boolean</span></span> | <span data-ttu-id="bc7fd-p102">Если задано значение true и указанный ресурс занят, [findMeetingTimes](../api/user-findmeetingtimes.md) ищет свободный ресурс. Если задано значение false и указанный ресурс занят, **findMeetingTimes** возвращает ресурс с наиболее высоким приоритетом в кэше пользователя, не проверяя, свободен ли этот ресурс. Значение по умолчанию: true.</span><span class="sxs-lookup"><span data-stu-id="bc7fd-p102">If set to true and the specified resource is busy, [findMeetingTimes](../api/user-findmeetingtimes.md) looks for another resource that is free. If set to false and the specified resource is busy, **findMeetingTimes** returns the resource best ranked in the user's cache without checking if it's free. Default is true.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "locationConstraintItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
