---
title: Тип ресурса bookingReminder
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 0e5188a5a440134d11404c102b4641fc98cad04f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526083"
---
# <a name="bookingreminder-resource-type"></a><span data-ttu-id="d7554-104">Тип ресурса bookingReminder</span><span class="sxs-lookup"><span data-stu-id="d7554-104">bookingReminder resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="d7554-105">Представляет при и к которым следует отправить по электронной почте напоминания.</span><span class="sxs-lookup"><span data-stu-id="d7554-105">Represents when and to whom to send an email reminder.</span></span>


## <a name="properties"></a><span data-ttu-id="d7554-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d7554-106">Properties</span></span>
| <span data-ttu-id="d7554-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="d7554-107">Property</span></span>     | <span data-ttu-id="d7554-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d7554-108">Type</span></span>   |<span data-ttu-id="d7554-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d7554-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d7554-110">message</span><span class="sxs-lookup"><span data-stu-id="d7554-110">message</span></span>|<span data-ttu-id="d7554-111">String</span><span class="sxs-lookup"><span data-stu-id="d7554-111">String</span></span>|<span data-ttu-id="d7554-112">Сообщение в напоминания.</span><span class="sxs-lookup"><span data-stu-id="d7554-112">The message in the reminder.</span></span>|
|<span data-ttu-id="d7554-113">Offset</span><span class="sxs-lookup"><span data-stu-id="d7554-113">offset</span></span>|<span data-ttu-id="d7554-114">Длительность</span><span class="sxs-lookup"><span data-stu-id="d7554-114">Duration</span></span>|<span data-ttu-id="d7554-115">Количество времени до начала встречи, на который будут отправляться напоминания.</span><span class="sxs-lookup"><span data-stu-id="d7554-115">The amount of time before the start of an appointment that the reminder should be sent.</span></span> <span data-ttu-id="d7554-116">Отображаются в формате [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="d7554-116">It's denoted in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="d7554-117">recipients</span><span class="sxs-lookup"><span data-stu-id="d7554-117">recipients</span></span>|<span data-ttu-id="d7554-118">String</span><span class="sxs-lookup"><span data-stu-id="d7554-118">String</span></span>| <span data-ttu-id="d7554-119">Лиц, которые shouold получать оповещение.</span><span class="sxs-lookup"><span data-stu-id="d7554-119">The persons who shouold receive the reminder.</span></span> <span data-ttu-id="d7554-120">Возможные значения: `allAttendees`, `staff`, `customer`.</span><span class="sxs-lookup"><span data-stu-id="d7554-120">Possible values are: `allAttendees`, `staff`, `customer`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d7554-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d7554-121">JSON representation</span></span>

<span data-ttu-id="d7554-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d7554-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingReminder"
}-->

```json
{
  "message": "String",
  "offset": "String (timestamp)",
  "recipients": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingReminder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingreminder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
