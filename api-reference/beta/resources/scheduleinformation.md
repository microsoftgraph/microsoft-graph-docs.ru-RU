---
title: Тип ресурса scheduleInformation
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
ms.openlocfilehash: 0b7bbd861a044b28cd22603fd0ccc27d20f46fba
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078137"
---
# <a name="scheduleinformation-resource-type"></a><span data-ttu-id="cd3dc-104">Тип ресурса scheduleInformation</span><span class="sxs-lookup"><span data-stu-id="cd3dc-104">scheduleInformation resource type</span></span>

 > <span data-ttu-id="cd3dc-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cd3dc-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cd3dc-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd3dc-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="cd3dc-107">Представляет доступности пользователя, ресурса или список рассылки для заданного периода времени.</span><span class="sxs-lookup"><span data-stu-id="cd3dc-107">Represents the availability of a user, distribution list, or resource for a specified time period.</span></span>

## <a name="properties"></a><span data-ttu-id="cd3dc-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="cd3dc-108">Properties</span></span>
| <span data-ttu-id="cd3dc-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="cd3dc-109">Property</span></span>     | <span data-ttu-id="cd3dc-110">Тип</span><span class="sxs-lookup"><span data-stu-id="cd3dc-110">Type</span></span>   |<span data-ttu-id="cd3dc-111">Description</span><span class="sxs-lookup"><span data-stu-id="cd3dc-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cd3dc-112">availabilityView</span><span class="sxs-lookup"><span data-stu-id="cd3dc-112">availabilityView</span></span> |<span data-ttu-id="cd3dc-113">String</span><span class="sxs-lookup"><span data-stu-id="cd3dc-113">String</span></span> |<span data-ttu-id="cd3dc-114">Представляет объединенное представление доступности всех элементов в `scheduleItems`.</span><span class="sxs-lookup"><span data-stu-id="cd3dc-114">Represents a merged view of availability of all the items in `scheduleItems`.</span></span> <span data-ttu-id="cd3dc-115">Представление состоит из слотами времени.</span><span class="sxs-lookup"><span data-stu-id="cd3dc-115">The view consists of time slots.</span></span> <span data-ttu-id="cd3dc-116">Доступность во время каждого промежуток времени, обозначается: `0`свободен, = `1`= под вопросом, `2`= «занят», `3`= нет на месте, `4`= работа в другом месте.</span><span class="sxs-lookup"><span data-stu-id="cd3dc-116">Availability during each time slot is indicated with: `0`= free, `1`= tentative, `2`= busy, `3`= out of office, `4`= working elsewhere.</span></span>|
|<span data-ttu-id="cd3dc-117">error</span><span class="sxs-lookup"><span data-stu-id="cd3dc-117">error</span></span> |[<span data-ttu-id="cd3dc-118">freeBusyError</span><span class="sxs-lookup"><span data-stu-id="cd3dc-118">freeBusyError</span></span>](freebusyerror.md) |<span data-ttu-id="cd3dc-119">Сведения об ошибке при попытке получить доступности пользователя, ресурса или список рассылки.</span><span class="sxs-lookup"><span data-stu-id="cd3dc-119">Error information from attempting to get the availability of the user, distribution list, or resource.</span></span> |
|<span data-ttu-id="cd3dc-120">scheduleId</span><span class="sxs-lookup"><span data-stu-id="cd3dc-120">scheduleId</span></span> |<span data-ttu-id="cd3dc-121">String</span><span class="sxs-lookup"><span data-stu-id="cd3dc-121">String</span></span> |<span data-ttu-id="cd3dc-122">SMTP-адрес пользователя, ресурса, идентифицирующий экземпляр **scheduleInformation**или список рассылки.</span><span class="sxs-lookup"><span data-stu-id="cd3dc-122">An SMTP address of the user, distribution list, or resource, identifying an instance of **scheduleInformation**.</span></span> |
|<span data-ttu-id="cd3dc-123">scheduleItems</span><span class="sxs-lookup"><span data-stu-id="cd3dc-123">scheduleItems</span></span> |<span data-ttu-id="cd3dc-124">[scheduleItem](scheduleitem.md) семейства сайтов</span><span class="sxs-lookup"><span data-stu-id="cd3dc-124">[scheduleItem](scheduleitem.md) collection</span></span> |<span data-ttu-id="cd3dc-125">Содержит элементы, описывающие доступности пользователя или ресурса.</span><span class="sxs-lookup"><span data-stu-id="cd3dc-125">Contains the items that describe the availability of the user or resource.</span></span> |
|<span data-ttu-id="cd3dc-126">workingHours</span><span class="sxs-lookup"><span data-stu-id="cd3dc-126">workingHours</span></span> |[<span data-ttu-id="cd3dc-127">workingHours</span><span class="sxs-lookup"><span data-stu-id="cd3dc-127">workingHours</span></span>](workinghours.md) |<span data-ttu-id="cd3dc-128">Дни недели и часы работы пользователя в определенном часовом поясе.</span><span class="sxs-lookup"><span data-stu-id="cd3dc-128">The days of the week and hours in a specific time zone that the user works.</span></span> <span data-ttu-id="cd3dc-129">Они задаются в составе пользователя [mailboxSettings](mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="cd3dc-129">These are set as part of the user's [mailboxSettings](mailboxsettings.md).</span></span>|


## <a name="json-representation"></a><span data-ttu-id="cd3dc-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cd3dc-130">JSON representation</span></span>

<span data-ttu-id="cd3dc-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cd3dc-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scheduleInformation"
}-->

```json
{
  "availabilityView": "String",
  "error": {"@odata.type": "microsoft.graph.freeBusyError"},
  "scheduleId": "String",
  "scheduleItems": [{"@odata.type": "microsoft.graph.scheduleItem"}],
  "workingHours": {"@odata.type": "microsoft.graph.workingHours"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "scheduleInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->