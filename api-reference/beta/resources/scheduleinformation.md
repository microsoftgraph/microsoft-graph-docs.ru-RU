---
title: Тип ресурса scheduleInformation
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: e84505ee2f30a5b7b52e9d5b589b8bb24d9a4c95
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521910"
---
# <a name="scheduleinformation-resource-type"></a><span data-ttu-id="259f8-104">Тип ресурса scheduleInformation</span><span class="sxs-lookup"><span data-stu-id="259f8-104">scheduleInformation resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="259f8-105">Представляет доступности пользователя, ресурса или список рассылки для заданного периода времени.</span><span class="sxs-lookup"><span data-stu-id="259f8-105">Represents the availability of a user, distribution list, or resource for a specified time period.</span></span>

## <a name="properties"></a><span data-ttu-id="259f8-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="259f8-106">Properties</span></span>
| <span data-ttu-id="259f8-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="259f8-107">Property</span></span>     | <span data-ttu-id="259f8-108">Тип</span><span class="sxs-lookup"><span data-stu-id="259f8-108">Type</span></span>   |<span data-ttu-id="259f8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="259f8-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="259f8-110">availabilityView</span><span class="sxs-lookup"><span data-stu-id="259f8-110">availabilityView</span></span> |<span data-ttu-id="259f8-111">String</span><span class="sxs-lookup"><span data-stu-id="259f8-111">String</span></span> |<span data-ttu-id="259f8-112">Представляет объединенное представление доступности всех элементов в `scheduleItems`.</span><span class="sxs-lookup"><span data-stu-id="259f8-112">Represents a merged view of availability of all the items in `scheduleItems`.</span></span> <span data-ttu-id="259f8-113">Представление состоит из слотами времени.</span><span class="sxs-lookup"><span data-stu-id="259f8-113">The view consists of time slots.</span></span> <span data-ttu-id="259f8-114">Доступность во время каждого промежуток времени, обозначается: `0`свободен, = `1`= под вопросом, `2`= «занят», `3`= нет на месте, `4`= работа в другом месте.</span><span class="sxs-lookup"><span data-stu-id="259f8-114">Availability during each time slot is indicated with: `0`= free, `1`= tentative, `2`= busy, `3`= out of office, `4`= working elsewhere.</span></span>|
|<span data-ttu-id="259f8-115">error</span><span class="sxs-lookup"><span data-stu-id="259f8-115">error</span></span> |[<span data-ttu-id="259f8-116">freeBusyError</span><span class="sxs-lookup"><span data-stu-id="259f8-116">freeBusyError</span></span>](freebusyerror.md) |<span data-ttu-id="259f8-117">Сведения об ошибке при попытке получить доступности пользователя, ресурса или список рассылки.</span><span class="sxs-lookup"><span data-stu-id="259f8-117">Error information from attempting to get the availability of the user, distribution list, or resource.</span></span> |
|<span data-ttu-id="259f8-118">scheduleId</span><span class="sxs-lookup"><span data-stu-id="259f8-118">scheduleId</span></span> |<span data-ttu-id="259f8-119">String</span><span class="sxs-lookup"><span data-stu-id="259f8-119">String</span></span> |<span data-ttu-id="259f8-120">SMTP-адрес пользователя, ресурса, идентифицирующий экземпляр **scheduleInformation**или список рассылки.</span><span class="sxs-lookup"><span data-stu-id="259f8-120">An SMTP address of the user, distribution list, or resource, identifying an instance of **scheduleInformation**.</span></span> |
|<span data-ttu-id="259f8-121">scheduleItems</span><span class="sxs-lookup"><span data-stu-id="259f8-121">scheduleItems</span></span> |<span data-ttu-id="259f8-122">[scheduleItem](scheduleitem.md) семейства сайтов</span><span class="sxs-lookup"><span data-stu-id="259f8-122">[scheduleItem](scheduleitem.md) collection</span></span> |<span data-ttu-id="259f8-123">Содержит элементы, описывающие доступности пользователя или ресурса.</span><span class="sxs-lookup"><span data-stu-id="259f8-123">Contains the items that describe the availability of the user or resource.</span></span> |
|<span data-ttu-id="259f8-124">workingHours</span><span class="sxs-lookup"><span data-stu-id="259f8-124">workingHours</span></span> |[<span data-ttu-id="259f8-125">workingHours</span><span class="sxs-lookup"><span data-stu-id="259f8-125">workingHours</span></span>](workinghours.md) |<span data-ttu-id="259f8-126">Дни недели и часы работы пользователя в определенном часовом поясе.</span><span class="sxs-lookup"><span data-stu-id="259f8-126">The days of the week and hours in a specific time zone that the user works.</span></span> <span data-ttu-id="259f8-127">Они задаются в составе пользователя [mailboxSettings](mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="259f8-127">These are set as part of the user's [mailboxSettings](mailboxsettings.md).</span></span>|


## <a name="json-representation"></a><span data-ttu-id="259f8-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="259f8-128">JSON representation</span></span>

<span data-ttu-id="259f8-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="259f8-129">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "scheduleInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/scheduleinformation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
