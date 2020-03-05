---
title: Тип ресурса Букингреминдер
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 685f4136b5b16c09d8fa53c385d75312a9337870
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507917"
---
# <a name="bookingreminder-resource-type"></a><span data-ttu-id="3d620-104">Тип ресурса Букингреминдер</span><span class="sxs-lookup"><span data-stu-id="3d620-104">bookingReminder resource type</span></span>

<span data-ttu-id="3d620-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3d620-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="3d620-106">Указывает, когда и кому отправлять напоминания по электронной почте.</span><span class="sxs-lookup"><span data-stu-id="3d620-106">Represents when and to whom to send an email reminder.</span></span>


## <a name="properties"></a><span data-ttu-id="3d620-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="3d620-107">Properties</span></span>
| <span data-ttu-id="3d620-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="3d620-108">Property</span></span>     | <span data-ttu-id="3d620-109">Тип</span><span class="sxs-lookup"><span data-stu-id="3d620-109">Type</span></span>   |<span data-ttu-id="3d620-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3d620-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3d620-111">message</span><span class="sxs-lookup"><span data-stu-id="3d620-111">message</span></span>|<span data-ttu-id="3d620-112">String</span><span class="sxs-lookup"><span data-stu-id="3d620-112">String</span></span>|<span data-ttu-id="3d620-113">Сообщение в памятке.</span><span class="sxs-lookup"><span data-stu-id="3d620-113">The message in the reminder.</span></span>|
|<span data-ttu-id="3d620-114">корреспондирующей</span><span class="sxs-lookup"><span data-stu-id="3d620-114">offset</span></span>|<span data-ttu-id="3d620-115">Длительность</span><span class="sxs-lookup"><span data-stu-id="3d620-115">Duration</span></span>|<span data-ttu-id="3d620-116">Количество времени до начала встречи, в которое будет отправлено напоминание.</span><span class="sxs-lookup"><span data-stu-id="3d620-116">The amount of time before the start of an appointment that the reminder should be sent.</span></span> <span data-ttu-id="3d620-117">Он отмечен в формате [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="3d620-117">It's denoted in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="3d620-118">recipients</span><span class="sxs-lookup"><span data-stu-id="3d620-118">recipients</span></span>|<span data-ttu-id="3d620-119">String</span><span class="sxs-lookup"><span data-stu-id="3d620-119">String</span></span>| <span data-ttu-id="3d620-120">Лица, шауолд получать напоминание.</span><span class="sxs-lookup"><span data-stu-id="3d620-120">The persons who shouold receive the reminder.</span></span> <span data-ttu-id="3d620-121">Возможные значения: `allAttendees`, `staff`, `customer`.</span><span class="sxs-lookup"><span data-stu-id="3d620-121">Possible values are: `allAttendees`, `staff`, `customer`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3d620-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3d620-122">JSON representation</span></span>

<span data-ttu-id="3d620-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3d620-123">The following is a JSON representation of the resource.</span></span>

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
