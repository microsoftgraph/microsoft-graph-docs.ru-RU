---
title: Тип ресурсов locationConstraint
description: Условия, заданные клиентом в отношении расположения для проведения собрания.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: d22e351217125cc54f2fa7f95e4be1d3d70fc6a2
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345314"
---
# <a name="locationconstraint-resource-type"></a><span data-ttu-id="f3458-103">Тип ресурсов locationConstraint</span><span class="sxs-lookup"><span data-stu-id="f3458-103">locationConstraint resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3458-104">Условия, заданные клиентом в отношении расположения для проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="f3458-104">The conditions stated by a client for the location of a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3458-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f3458-105">JSON representation</span></span>

<span data-ttu-id="f3458-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="f3458-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="f3458-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f3458-107">Properties</span></span>
| <span data-ttu-id="f3458-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f3458-108">Property</span></span>     | <span data-ttu-id="f3458-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f3458-109">Type</span></span>   |<span data-ttu-id="f3458-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f3458-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f3458-111">isRequired</span><span class="sxs-lookup"><span data-stu-id="f3458-111">isRequired</span></span>|<span data-ttu-id="f3458-112">Логический</span><span class="sxs-lookup"><span data-stu-id="f3458-112">Boolean</span></span>|<span data-ttu-id="f3458-p101">Клиент запрашивает у службы включение в отклик данных о расположении для проведения собрания. Если задано значение true и все ресурсы заняты, [findMeetingTimes](../api/user-findmeetingtimes.md) не вернет вариантов времени для проведения собрания. Если задано значение false и все ресурсы заняты, **findMeetingTimes** все равно будет искать варианты времени для проведения собрания, но без указания расположений.</span><span class="sxs-lookup"><span data-stu-id="f3458-p101">The client requests the service to include in the response a meeting location for the meeting. If this is true and all the resources are busy, [findMeetingTimes](../api/user-findmeetingtimes.md) will not return any meeting time suggestions. If this is false and all the resources are busy, **findMeetingTimes** would still look for meeting times without locations.</span></span> |
|<span data-ttu-id="f3458-116">locations</span><span class="sxs-lookup"><span data-stu-id="f3458-116">locations</span></span>|<span data-ttu-id="f3458-117">Коллекция [locationConstraintItem](locationconstraintitem.md)</span><span class="sxs-lookup"><span data-stu-id="f3458-117">[locationConstraintItem](locationconstraintitem.md) collection</span></span>|<span data-ttu-id="f3458-118">Ограниченные сведения об одном или нескольких расположениях, которые клиент запрашивает для собрания.</span><span class="sxs-lookup"><span data-stu-id="f3458-118">Constraint information for one or more locations that the client requests for the meeting.</span></span>|
|<span data-ttu-id="f3458-119">Сугжестлокатион</span><span class="sxs-lookup"><span data-stu-id="f3458-119">suggestLocation</span></span>|<span data-ttu-id="f3458-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3458-120">Boolean</span></span>|<span data-ttu-id="f3458-121">Клиент запрашивает у службы один или несколько вариантов расположений для проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="f3458-121">The client requests the service to suggest one or more meeting locations.</span></span>|

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
