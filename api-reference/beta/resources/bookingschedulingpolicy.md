---
title: Тип ресурса bookingSchedulingPolicy
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: 15f9e0dea22a7cfb5eab437bcc023fe3387bb2ea
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805365"
---
# <a name="bookingschedulingpolicy-resource-type"></a><span data-ttu-id="6065a-104">Тип ресурса bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="6065a-104">bookingSchedulingPolicy resource type</span></span>

 > <span data-ttu-id="6065a-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6065a-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6065a-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6065a-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="6065a-107">Представляет набор политик, определяющие способ создания встреч в календаре Microsoft резервирования.</span><span class="sxs-lookup"><span data-stu-id="6065a-107">Represents the set of policies that determine how appointments should be created in a Microsoft Bookings calendar.</span></span>

## <a name="properties"></a><span data-ttu-id="6065a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6065a-108">Properties</span></span>
| <span data-ttu-id="6065a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="6065a-109">Property</span></span>     | <span data-ttu-id="6065a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6065a-110">Type</span></span>   |<span data-ttu-id="6065a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6065a-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6065a-112">allowStaffSelection</span><span class="sxs-lookup"><span data-stu-id="6065a-112">allowStaffSelection</span></span>|<span data-ttu-id="6065a-113">Логический</span><span class="sxs-lookup"><span data-stu-id="6065a-113">Boolean</span></span>|<span data-ttu-id="6065a-114">True, если разрешить пользователям выбрать определенным человеком резервирования.</span><span class="sxs-lookup"><span data-stu-id="6065a-114">True if to allow customers to choose a specific person for the booking.</span></span>|
|<span data-ttu-id="6065a-115">maximumAdvance</span><span class="sxs-lookup"><span data-stu-id="6065a-115">maximumAdvance</span></span>|<span data-ttu-id="6065a-116">Продолжительность</span><span class="sxs-lookup"><span data-stu-id="6065a-116">Duration</span></span>|<span data-ttu-id="6065a-117">Максимальное количество дней, которые могут поступать резервирования.</span><span class="sxs-lookup"><span data-stu-id="6065a-117">Maximum number of days in advance that a booking can be made.</span></span> <span data-ttu-id="6065a-118">Следует формате [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="6065a-118">It follows the [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="6065a-119">minimumLeadTime</span><span class="sxs-lookup"><span data-stu-id="6065a-119">minimumLeadTime</span></span>|<span data-ttu-id="6065a-120">Продолжительность</span><span class="sxs-lookup"><span data-stu-id="6065a-120">Duration</span></span>|<span data-ttu-id="6065a-121">Минимальное количество времени, созданные ранее которой должна состоять резервирования и отмены ресурса.</span><span class="sxs-lookup"><span data-stu-id="6065a-121">The minimum amount of time before which bookings and cancellations must be made.</span></span> <span data-ttu-id="6065a-122">Следует формате [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="6065a-122">It follows the [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="6065a-123">sendConfirmationsToOwner</span><span class="sxs-lookup"><span data-stu-id="6065a-123">sendConfirmationsToOwner</span></span>|<span data-ttu-id="6065a-124">Логический</span><span class="sxs-lookup"><span data-stu-id="6065a-124">Boolean</span></span>| <span data-ttu-id="6065a-125">Значение true для уведомления business по электронной почте при создании или изменении резервирования.</span><span class="sxs-lookup"><span data-stu-id="6065a-125">True to notify the business via email when a booking is created or changed.</span></span> <span data-ttu-id="6065a-126">Используйте адрес электронной почты, указанных в свойстве **электронной почты** объекта **bookingBusiness** для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="6065a-126">Use the email address specified in the **email** property of the **bookingBusiness** entity for the business.</span></span> |
|<span data-ttu-id="6065a-127">timeSlotInterval</span><span class="sxs-lookup"><span data-stu-id="6065a-127">timeSlotInterval</span></span>|<span data-ttu-id="6065a-128">Продолжительность</span><span class="sxs-lookup"><span data-stu-id="6065a-128">Duration</span></span>|<span data-ttu-id="6065a-129">Продолжительность каждого промежуток времени, идентификаторами в формате [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="6065a-129">Duration of each time slot, denoted in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6065a-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6065a-130">JSON representation</span></span>

<span data-ttu-id="6065a-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6065a-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingSchedulingPolicy"
}-->

```json
{
  "allowStaffSelection": true,
  "maximumAdvance": "String (timestamp)",
  "minimumLeadTime": "String (timestamp)",
  "sendConfirmationsToOwner": true,
  "timeSlotInterval": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "bookingSchedulingPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
