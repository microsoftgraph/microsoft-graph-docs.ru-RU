---
title: Тип ресурсов locationConstraintItem
description: Условия, заданные клиентом в отношении расположения для проведения собрания.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 404b0fd380c1161a827fe4610f744d0b9872c92b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447530"
---
# <a name="locationconstraintitem-resource-type"></a><span data-ttu-id="efb46-103">Тип ресурсов locationConstraintItem</span><span class="sxs-lookup"><span data-stu-id="efb46-103">locationConstraintItem resource type</span></span>

<span data-ttu-id="efb46-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="efb46-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="efb46-105">Условия, заданные клиентом в отношении расположения для проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="efb46-105">The conditions stated by a client for the location of a meeting.</span></span>

<span data-ttu-id="efb46-106">Тип, производный от [location](location.md).</span><span class="sxs-lookup"><span data-stu-id="efb46-106">Derived from [location](location.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="efb46-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="efb46-107">JSON representation</span></span>

<span data-ttu-id="efb46-108">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="efb46-108">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.location",
  "@odata.type": "microsoft.graph.locationConstraintItem"
}-->

```json
{
  "resolveAvailability": true,
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "displayName": "string",
  "locationEmailAddress": "string"
}

```
## <a name="properties"></a><span data-ttu-id="efb46-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="efb46-109">Properties</span></span>
| <span data-ttu-id="efb46-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="efb46-110">Property</span></span>     | <span data-ttu-id="efb46-111">Тип</span><span class="sxs-lookup"><span data-stu-id="efb46-111">Type</span></span>   |<span data-ttu-id="efb46-112">Описание</span><span class="sxs-lookup"><span data-stu-id="efb46-112">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="efb46-113">address</span><span class="sxs-lookup"><span data-stu-id="efb46-113">address</span></span> | [<span data-ttu-id="efb46-114">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="efb46-114">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="efb46-115">Почтовый адрес расположения.</span><span class="sxs-lookup"><span data-stu-id="efb46-115">The street address of the location.</span></span> |
| <span data-ttu-id="efb46-116">displayName</span><span class="sxs-lookup"><span data-stu-id="efb46-116">displayName</span></span>  | <span data-ttu-id="efb46-117">String</span><span class="sxs-lookup"><span data-stu-id="efb46-117">String</span></span> | <span data-ttu-id="efb46-118">Имя, связанное с расположением.</span><span class="sxs-lookup"><span data-stu-id="efb46-118">The name associated with the location.</span></span>                       |
| <span data-ttu-id="efb46-119">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="efb46-119">locationEmailAddress</span></span> | <span data-ttu-id="efb46-120">String</span><span class="sxs-lookup"><span data-stu-id="efb46-120">String</span></span> | <span data-ttu-id="efb46-121">Необязательный адрес электронной почты для расположения.</span><span class="sxs-lookup"><span data-stu-id="efb46-121">Optional email address of the location.</span></span> |
| <span data-ttu-id="efb46-122">ресолвеаваилабилити</span><span class="sxs-lookup"><span data-stu-id="efb46-122">resolveAvailability</span></span> | <span data-ttu-id="efb46-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="efb46-123">Boolean</span></span> | <span data-ttu-id="efb46-p101">Если задано значение true и указанный ресурс занят, [findMeetingTimes](../api/user-findmeetingtimes.md) ищет свободный ресурс. Если задано значение false и указанный ресурс занят, **findMeetingTimes** возвращает ресурс с наиболее высоким приоритетом в кэше пользователя, не проверяя, свободен ли этот ресурс. Значение по умолчанию: true.</span><span class="sxs-lookup"><span data-stu-id="efb46-p101">If set to true and the specified resource is busy, [findMeetingTimes](../api/user-findmeetingtimes.md) looks for another resource that is free. If set to false and the specified resource is busy, **findMeetingTimes** returns the resource best ranked in the user's cache without checking if it's free. Default is true.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "locationConstraintItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
