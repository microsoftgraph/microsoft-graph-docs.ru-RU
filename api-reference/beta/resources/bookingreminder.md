---
title: Тип ресурса Букингреминдер
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 0e5188a5a440134d11404c102b4641fc98cad04f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535486"
---
# <a name="bookingreminder-resource-type"></a><span data-ttu-id="daa51-104">Тип ресурса Букингреминдер</span><span class="sxs-lookup"><span data-stu-id="daa51-104">bookingReminder resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="daa51-105">Указывает, когда и кому отправлять напоминания по электронной почте.</span><span class="sxs-lookup"><span data-stu-id="daa51-105">Represents when and to whom to send an email reminder.</span></span>


## <a name="properties"></a><span data-ttu-id="daa51-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="daa51-106">Properties</span></span>
| <span data-ttu-id="daa51-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="daa51-107">Property</span></span>     | <span data-ttu-id="daa51-108">Тип</span><span class="sxs-lookup"><span data-stu-id="daa51-108">Type</span></span>   |<span data-ttu-id="daa51-109">Описание</span><span class="sxs-lookup"><span data-stu-id="daa51-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="daa51-110">message</span><span class="sxs-lookup"><span data-stu-id="daa51-110">message</span></span>|<span data-ttu-id="daa51-111">String</span><span class="sxs-lookup"><span data-stu-id="daa51-111">String</span></span>|<span data-ttu-id="daa51-112">Сообщение в памятке.</span><span class="sxs-lookup"><span data-stu-id="daa51-112">The message in the reminder.</span></span>|
|<span data-ttu-id="daa51-113">корреспондирующей</span><span class="sxs-lookup"><span data-stu-id="daa51-113">offset</span></span>|<span data-ttu-id="daa51-114">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="daa51-114">Duration</span></span>|<span data-ttu-id="daa51-115">Количество времени до начала встречи, в которое будет отправлено напоминание.</span><span class="sxs-lookup"><span data-stu-id="daa51-115">The amount of time before the start of an appointment that the reminder should be sent.</span></span> <span data-ttu-id="daa51-116">Он отмечен в формате [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="daa51-116">It's denoted in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="daa51-117">recipients</span><span class="sxs-lookup"><span data-stu-id="daa51-117">recipients</span></span>|<span data-ttu-id="daa51-118">String</span><span class="sxs-lookup"><span data-stu-id="daa51-118">String</span></span>| <span data-ttu-id="daa51-119">Лица, шауолд получать напоминание.</span><span class="sxs-lookup"><span data-stu-id="daa51-119">The persons who shouold receive the reminder.</span></span> <span data-ttu-id="daa51-120">Возможные значения: `allAttendees`, `staff`, `customer`.</span><span class="sxs-lookup"><span data-stu-id="daa51-120">Possible values are: `allAttendees`, `staff`, `customer`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="daa51-121">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="daa51-121">JSON representation</span></span>

<span data-ttu-id="daa51-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="daa51-122">The following is a JSON representation of the resource.</span></span>

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
