---
title: Тип ресурса bookingSchedulingPolicy
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 039d76b00787c9bf2e4f0bee4eb927a7628a9e76
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914640"
---
# <a name="bookingschedulingpolicy-resource-type"></a><span data-ttu-id="7d5ac-104">Тип ресурса bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="7d5ac-104">bookingSchedulingPolicy resource type</span></span>

 > <span data-ttu-id="7d5ac-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7d5ac-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7d5ac-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d5ac-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="7d5ac-107">Представляет набор политик, определяющие способ создания встреч в календаре Microsoft резервирования.</span><span class="sxs-lookup"><span data-stu-id="7d5ac-107">Represents the set of policies that determine how appointments should be created in a Microsoft Bookings calendar.</span></span>

## <a name="properties"></a><span data-ttu-id="7d5ac-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="7d5ac-108">Properties</span></span>
| <span data-ttu-id="7d5ac-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="7d5ac-109">Property</span></span>     | <span data-ttu-id="7d5ac-110">Тип</span><span class="sxs-lookup"><span data-stu-id="7d5ac-110">Type</span></span>   |<span data-ttu-id="7d5ac-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7d5ac-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7d5ac-112">allowStaffSelection</span><span class="sxs-lookup"><span data-stu-id="7d5ac-112">allowStaffSelection</span></span>|<span data-ttu-id="7d5ac-113">Логический</span><span class="sxs-lookup"><span data-stu-id="7d5ac-113">Boolean</span></span>|<span data-ttu-id="7d5ac-114">True, если разрешить пользователям выбрать определенным человеком резервирования.</span><span class="sxs-lookup"><span data-stu-id="7d5ac-114">True if to allow customers to choose a specific person for the booking.</span></span>|
|<span data-ttu-id="7d5ac-115">maximumAdvance</span><span class="sxs-lookup"><span data-stu-id="7d5ac-115">maximumAdvance</span></span>|<span data-ttu-id="7d5ac-116">Продолжительность</span><span class="sxs-lookup"><span data-stu-id="7d5ac-116">Duration</span></span>|<span data-ttu-id="7d5ac-117">Максимальное количество дней, которые могут поступать резервирования.</span><span class="sxs-lookup"><span data-stu-id="7d5ac-117">Maximum number of days in advance that a booking can be made.</span></span> <span data-ttu-id="7d5ac-118">Следует формате [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="7d5ac-118">It follows the [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="7d5ac-119">minimumLeadTime</span><span class="sxs-lookup"><span data-stu-id="7d5ac-119">minimumLeadTime</span></span>|<span data-ttu-id="7d5ac-120">Продолжительность</span><span class="sxs-lookup"><span data-stu-id="7d5ac-120">Duration</span></span>|<span data-ttu-id="7d5ac-121">Минимальное количество времени, созданные ранее которой должна состоять резервирования и отмены ресурса.</span><span class="sxs-lookup"><span data-stu-id="7d5ac-121">The minimum amount of time before which bookings and cancellations must be made.</span></span> <span data-ttu-id="7d5ac-122">Следует формате [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="7d5ac-122">It follows the [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="7d5ac-123">sendConfirmationsToOwner</span><span class="sxs-lookup"><span data-stu-id="7d5ac-123">sendConfirmationsToOwner</span></span>|<span data-ttu-id="7d5ac-124">Логический</span><span class="sxs-lookup"><span data-stu-id="7d5ac-124">Boolean</span></span>| <span data-ttu-id="7d5ac-125">Значение true для уведомления business по электронной почте при создании или изменении резервирования.</span><span class="sxs-lookup"><span data-stu-id="7d5ac-125">True to notify the business via email when a booking is created or changed.</span></span> <span data-ttu-id="7d5ac-126">Используйте адрес электронной почты, указанных в свойстве **электронной почты** объекта **bookingBusiness** для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="7d5ac-126">Use the email address specified in the **email** property of the **bookingBusiness** entity for the business.</span></span> |
|<span data-ttu-id="7d5ac-127">timeSlotInterval</span><span class="sxs-lookup"><span data-stu-id="7d5ac-127">timeSlotInterval</span></span>|<span data-ttu-id="7d5ac-128">Продолжительность</span><span class="sxs-lookup"><span data-stu-id="7d5ac-128">Duration</span></span>|<span data-ttu-id="7d5ac-129">Продолжительность каждого промежуток времени, идентификаторами в формате [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="7d5ac-129">Duration of each time slot, denoted in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7d5ac-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7d5ac-130">JSON representation</span></span>

<span data-ttu-id="7d5ac-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7d5ac-131">The following is a JSON representation of the resource.</span></span>

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
