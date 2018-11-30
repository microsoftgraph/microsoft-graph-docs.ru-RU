---
title: Тип ресурса scheduleItem
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
ms.openlocfilehash: a7a31f47cde92549a72299b22a40b10c6f7845c6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080206"
---
# <a name="scheduleitem-resource-type"></a><span data-ttu-id="394cb-104">Тип ресурса scheduleItem</span><span class="sxs-lookup"><span data-stu-id="394cb-104">scheduleItem resource type</span></span>

 > <span data-ttu-id="394cb-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="394cb-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="394cb-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="394cb-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="394cb-107">Элемент, сведения о доступности пользователя, соответствующего Фактическое событие в календаре пользователя по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="394cb-107">An item that describes the availability of a user corresponding to an actual event on the user's default calendar.</span></span> <span data-ttu-id="394cb-108">Этот элемент применяется к ресурсам, а также.</span><span class="sxs-lookup"><span data-stu-id="394cb-108">This item applies to a resource as well.</span></span>

## <a name="properties"></a><span data-ttu-id="394cb-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="394cb-109">Properties</span></span>
| <span data-ttu-id="394cb-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="394cb-110">Property</span></span>     | <span data-ttu-id="394cb-111">Тип</span><span class="sxs-lookup"><span data-stu-id="394cb-111">Type</span></span>   |<span data-ttu-id="394cb-112">Описание</span><span class="sxs-lookup"><span data-stu-id="394cb-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="394cb-113">end</span><span class="sxs-lookup"><span data-stu-id="394cb-113">end</span></span> |[<span data-ttu-id="394cb-114">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="394cb-114">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="394cb-115">Даты, времени и часового пояса, название которого заканчивается соответствующего события.</span><span class="sxs-lookup"><span data-stu-id="394cb-115">The date, time, and time zone that the corresponding event ends.</span></span> |
|<span data-ttu-id="394cb-116">isPrivate</span><span class="sxs-lookup"><span data-stu-id="394cb-116">isPrivate</span></span> |<span data-ttu-id="394cb-117">Логический</span><span class="sxs-lookup"><span data-stu-id="394cb-117">Boolean</span></span> |<span data-ttu-id="394cb-118">Уровень конфиденциальности сообщения соответствующего события.</span><span class="sxs-lookup"><span data-stu-id="394cb-118">The sensitivity of the corresponding event.</span></span> <span data-ttu-id="394cb-119">Значение true, если событие помечено `private`, и false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="394cb-119">True if the event is marked `private`, false otherwise.</span></span> |
|<span data-ttu-id="394cb-120">location</span><span class="sxs-lookup"><span data-stu-id="394cb-120">location</span></span> |<span data-ttu-id="394cb-121">String</span><span class="sxs-lookup"><span data-stu-id="394cb-121">String</span></span> | <span data-ttu-id="394cb-122">Расположение, где удерживается или посетившие из соответствующих событий.</span><span class="sxs-lookup"><span data-stu-id="394cb-122">The location where the corresponding event is held or attended from.</span></span> <span data-ttu-id="394cb-123">Необязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="394cb-123">Optional.</span></span>|
|<span data-ttu-id="394cb-124">start</span><span class="sxs-lookup"><span data-stu-id="394cb-124">start</span></span> |[<span data-ttu-id="394cb-125">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="394cb-125">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="394cb-126">Даты, времени и часового пояса, который запускает соответствующего события.</span><span class="sxs-lookup"><span data-stu-id="394cb-126">The date, time, and time zone that the corresponding event starts.</span></span> |
|<span data-ttu-id="394cb-127">status</span><span class="sxs-lookup"><span data-stu-id="394cb-127">status</span></span> |<span data-ttu-id="394cb-128">String</span><span class="sxs-lookup"><span data-stu-id="394cb-128">String</span></span> | <span data-ttu-id="394cb-129">Состояние доступности пользователя или ресурсов во время соответствующего события.</span><span class="sxs-lookup"><span data-stu-id="394cb-129">The availability status of the user or resource during the corresponding event.</span></span> <span data-ttu-id="394cb-130">Возможные значения: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="394cb-130">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span> |
|<span data-ttu-id="394cb-131">subject</span><span class="sxs-lookup"><span data-stu-id="394cb-131">subject</span></span> |<span data-ttu-id="394cb-132">String</span><span class="sxs-lookup"><span data-stu-id="394cb-132">String</span></span> | <span data-ttu-id="394cb-133">Строка темы соответствующего события.</span><span class="sxs-lookup"><span data-stu-id="394cb-133">The corresponding event's subject line.</span></span> <span data-ttu-id="394cb-134">Необязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="394cb-134">Optional.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="394cb-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="394cb-135">JSON representation</span></span>

<span data-ttu-id="394cb-136">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="394cb-136">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "scheduleItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->