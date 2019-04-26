---
title: Тип ресурса Букингреминдер
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 18265a9d9e86b79706b6a268df3b8512b7b65111
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328208"
---
# <a name="bookingreminder-resource-type"></a><span data-ttu-id="d8d76-104">Тип ресурса Букингреминдер</span><span class="sxs-lookup"><span data-stu-id="d8d76-104">bookingReminder resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="d8d76-105">Указывает, когда и кому отправлять напоминания по электронной почте.</span><span class="sxs-lookup"><span data-stu-id="d8d76-105">Represents when and to whom to send an email reminder.</span></span>


## <a name="properties"></a><span data-ttu-id="d8d76-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d8d76-106">Properties</span></span>
| <span data-ttu-id="d8d76-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="d8d76-107">Property</span></span>     | <span data-ttu-id="d8d76-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d8d76-108">Type</span></span>   |<span data-ttu-id="d8d76-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d8d76-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d8d76-110">message</span><span class="sxs-lookup"><span data-stu-id="d8d76-110">message</span></span>|<span data-ttu-id="d8d76-111">String</span><span class="sxs-lookup"><span data-stu-id="d8d76-111">String</span></span>|<span data-ttu-id="d8d76-112">Сообщение в памятке.</span><span class="sxs-lookup"><span data-stu-id="d8d76-112">The message in the reminder.</span></span>|
|<span data-ttu-id="d8d76-113">корреспондирующей</span><span class="sxs-lookup"><span data-stu-id="d8d76-113">offset</span></span>|<span data-ttu-id="d8d76-114">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="d8d76-114">Duration</span></span>|<span data-ttu-id="d8d76-115">Количество времени до начала встречи, в которое будет отправлено напоминание.</span><span class="sxs-lookup"><span data-stu-id="d8d76-115">The amount of time before the start of an appointment that the reminder should be sent.</span></span> <span data-ttu-id="d8d76-116">Он отмечен в формате [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="d8d76-116">It's denoted in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="d8d76-117">recipients</span><span class="sxs-lookup"><span data-stu-id="d8d76-117">recipients</span></span>|<span data-ttu-id="d8d76-118">String</span><span class="sxs-lookup"><span data-stu-id="d8d76-118">String</span></span>| <span data-ttu-id="d8d76-119">Лица, шауолд получать напоминание.</span><span class="sxs-lookup"><span data-stu-id="d8d76-119">The persons who shouold receive the reminder.</span></span> <span data-ttu-id="d8d76-120">Возможные значения: `allAttendees`, `staff`, `customer`.</span><span class="sxs-lookup"><span data-stu-id="d8d76-120">Possible values are: `allAttendees`, `staff`, `customer`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d8d76-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d8d76-121">JSON representation</span></span>

<span data-ttu-id="d8d76-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d8d76-122">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
