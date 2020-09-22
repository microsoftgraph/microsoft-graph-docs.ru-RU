---
title: Тип ресурсов locationConstraint
description: Условия, заданные клиентом в отношении расположения для проведения собрания.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: f79f6243d996193aacee66c8955ce49c8b779482
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48073592"
---
# <a name="locationconstraint-resource-type"></a><span data-ttu-id="529c1-103">Тип ресурсов locationConstraint</span><span class="sxs-lookup"><span data-stu-id="529c1-103">locationConstraint resource type</span></span>

<span data-ttu-id="529c1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="529c1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="529c1-105">Условия, заданные клиентом в отношении расположения для проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="529c1-105">The conditions stated by a client for the location of a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="529c1-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="529c1-106">JSON representation</span></span>

<span data-ttu-id="529c1-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="529c1-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.locationConstraint"
}-->

```json
{
  "isRequired": true,
  "locations": [{"@odata.type": "microsoft.graph.locationConstraintItem"}],
  "suggestLocation": true
}

```
## <a name="properties"></a><span data-ttu-id="529c1-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="529c1-108">Properties</span></span>
| <span data-ttu-id="529c1-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="529c1-109">Property</span></span>     | <span data-ttu-id="529c1-110">Тип</span><span class="sxs-lookup"><span data-stu-id="529c1-110">Type</span></span>   |<span data-ttu-id="529c1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="529c1-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="529c1-112">isRequired</span><span class="sxs-lookup"><span data-stu-id="529c1-112">isRequired</span></span>|<span data-ttu-id="529c1-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="529c1-113">Boolean</span></span>|<span data-ttu-id="529c1-p101">Клиент запрашивает у службы включение в отклик данных о расположении для проведения собрания. Если задано значение true и все ресурсы заняты, [findMeetingTimes](../api/user-findmeetingtimes.md) не вернет вариантов времени для проведения собрания. Если задано значение false и все ресурсы заняты, **findMeetingTimes** все равно будет искать варианты времени для проведения собрания, но без указания расположений.</span><span class="sxs-lookup"><span data-stu-id="529c1-p101">The client requests the service to include in the response a meeting location for the meeting. If this is true and all the resources are busy, [findMeetingTimes](../api/user-findmeetingtimes.md) will not return any meeting time suggestions. If this is false and all the resources are busy, **findMeetingTimes** would still look for meeting times without locations.</span></span> |
|<span data-ttu-id="529c1-117">locations</span><span class="sxs-lookup"><span data-stu-id="529c1-117">locations</span></span>|<span data-ttu-id="529c1-118">Коллекция [locationConstraintItem](locationconstraintitem.md)</span><span class="sxs-lookup"><span data-stu-id="529c1-118">[locationConstraintItem](locationconstraintitem.md) collection</span></span>|<span data-ttu-id="529c1-119">Ограниченные сведения об одном или нескольких расположениях, которые клиент запрашивает для собрания.</span><span class="sxs-lookup"><span data-stu-id="529c1-119">Constraint information for one or more locations that the client requests for the meeting.</span></span>|
|<span data-ttu-id="529c1-120">сугжестлокатион</span><span class="sxs-lookup"><span data-stu-id="529c1-120">suggestLocation</span></span>|<span data-ttu-id="529c1-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="529c1-121">Boolean</span></span>|<span data-ttu-id="529c1-122">Клиент запрашивает у службы один или несколько вариантов расположений для проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="529c1-122">The client requests the service to suggest one or more meeting locations.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "locationConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


