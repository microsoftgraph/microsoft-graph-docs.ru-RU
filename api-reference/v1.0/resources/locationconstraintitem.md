---
title: Тип ресурсов locationConstraintItem
description: Условия, заданные клиентом в отношении расположения для проведения собрания.
localization_priority: Normal
ms.openlocfilehash: d9124377172c7598d45b0be9b9f3f9799bd3e1f5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32525525"
---
# <a name="locationconstraintitem-resource-type"></a><span data-ttu-id="7005a-103">Тип ресурсов locationConstraintItem</span><span class="sxs-lookup"><span data-stu-id="7005a-103">locationConstraintItem resource type</span></span>

<span data-ttu-id="7005a-104">Условия, заданные клиентом в отношении расположения для проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="7005a-104">The conditions stated by a client for the location of a meeting.</span></span>

<span data-ttu-id="7005a-105">Тип, производный от [location](location.md).</span><span class="sxs-lookup"><span data-stu-id="7005a-105">Derived from [location](location.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="7005a-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7005a-106">JSON representation</span></span>

<span data-ttu-id="7005a-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="7005a-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="7005a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="7005a-108">Properties</span></span>
| <span data-ttu-id="7005a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="7005a-109">Property</span></span>     | <span data-ttu-id="7005a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="7005a-110">Type</span></span>   |<span data-ttu-id="7005a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7005a-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7005a-112">address</span><span class="sxs-lookup"><span data-stu-id="7005a-112">address</span></span> | [<span data-ttu-id="7005a-113">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="7005a-113">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="7005a-114">Почтовый адрес расположения.</span><span class="sxs-lookup"><span data-stu-id="7005a-114">The street address of the location.</span></span> |
| <span data-ttu-id="7005a-115">displayName</span><span class="sxs-lookup"><span data-stu-id="7005a-115">displayName</span></span>  | <span data-ttu-id="7005a-116">String</span><span class="sxs-lookup"><span data-stu-id="7005a-116">String</span></span> | <span data-ttu-id="7005a-117">Имя, связанное с расположением.</span><span class="sxs-lookup"><span data-stu-id="7005a-117">The name associated with the location.</span></span>                       |
| <span data-ttu-id="7005a-118">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="7005a-118">locationEmailAddress</span></span> | <span data-ttu-id="7005a-119">String</span><span class="sxs-lookup"><span data-stu-id="7005a-119">String</span></span> | <span data-ttu-id="7005a-120">Необязательный адрес электронной почты для расположения.</span><span class="sxs-lookup"><span data-stu-id="7005a-120">Optional email address of the location.</span></span> |
| <span data-ttu-id="7005a-121">Ресолвеаваилабилити</span><span class="sxs-lookup"><span data-stu-id="7005a-121">resolveAvailability</span></span> | <span data-ttu-id="7005a-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="7005a-122">Boolean</span></span> | <span data-ttu-id="7005a-p101">Если задано значение true и указанный ресурс занят, [findMeetingTimes](../api/user-findmeetingtimes.md) ищет свободный ресурс. Если задано значение false и указанный ресурс занят, **findMeetingTimes** возвращает ресурс с наиболее высоким приоритетом в кэше пользователя, не проверяя, свободен ли этот ресурс. Значение по умолчанию: true.</span><span class="sxs-lookup"><span data-stu-id="7005a-p101">If set to true and the specified resource is busy, [findMeetingTimes](../api/user-findmeetingtimes.md) looks for another resource that is free. If set to false and the specified resource is busy, **findMeetingTimes** returns the resource best ranked in the user's cache without checking if it's free. Default is true.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "locationConstraintItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
