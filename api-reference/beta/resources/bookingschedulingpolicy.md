---
title: Тип ресурса bookingSchedulingPolicy
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 3dee3314818d46c4131526dc92565eb4f8ca6ea2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523451"
---
# <a name="bookingschedulingpolicy-resource-type"></a><span data-ttu-id="9a072-104">Тип ресурса bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="9a072-104">bookingSchedulingPolicy resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="9a072-105">Представляет набор политик, определяющие способ создания встреч в календаре Microsoft резервирования.</span><span class="sxs-lookup"><span data-stu-id="9a072-105">Represents the set of policies that determine how appointments should be created in a Microsoft Bookings calendar.</span></span>

## <a name="properties"></a><span data-ttu-id="9a072-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="9a072-106">Properties</span></span>
| <span data-ttu-id="9a072-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="9a072-107">Property</span></span>     | <span data-ttu-id="9a072-108">Тип</span><span class="sxs-lookup"><span data-stu-id="9a072-108">Type</span></span>   |<span data-ttu-id="9a072-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9a072-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9a072-110">allowStaffSelection</span><span class="sxs-lookup"><span data-stu-id="9a072-110">allowStaffSelection</span></span>|<span data-ttu-id="9a072-111">Логическое</span><span class="sxs-lookup"><span data-stu-id="9a072-111">Boolean</span></span>|<span data-ttu-id="9a072-112">True, если разрешить пользователям выбрать определенным человеком резервирования.</span><span class="sxs-lookup"><span data-stu-id="9a072-112">True if to allow customers to choose a specific person for the booking.</span></span>|
|<span data-ttu-id="9a072-113">maximumAdvance</span><span class="sxs-lookup"><span data-stu-id="9a072-113">maximumAdvance</span></span>|<span data-ttu-id="9a072-114">Длительность</span><span class="sxs-lookup"><span data-stu-id="9a072-114">Duration</span></span>|<span data-ttu-id="9a072-115">Максимальное количество дней, которые могут поступать резервирования.</span><span class="sxs-lookup"><span data-stu-id="9a072-115">Maximum number of days in advance that a booking can be made.</span></span> <span data-ttu-id="9a072-116">Следует формате [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="9a072-116">It follows the [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="9a072-117">minimumLeadTime</span><span class="sxs-lookup"><span data-stu-id="9a072-117">minimumLeadTime</span></span>|<span data-ttu-id="9a072-118">Длительность</span><span class="sxs-lookup"><span data-stu-id="9a072-118">Duration</span></span>|<span data-ttu-id="9a072-119">Минимальное количество времени, созданные ранее которой должна состоять резервирования и отмены ресурса.</span><span class="sxs-lookup"><span data-stu-id="9a072-119">The minimum amount of time before which bookings and cancellations must be made.</span></span> <span data-ttu-id="9a072-120">Следует формате [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="9a072-120">It follows the [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="9a072-121">sendConfirmationsToOwner</span><span class="sxs-lookup"><span data-stu-id="9a072-121">sendConfirmationsToOwner</span></span>|<span data-ttu-id="9a072-122">Логическое</span><span class="sxs-lookup"><span data-stu-id="9a072-122">Boolean</span></span>| <span data-ttu-id="9a072-123">Значение true для уведомления business по электронной почте при создании или изменении резервирования.</span><span class="sxs-lookup"><span data-stu-id="9a072-123">True to notify the business via email when a booking is created or changed.</span></span> <span data-ttu-id="9a072-124">Используйте адрес электронной почты, указанных в свойстве **электронной почты** объекта **bookingBusiness** для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="9a072-124">Use the email address specified in the **email** property of the **bookingBusiness** entity for the business.</span></span> |
|<span data-ttu-id="9a072-125">timeSlotInterval</span><span class="sxs-lookup"><span data-stu-id="9a072-125">timeSlotInterval</span></span>|<span data-ttu-id="9a072-126">Длительность</span><span class="sxs-lookup"><span data-stu-id="9a072-126">Duration</span></span>|<span data-ttu-id="9a072-127">Продолжительность каждого промежуток времени, идентификаторами в формате [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="9a072-127">Duration of each time slot, denoted in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9a072-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9a072-128">JSON representation</span></span>

<span data-ttu-id="9a072-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9a072-129">The following is a JSON representation of the resource.</span></span>

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
