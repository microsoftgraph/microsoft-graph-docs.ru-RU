---
title: Тип ресурсов locationConstraint
description: Условия, заданные клиентом в отношении расположения для проведения собрания.
ms.openlocfilehash: d151ea97aa65aabdb759be4cb90b577606c648a5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076516"
---
# <a name="locationconstraint-resource-type"></a><span data-ttu-id="e630c-103">Тип ресурсов locationConstraint</span><span class="sxs-lookup"><span data-stu-id="e630c-103">locationConstraint resource type</span></span>

> <span data-ttu-id="e630c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e630c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e630c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e630c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e630c-106">Условия, заданные клиентом в отношении расположения для проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="e630c-106">The conditions stated by a client for the location of a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e630c-107">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e630c-107">JSON representation</span></span>

<span data-ttu-id="e630c-108">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="e630c-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.locationconstraint"
}-->

```json
{
  "isRequired": true,
  "locations": [{"@odata.type": "microsoft.graph.locationConstraintItem"}],
  "suggestLocation": true
}

```
## <a name="properties"></a><span data-ttu-id="e630c-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="e630c-109">Properties</span></span>
| <span data-ttu-id="e630c-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="e630c-110">Property</span></span>     | <span data-ttu-id="e630c-111">Тип</span><span class="sxs-lookup"><span data-stu-id="e630c-111">Type</span></span>   |<span data-ttu-id="e630c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="e630c-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e630c-113">isRequired</span><span class="sxs-lookup"><span data-stu-id="e630c-113">isRequired</span></span>|<span data-ttu-id="e630c-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="e630c-114">Boolean</span></span>|<span data-ttu-id="e630c-p102">Клиент запрашивает у службы включение в отклик данных о расположении для проведения собрания. Если задано значение true и все ресурсы заняты, [findMeetingTimes](../api/user-findmeetingtimes.md) не вернет вариантов времени для проведения собрания. Если задано значение false и все ресурсы заняты, **findMeetingTimes** все равно будет искать варианты времени для проведения собрания, но без указания расположений.</span><span class="sxs-lookup"><span data-stu-id="e630c-p102">The client requests the service to include in the response a meeting location for the meeting. If this is true and all the resources are busy, [findMeetingTimes](../api/user-findmeetingtimes.md) will not return any meeting time suggestions. If this is false and all the resources are busy, **findMeetingTimes** would still look for meeting times without locations.</span></span> |
|<span data-ttu-id="e630c-118">locations</span><span class="sxs-lookup"><span data-stu-id="e630c-118">locations</span></span>|<span data-ttu-id="e630c-119">Коллекция [locationConstraintItem](locationconstraintitem.md)</span><span class="sxs-lookup"><span data-stu-id="e630c-119">[locationConstraintItem](locationconstraintitem.md) collection</span></span>|<span data-ttu-id="e630c-120">Ограниченные сведения об одном или нескольких расположениях, которые клиент запрашивает для собрания.</span><span class="sxs-lookup"><span data-stu-id="e630c-120">Constraint information for one or more locations that the client requests for the meeting.</span></span>|
|<span data-ttu-id="e630c-121">suggestLocation</span><span class="sxs-lookup"><span data-stu-id="e630c-121">suggestLocation</span></span>|<span data-ttu-id="e630c-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="e630c-122">Boolean</span></span>|<span data-ttu-id="e630c-123">Клиент запрашивает у службы один или несколько вариантов расположений для проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="e630c-123">The client requests the service to suggest one or more meeting locations.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "locationConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->