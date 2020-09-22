---
title: Тип ресурса Букингсчедулингполици
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 5839ad12b746f83e2e41648ded6ce35346e97f28
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071768"
---
# <a name="bookingschedulingpolicy-resource-type"></a><span data-ttu-id="61fd5-104">Тип ресурса Букингсчедулингполици</span><span class="sxs-lookup"><span data-stu-id="61fd5-104">bookingSchedulingPolicy resource type</span></span>

<span data-ttu-id="61fd5-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61fd5-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="61fd5-106">Представляет набор политик, определяющих, как будут создаваться встречи в календаре Microsoft Books.</span><span class="sxs-lookup"><span data-stu-id="61fd5-106">Represents the set of policies that determine how appointments should be created in a Microsoft Bookings calendar.</span></span>

## <a name="properties"></a><span data-ttu-id="61fd5-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="61fd5-107">Properties</span></span>
| <span data-ttu-id="61fd5-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="61fd5-108">Property</span></span>     | <span data-ttu-id="61fd5-109">Тип</span><span class="sxs-lookup"><span data-stu-id="61fd5-109">Type</span></span>   |<span data-ttu-id="61fd5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="61fd5-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="61fd5-111">алловстаффселектион</span><span class="sxs-lookup"><span data-stu-id="61fd5-111">allowStaffSelection</span></span>|<span data-ttu-id="61fd5-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="61fd5-112">Boolean</span></span>|<span data-ttu-id="61fd5-113">Значение true, если необходимо разрешить клиентам выбирать определенного человека для резервирования.</span><span class="sxs-lookup"><span data-stu-id="61fd5-113">True if to allow customers to choose a specific person for the booking.</span></span>|
|<span data-ttu-id="61fd5-114">максимумадванце</span><span class="sxs-lookup"><span data-stu-id="61fd5-114">maximumAdvance</span></span>|<span data-ttu-id="61fd5-115">Длительность</span><span class="sxs-lookup"><span data-stu-id="61fd5-115">Duration</span></span>|<span data-ttu-id="61fd5-116">Максимальное количество дней, в течение которых можно выполнить резервирование.</span><span class="sxs-lookup"><span data-stu-id="61fd5-116">Maximum number of days in advance that a booking can be made.</span></span> <span data-ttu-id="61fd5-117">Он соответствует формату [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="61fd5-117">It follows the [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="61fd5-118">минимумлеадтиме</span><span class="sxs-lookup"><span data-stu-id="61fd5-118">minimumLeadTime</span></span>|<span data-ttu-id="61fd5-119">Длительность</span><span class="sxs-lookup"><span data-stu-id="61fd5-119">Duration</span></span>|<span data-ttu-id="61fd5-120">Минимальное время, по истечении которого должны выполняться резервирования и отмены.</span><span class="sxs-lookup"><span data-stu-id="61fd5-120">The minimum amount of time before which bookings and cancellations must be made.</span></span> <span data-ttu-id="61fd5-121">Он соответствует формату [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="61fd5-121">It follows the [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="61fd5-122">сендконфирматионстувнер</span><span class="sxs-lookup"><span data-stu-id="61fd5-122">sendConfirmationsToOwner</span></span>|<span data-ttu-id="61fd5-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="61fd5-123">Boolean</span></span>| <span data-ttu-id="61fd5-124">Значение true, чтобы уведомить бизнес по электронной почте при создании или изменении резервирования.</span><span class="sxs-lookup"><span data-stu-id="61fd5-124">True to notify the business via email when a booking is created or changed.</span></span> <span data-ttu-id="61fd5-125">Используйте адрес электронной почты, указанный в свойстве **Email** объекта **букингбусинесс** для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="61fd5-125">Use the email address specified in the **email** property of the **bookingBusiness** entity for the business.</span></span> |
|<span data-ttu-id="61fd5-126">тимеслотинтервал</span><span class="sxs-lookup"><span data-stu-id="61fd5-126">timeSlotInterval</span></span>|<span data-ttu-id="61fd5-127">Длительность</span><span class="sxs-lookup"><span data-stu-id="61fd5-127">Duration</span></span>|<span data-ttu-id="61fd5-128">Продолжительность каждого интервала времени, обозначенного в формате [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="61fd5-128">Duration of each time slot, denoted in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="61fd5-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="61fd5-129">JSON representation</span></span>

<span data-ttu-id="61fd5-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="61fd5-130">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "bookingSchedulingPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


