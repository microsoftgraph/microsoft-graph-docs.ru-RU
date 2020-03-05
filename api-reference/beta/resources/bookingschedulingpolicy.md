---
title: Тип ресурса Букингсчедулингполици
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: edc456aaa03cc54bd7b385bc97d37eb657ea53b2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507910"
---
# <a name="bookingschedulingpolicy-resource-type"></a><span data-ttu-id="2e5c6-104">Тип ресурса Букингсчедулингполици</span><span class="sxs-lookup"><span data-stu-id="2e5c6-104">bookingSchedulingPolicy resource type</span></span>

<span data-ttu-id="2e5c6-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2e5c6-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="2e5c6-106">Представляет набор политик, определяющих, как будут создаваться встречи в календаре Microsoft Books.</span><span class="sxs-lookup"><span data-stu-id="2e5c6-106">Represents the set of policies that determine how appointments should be created in a Microsoft Bookings calendar.</span></span>

## <a name="properties"></a><span data-ttu-id="2e5c6-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2e5c6-107">Properties</span></span>
| <span data-ttu-id="2e5c6-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2e5c6-108">Property</span></span>     | <span data-ttu-id="2e5c6-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2e5c6-109">Type</span></span>   |<span data-ttu-id="2e5c6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2e5c6-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2e5c6-111">алловстаффселектион</span><span class="sxs-lookup"><span data-stu-id="2e5c6-111">allowStaffSelection</span></span>|<span data-ttu-id="2e5c6-112">Логический</span><span class="sxs-lookup"><span data-stu-id="2e5c6-112">Boolean</span></span>|<span data-ttu-id="2e5c6-113">Значение true, если необходимо разрешить клиентам выбирать определенного человека для резервирования.</span><span class="sxs-lookup"><span data-stu-id="2e5c6-113">True if to allow customers to choose a specific person for the booking.</span></span>|
|<span data-ttu-id="2e5c6-114">максимумадванце</span><span class="sxs-lookup"><span data-stu-id="2e5c6-114">maximumAdvance</span></span>|<span data-ttu-id="2e5c6-115">Длительность</span><span class="sxs-lookup"><span data-stu-id="2e5c6-115">Duration</span></span>|<span data-ttu-id="2e5c6-116">Максимальное количество дней, в течение которых можно выполнить резервирование.</span><span class="sxs-lookup"><span data-stu-id="2e5c6-116">Maximum number of days in advance that a booking can be made.</span></span> <span data-ttu-id="2e5c6-117">Он соответствует формату [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="2e5c6-117">It follows the [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="2e5c6-118">минимумлеадтиме</span><span class="sxs-lookup"><span data-stu-id="2e5c6-118">minimumLeadTime</span></span>|<span data-ttu-id="2e5c6-119">Длительность</span><span class="sxs-lookup"><span data-stu-id="2e5c6-119">Duration</span></span>|<span data-ttu-id="2e5c6-120">Минимальное время, по истечении которого должны выполняться резервирования и отмены.</span><span class="sxs-lookup"><span data-stu-id="2e5c6-120">The minimum amount of time before which bookings and cancellations must be made.</span></span> <span data-ttu-id="2e5c6-121">Он соответствует формату [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="2e5c6-121">It follows the [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="2e5c6-122">сендконфирматионстувнер</span><span class="sxs-lookup"><span data-stu-id="2e5c6-122">sendConfirmationsToOwner</span></span>|<span data-ttu-id="2e5c6-123">Логический</span><span class="sxs-lookup"><span data-stu-id="2e5c6-123">Boolean</span></span>| <span data-ttu-id="2e5c6-124">Значение true, чтобы уведомить бизнес по электронной почте при создании или изменении резервирования.</span><span class="sxs-lookup"><span data-stu-id="2e5c6-124">True to notify the business via email when a booking is created or changed.</span></span> <span data-ttu-id="2e5c6-125">Используйте адрес электронной почты, указанный в свойстве **Email** объекта **букингбусинесс** для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="2e5c6-125">Use the email address specified in the **email** property of the **bookingBusiness** entity for the business.</span></span> |
|<span data-ttu-id="2e5c6-126">тимеслотинтервал</span><span class="sxs-lookup"><span data-stu-id="2e5c6-126">timeSlotInterval</span></span>|<span data-ttu-id="2e5c6-127">Длительность</span><span class="sxs-lookup"><span data-stu-id="2e5c6-127">Duration</span></span>|<span data-ttu-id="2e5c6-128">Продолжительность каждого интервала времени, обозначенного в формате [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="2e5c6-128">Duration of each time slot, denoted in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2e5c6-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2e5c6-129">JSON representation</span></span>

<span data-ttu-id="2e5c6-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2e5c6-130">The following is a JSON representation of the resource.</span></span>

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
