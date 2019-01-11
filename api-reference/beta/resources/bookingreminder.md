---
title: Тип ресурса bookingReminder
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: 1f1708d4ac9606ad5c862cb9b1bc73e1ddcfec4a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853867"
---
# <a name="bookingreminder-resource-type"></a><span data-ttu-id="bc4be-104">Тип ресурса bookingReminder</span><span class="sxs-lookup"><span data-stu-id="bc4be-104">bookingReminder resource type</span></span>

 > <span data-ttu-id="bc4be-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bc4be-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bc4be-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc4be-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="bc4be-107">Представляет при и к которым следует отправить по электронной почте напоминания.</span><span class="sxs-lookup"><span data-stu-id="bc4be-107">Represents when and to whom to send an email reminder.</span></span>


## <a name="properties"></a><span data-ttu-id="bc4be-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="bc4be-108">Properties</span></span>
| <span data-ttu-id="bc4be-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="bc4be-109">Property</span></span>     | <span data-ttu-id="bc4be-110">Тип</span><span class="sxs-lookup"><span data-stu-id="bc4be-110">Type</span></span>   |<span data-ttu-id="bc4be-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bc4be-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bc4be-112">message</span><span class="sxs-lookup"><span data-stu-id="bc4be-112">message</span></span>|<span data-ttu-id="bc4be-113">String</span><span class="sxs-lookup"><span data-stu-id="bc4be-113">String</span></span>|<span data-ttu-id="bc4be-114">Сообщение в напоминания.</span><span class="sxs-lookup"><span data-stu-id="bc4be-114">The message in the reminder.</span></span>|
|<span data-ttu-id="bc4be-115">Смещение</span><span class="sxs-lookup"><span data-stu-id="bc4be-115">offset</span></span>|<span data-ttu-id="bc4be-116">Продолжительность</span><span class="sxs-lookup"><span data-stu-id="bc4be-116">Duration</span></span>|<span data-ttu-id="bc4be-117">Количество времени до начала встречи, на который будут отправляться напоминания.</span><span class="sxs-lookup"><span data-stu-id="bc4be-117">The amount of time before the start of an appointment that the reminder should be sent.</span></span> <span data-ttu-id="bc4be-118">Отображаются в формате [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="bc4be-118">It's denoted in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="bc4be-119">recipients</span><span class="sxs-lookup"><span data-stu-id="bc4be-119">recipients</span></span>|<span data-ttu-id="bc4be-120">Строка</span><span class="sxs-lookup"><span data-stu-id="bc4be-120">String</span></span>| <span data-ttu-id="bc4be-121">Лиц, которые shouold получать оповещение.</span><span class="sxs-lookup"><span data-stu-id="bc4be-121">The persons who shouold receive the reminder.</span></span> <span data-ttu-id="bc4be-122">Возможные значения: `allAttendees`, `staff`, `customer`.</span><span class="sxs-lookup"><span data-stu-id="bc4be-122">Possible values are: `allAttendees`, `staff`, `customer`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bc4be-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bc4be-123">JSON representation</span></span>

<span data-ttu-id="bc4be-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bc4be-124">The following is a JSON representation of the resource.</span></span>

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
