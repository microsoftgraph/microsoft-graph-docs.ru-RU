---
title: Тип ресурса Букингреминдер
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: a87f504824136fc1f3e3639361e22f78c6719dba
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974138"
---
# <a name="bookingreminder-resource-type"></a><span data-ttu-id="c081b-104">Тип ресурса Букингреминдер</span><span class="sxs-lookup"><span data-stu-id="c081b-104">bookingReminder resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="c081b-105">Указывает, когда и кому отправлять напоминания по электронной почте.</span><span class="sxs-lookup"><span data-stu-id="c081b-105">Represents when and to whom to send an email reminder.</span></span>


## <a name="properties"></a><span data-ttu-id="c081b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c081b-106">Properties</span></span>
| <span data-ttu-id="c081b-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c081b-107">Property</span></span>     | <span data-ttu-id="c081b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c081b-108">Type</span></span>   |<span data-ttu-id="c081b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c081b-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c081b-110">message</span><span class="sxs-lookup"><span data-stu-id="c081b-110">message</span></span>|<span data-ttu-id="c081b-111">String</span><span class="sxs-lookup"><span data-stu-id="c081b-111">String</span></span>|<span data-ttu-id="c081b-112">Сообщение в памятке.</span><span class="sxs-lookup"><span data-stu-id="c081b-112">The message in the reminder.</span></span>|
|<span data-ttu-id="c081b-113">корреспондирующей</span><span class="sxs-lookup"><span data-stu-id="c081b-113">offset</span></span>|<span data-ttu-id="c081b-114">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="c081b-114">Duration</span></span>|<span data-ttu-id="c081b-115">Количество времени до начала встречи, в которое будет отправлено напоминание.</span><span class="sxs-lookup"><span data-stu-id="c081b-115">The amount of time before the start of an appointment that the reminder should be sent.</span></span> <span data-ttu-id="c081b-116">Он отмечен в формате [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="c081b-116">It's denoted in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="c081b-117">recipients</span><span class="sxs-lookup"><span data-stu-id="c081b-117">recipients</span></span>|<span data-ttu-id="c081b-118">String</span><span class="sxs-lookup"><span data-stu-id="c081b-118">String</span></span>| <span data-ttu-id="c081b-119">Лица, шауолд получать напоминание.</span><span class="sxs-lookup"><span data-stu-id="c081b-119">The persons who shouold receive the reminder.</span></span> <span data-ttu-id="c081b-120">Возможные значения: `allAttendees`, `staff`, `customer`.</span><span class="sxs-lookup"><span data-stu-id="c081b-120">Possible values are: `allAttendees`, `staff`, `customer`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c081b-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c081b-121">JSON representation</span></span>

<span data-ttu-id="c081b-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c081b-122">The following is a JSON representation of the resource.</span></span>

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
