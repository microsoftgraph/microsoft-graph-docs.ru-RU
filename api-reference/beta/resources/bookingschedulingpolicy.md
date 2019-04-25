---
title: Тип ресурса Букингсчедулингполици
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 3dee3314818d46c4131526dc92565eb4f8ca6ea2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543774"
---
# <a name="bookingschedulingpolicy-resource-type"></a><span data-ttu-id="13d2e-104">Тип ресурса Букингсчедулингполици</span><span class="sxs-lookup"><span data-stu-id="13d2e-104">bookingSchedulingPolicy resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="13d2e-105">Представляет набор политик, определяющих, как будут создаваться встречи в календаре Microsoft Books.</span><span class="sxs-lookup"><span data-stu-id="13d2e-105">Represents the set of policies that determine how appointments should be created in a Microsoft Bookings calendar.</span></span>

## <a name="properties"></a><span data-ttu-id="13d2e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="13d2e-106">Properties</span></span>
| <span data-ttu-id="13d2e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="13d2e-107">Property</span></span>     | <span data-ttu-id="13d2e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="13d2e-108">Type</span></span>   |<span data-ttu-id="13d2e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="13d2e-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="13d2e-110">Алловстаффселектион</span><span class="sxs-lookup"><span data-stu-id="13d2e-110">allowStaffSelection</span></span>|<span data-ttu-id="13d2e-111">Логический</span><span class="sxs-lookup"><span data-stu-id="13d2e-111">Boolean</span></span>|<span data-ttu-id="13d2e-112">Значение true, если необходимо разрешить клиентам выбирать определенного человека для резервирования.</span><span class="sxs-lookup"><span data-stu-id="13d2e-112">True if to allow customers to choose a specific person for the booking.</span></span>|
|<span data-ttu-id="13d2e-113">Максимумадванце</span><span class="sxs-lookup"><span data-stu-id="13d2e-113">maximumAdvance</span></span>|<span data-ttu-id="13d2e-114">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="13d2e-114">Duration</span></span>|<span data-ttu-id="13d2e-115">Максимальное количество дней, в течение которых можно выполнить резервирование.</span><span class="sxs-lookup"><span data-stu-id="13d2e-115">Maximum number of days in advance that a booking can be made.</span></span> <span data-ttu-id="13d2e-116">Он соответствует формату [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="13d2e-116">It follows the [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="13d2e-117">Минимумлеадтиме</span><span class="sxs-lookup"><span data-stu-id="13d2e-117">minimumLeadTime</span></span>|<span data-ttu-id="13d2e-118">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="13d2e-118">Duration</span></span>|<span data-ttu-id="13d2e-119">Минимальное время, по истечении которого должны выполняться резервирования и отмены.</span><span class="sxs-lookup"><span data-stu-id="13d2e-119">The minimum amount of time before which bookings and cancellations must be made.</span></span> <span data-ttu-id="13d2e-120">Он соответствует формату [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="13d2e-120">It follows the [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="13d2e-121">Сендконфирматионстувнер</span><span class="sxs-lookup"><span data-stu-id="13d2e-121">sendConfirmationsToOwner</span></span>|<span data-ttu-id="13d2e-122">Логический</span><span class="sxs-lookup"><span data-stu-id="13d2e-122">Boolean</span></span>| <span data-ttu-id="13d2e-123">Значение true, чтобы уведомить бизнес по электронной почте при создании или изменении резервирования.</span><span class="sxs-lookup"><span data-stu-id="13d2e-123">True to notify the business via email when a booking is created or changed.</span></span> <span data-ttu-id="13d2e-124">Используйте адрес электронной почты, указанный в свойстве **Email** объекта **букингбусинесс** для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="13d2e-124">Use the email address specified in the **email** property of the **bookingBusiness** entity for the business.</span></span> |
|<span data-ttu-id="13d2e-125">Тимеслотинтервал</span><span class="sxs-lookup"><span data-stu-id="13d2e-125">timeSlotInterval</span></span>|<span data-ttu-id="13d2e-126">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="13d2e-126">Duration</span></span>|<span data-ttu-id="13d2e-127">Продолжительность каждого интервала времени, обозначенного в формате [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="13d2e-127">Duration of each time slot, denoted in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="13d2e-128">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="13d2e-128">JSON representation</span></span>

<span data-ttu-id="13d2e-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="13d2e-129">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingschedulingpolicy.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
