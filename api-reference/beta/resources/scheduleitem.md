---
title: Тип ресурса scheduleItem
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: ed6b7441996cdf00b33be03f70afb888cc9bb251
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511354"
---
# <a name="scheduleitem-resource-type"></a><span data-ttu-id="eacb9-104">Тип ресурса scheduleItem</span><span class="sxs-lookup"><span data-stu-id="eacb9-104">scheduleItem resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="eacb9-105">Элемент, сведения о доступности пользователя, соответствующего Фактическое событие в календаре пользователя по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="eacb9-105">An item that describes the availability of a user corresponding to an actual event on the user's default calendar.</span></span> <span data-ttu-id="eacb9-106">Этот элемент применяется к ресурсам, а также.</span><span class="sxs-lookup"><span data-stu-id="eacb9-106">This item applies to a resource as well.</span></span>

## <a name="properties"></a><span data-ttu-id="eacb9-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="eacb9-107">Properties</span></span>
| <span data-ttu-id="eacb9-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="eacb9-108">Property</span></span>     | <span data-ttu-id="eacb9-109">Тип</span><span class="sxs-lookup"><span data-stu-id="eacb9-109">Type</span></span>   |<span data-ttu-id="eacb9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="eacb9-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eacb9-111">end</span><span class="sxs-lookup"><span data-stu-id="eacb9-111">end</span></span> |[<span data-ttu-id="eacb9-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="eacb9-112">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="eacb9-113">Даты, времени и часового пояса, название которого заканчивается соответствующего события.</span><span class="sxs-lookup"><span data-stu-id="eacb9-113">The date, time, and time zone that the corresponding event ends.</span></span> |
|<span data-ttu-id="eacb9-114">IsPrivate</span><span class="sxs-lookup"><span data-stu-id="eacb9-114">isPrivate</span></span> |<span data-ttu-id="eacb9-115">Логическое</span><span class="sxs-lookup"><span data-stu-id="eacb9-115">Boolean</span></span> |<span data-ttu-id="eacb9-116">Уровень конфиденциальности сообщения соответствующего события.</span><span class="sxs-lookup"><span data-stu-id="eacb9-116">The sensitivity of the corresponding event.</span></span> <span data-ttu-id="eacb9-117">Значение true, если событие помечено `private`, и false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="eacb9-117">True if the event is marked `private`, false otherwise.</span></span> |
|<span data-ttu-id="eacb9-118">location</span><span class="sxs-lookup"><span data-stu-id="eacb9-118">location</span></span> |<span data-ttu-id="eacb9-119">String</span><span class="sxs-lookup"><span data-stu-id="eacb9-119">String</span></span> | <span data-ttu-id="eacb9-120">Расположение, где удерживается или посетившие из соответствующих событий.</span><span class="sxs-lookup"><span data-stu-id="eacb9-120">The location where the corresponding event is held or attended from.</span></span> <span data-ttu-id="eacb9-121">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="eacb9-121">Optional.</span></span>|
|<span data-ttu-id="eacb9-122">start</span><span class="sxs-lookup"><span data-stu-id="eacb9-122">start</span></span> |[<span data-ttu-id="eacb9-123">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="eacb9-123">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="eacb9-124">Даты, времени и часового пояса, который запускает соответствующего события.</span><span class="sxs-lookup"><span data-stu-id="eacb9-124">The date, time, and time zone that the corresponding event starts.</span></span> |
|<span data-ttu-id="eacb9-125">status</span><span class="sxs-lookup"><span data-stu-id="eacb9-125">status</span></span> |<span data-ttu-id="eacb9-126">String</span><span class="sxs-lookup"><span data-stu-id="eacb9-126">String</span></span> | <span data-ttu-id="eacb9-127">Состояние доступности пользователя или ресурсов во время соответствующего события.</span><span class="sxs-lookup"><span data-stu-id="eacb9-127">The availability status of the user or resource during the corresponding event.</span></span> <span data-ttu-id="eacb9-128">Возможные значения: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="eacb9-128">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span> |
|<span data-ttu-id="eacb9-129">subject</span><span class="sxs-lookup"><span data-stu-id="eacb9-129">subject</span></span> |<span data-ttu-id="eacb9-130">String</span><span class="sxs-lookup"><span data-stu-id="eacb9-130">String</span></span> | <span data-ttu-id="eacb9-131">Строка темы соответствующего события.</span><span class="sxs-lookup"><span data-stu-id="eacb9-131">The corresponding event's subject line.</span></span> <span data-ttu-id="eacb9-132">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="eacb9-132">Optional.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="eacb9-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eacb9-133">JSON representation</span></span>

<span data-ttu-id="eacb9-134">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eacb9-134">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scheduleItem"
}-->

```json
{
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "isPrivate": true,
  "location": "String",
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "status": "String",
  "subject": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "scheduleItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/scheduleitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
