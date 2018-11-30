---
title: Тип ресурса bookingReminder
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
ms.openlocfilehash: f5f7b30c296433dd96ffa14a75e3f0286e8a16a1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079008"
---
# <a name="bookingreminder-resource-type"></a><span data-ttu-id="7c6e1-104">Тип ресурса bookingReminder</span><span class="sxs-lookup"><span data-stu-id="7c6e1-104">bookingReminder resource type</span></span>

 > <span data-ttu-id="7c6e1-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7c6e1-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7c6e1-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c6e1-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="7c6e1-107">Представляет при и к которым следует отправить по электронной почте напоминания.</span><span class="sxs-lookup"><span data-stu-id="7c6e1-107">Represents when and to whom to send an email reminder.</span></span>


## <a name="properties"></a><span data-ttu-id="7c6e1-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="7c6e1-108">Properties</span></span>
| <span data-ttu-id="7c6e1-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="7c6e1-109">Property</span></span>     | <span data-ttu-id="7c6e1-110">Тип</span><span class="sxs-lookup"><span data-stu-id="7c6e1-110">Type</span></span>   |<span data-ttu-id="7c6e1-111">Description</span><span class="sxs-lookup"><span data-stu-id="7c6e1-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7c6e1-112">message</span><span class="sxs-lookup"><span data-stu-id="7c6e1-112">message</span></span>|<span data-ttu-id="7c6e1-113">String</span><span class="sxs-lookup"><span data-stu-id="7c6e1-113">String</span></span>|<span data-ttu-id="7c6e1-114">Сообщение в напоминания.</span><span class="sxs-lookup"><span data-stu-id="7c6e1-114">The message in the reminder.</span></span>|
|<span data-ttu-id="7c6e1-115">Смещение</span><span class="sxs-lookup"><span data-stu-id="7c6e1-115">offset</span></span>|<span data-ttu-id="7c6e1-116">Продолжительность</span><span class="sxs-lookup"><span data-stu-id="7c6e1-116">Duration</span></span>|<span data-ttu-id="7c6e1-117">Количество времени до начала встречи, на который будут отправляться напоминания.</span><span class="sxs-lookup"><span data-stu-id="7c6e1-117">The amount of time before the start of an appointment that the reminder should be sent.</span></span> <span data-ttu-id="7c6e1-118">Отображаются в формате [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="7c6e1-118">It's denoted in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="7c6e1-119">recipients</span><span class="sxs-lookup"><span data-stu-id="7c6e1-119">recipients</span></span>|<span data-ttu-id="7c6e1-120">String</span><span class="sxs-lookup"><span data-stu-id="7c6e1-120">String</span></span>| <span data-ttu-id="7c6e1-121">Лиц, которые shouold получать оповещение.</span><span class="sxs-lookup"><span data-stu-id="7c6e1-121">The persons who shouold receive the reminder.</span></span> <span data-ttu-id="7c6e1-122">Возможные значения: `allAttendees`, `staff`, `customer`.</span><span class="sxs-lookup"><span data-stu-id="7c6e1-122">Possible values are: `allAttendees`, `staff`, `customer`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7c6e1-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7c6e1-123">JSON representation</span></span>

<span data-ttu-id="7c6e1-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7c6e1-124">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "bookingReminder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->