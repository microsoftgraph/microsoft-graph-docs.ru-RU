---
title: Тип ресурса bookingReminder
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 17cd444b8656c30e8f8966ab14571876ef9354fe
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936699"
---
# <a name="bookingreminder-resource-type"></a><span data-ttu-id="ca2ed-104">Тип ресурса bookingReminder</span><span class="sxs-lookup"><span data-stu-id="ca2ed-104">bookingReminder resource type</span></span>

 > <span data-ttu-id="ca2ed-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ca2ed-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ca2ed-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca2ed-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="ca2ed-107">Представляет при и к которым следует отправить по электронной почте напоминания.</span><span class="sxs-lookup"><span data-stu-id="ca2ed-107">Represents when and to whom to send an email reminder.</span></span>


## <a name="properties"></a><span data-ttu-id="ca2ed-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ca2ed-108">Properties</span></span>
| <span data-ttu-id="ca2ed-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ca2ed-109">Property</span></span>     | <span data-ttu-id="ca2ed-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ca2ed-110">Type</span></span>   |<span data-ttu-id="ca2ed-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ca2ed-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ca2ed-112">message</span><span class="sxs-lookup"><span data-stu-id="ca2ed-112">message</span></span>|<span data-ttu-id="ca2ed-113">String</span><span class="sxs-lookup"><span data-stu-id="ca2ed-113">String</span></span>|<span data-ttu-id="ca2ed-114">Сообщение в напоминания.</span><span class="sxs-lookup"><span data-stu-id="ca2ed-114">The message in the reminder.</span></span>|
|<span data-ttu-id="ca2ed-115">Смещение</span><span class="sxs-lookup"><span data-stu-id="ca2ed-115">offset</span></span>|<span data-ttu-id="ca2ed-116">Продолжительность</span><span class="sxs-lookup"><span data-stu-id="ca2ed-116">Duration</span></span>|<span data-ttu-id="ca2ed-117">Количество времени до начала встречи, на который будут отправляться напоминания.</span><span class="sxs-lookup"><span data-stu-id="ca2ed-117">The amount of time before the start of an appointment that the reminder should be sent.</span></span> <span data-ttu-id="ca2ed-118">Отображаются в формате [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="ca2ed-118">It's denoted in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="ca2ed-119">recipients</span><span class="sxs-lookup"><span data-stu-id="ca2ed-119">recipients</span></span>|<span data-ttu-id="ca2ed-120">Строка</span><span class="sxs-lookup"><span data-stu-id="ca2ed-120">String</span></span>| <span data-ttu-id="ca2ed-121">Лиц, которые shouold получать оповещение.</span><span class="sxs-lookup"><span data-stu-id="ca2ed-121">The persons who shouold receive the reminder.</span></span> <span data-ttu-id="ca2ed-122">Возможные значения: `allAttendees`, `staff`, `customer`.</span><span class="sxs-lookup"><span data-stu-id="ca2ed-122">Possible values are: `allAttendees`, `staff`, `customer`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ca2ed-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ca2ed-123">JSON representation</span></span>

<span data-ttu-id="ca2ed-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ca2ed-124">The following is a JSON representation of the resource.</span></span>

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
