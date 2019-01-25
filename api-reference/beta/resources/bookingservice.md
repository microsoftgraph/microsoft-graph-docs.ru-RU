---
title: Тип ресурса bookingService
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 35e439888b39c81451242f01d2aaae89b65ad8ee
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519887"
---
# <a name="bookingservice-resource-type"></a><span data-ttu-id="33329-104">Тип ресурса bookingService</span><span class="sxs-lookup"><span data-stu-id="33329-104">bookingService resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="33329-105">Представляет сведения об определенной службы, предоставляемые [bookingBusiness](bookingbusiness.md), такие как имя службы, цены и персонала, который обычно предоставляет такие службы.</span><span class="sxs-lookup"><span data-stu-id="33329-105">Represents information about a particular service provided by a [bookingBusiness](bookingbusiness.md), such as the service name, price, and the staff that usually provides such service.</span></span>

## <a name="methods"></a><span data-ttu-id="33329-106">Методы</span><span class="sxs-lookup"><span data-stu-id="33329-106">Methods</span></span>

| <span data-ttu-id="33329-107">Метод</span><span class="sxs-lookup"><span data-stu-id="33329-107">Method</span></span>           | <span data-ttu-id="33329-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="33329-108">Return Type</span></span>    |<span data-ttu-id="33329-109">Описание</span><span class="sxs-lookup"><span data-stu-id="33329-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="33329-110">Список служб</span><span class="sxs-lookup"><span data-stu-id="33329-110">List services</span></span>](../api/bookingbusiness-list-services.md) | <span data-ttu-id="33329-111">[bookingService](bookingservice.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="33329-111">[bookingService](bookingservice.md) collection</span></span> | <span data-ttu-id="33329-112">Получите список объектов **bookingService** в указанном [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="33329-112">Get a list of **bookingService** objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="33329-113">Создание bookingService</span><span class="sxs-lookup"><span data-stu-id="33329-113">Create bookingService</span></span>](../api/bookingbusiness-post-services.md) | [<span data-ttu-id="33329-114">bookingService</span><span class="sxs-lookup"><span data-stu-id="33329-114">bookingService</span></span>](bookingservice.md) | <span data-ttu-id="33329-115">Создание **bookingService** для указанного [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="33329-115">Create a **bookingService** for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="33329-116">Получение bookingService</span><span class="sxs-lookup"><span data-stu-id="33329-116">Get bookingService</span></span>](../api/bookingservice-get.md) | [<span data-ttu-id="33329-117">bookingService</span><span class="sxs-lookup"><span data-stu-id="33329-117">bookingService</span></span>](bookingservice.md) |<span data-ttu-id="33329-118">Получите свойства и связи объекта **bookingService** в указанном [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="33329-118">Get the properties and relationships of a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="33329-119">Update</span><span class="sxs-lookup"><span data-stu-id="33329-119">Update</span></span>](../api/bookingservice-update.md) | [<span data-ttu-id="33329-120">bookingService</span><span class="sxs-lookup"><span data-stu-id="33329-120">bookingService</span></span>](bookingservice.md)    |<span data-ttu-id="33329-121">Обновление объекта **bookingService** в указанном [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="33329-121">Update a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="33329-122">Delete</span><span class="sxs-lookup"><span data-stu-id="33329-122">Delete</span></span>](../api/bookingservice-delete.md) | <span data-ttu-id="33329-123">Нет</span><span class="sxs-lookup"><span data-stu-id="33329-123">None</span></span> |<span data-ttu-id="33329-124">Удаление объекта **bookingService** в указанном [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="33329-124">Delete a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |

## <a name="properties"></a><span data-ttu-id="33329-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="33329-125">Properties</span></span>
| <span data-ttu-id="33329-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="33329-126">Property</span></span>     | <span data-ttu-id="33329-127">Тип</span><span class="sxs-lookup"><span data-stu-id="33329-127">Type</span></span>   |<span data-ttu-id="33329-128">Описание</span><span class="sxs-lookup"><span data-stu-id="33329-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="33329-129">defaultDuration</span><span class="sxs-lookup"><span data-stu-id="33329-129">defaultDuration</span></span>|<span data-ttu-id="33329-130">Длительность</span><span class="sxs-lookup"><span data-stu-id="33329-130">Duration</span></span>|<span data-ttu-id="33329-131">Длина по умолчанию службы, представленный в числа дней, часов, минут и секунд.</span><span class="sxs-lookup"><span data-stu-id="33329-131">The default length of the service, represented in numbers of days, hours, minutes, and seconds.</span></span> <span data-ttu-id="33329-132">Например P11D23H59M59.999999999999S.</span><span class="sxs-lookup"><span data-stu-id="33329-132">For example, P11D23H59M59.999999999999S.</span></span> |
|<span data-ttu-id="33329-133">defaultLocation</span><span class="sxs-lookup"><span data-stu-id="33329-133">defaultLocation</span></span>|[<span data-ttu-id="33329-134">location</span><span class="sxs-lookup"><span data-stu-id="33329-134">location</span></span>](location.md)|<span data-ttu-id="33329-135">Физическое расположение по умолчанию для службы.</span><span class="sxs-lookup"><span data-stu-id="33329-135">The default physical location for the service.</span></span>|
|<span data-ttu-id="33329-136">defaultPrice</span><span class="sxs-lookup"><span data-stu-id="33329-136">defaultPrice</span></span>|<span data-ttu-id="33329-137">Double</span><span class="sxs-lookup"><span data-stu-id="33329-137">Double</span></span>|<span data-ttu-id="33329-138">Денежные Цена по умолчанию для службы.</span><span class="sxs-lookup"><span data-stu-id="33329-138">The default monetary price for the service.</span></span>|
|<span data-ttu-id="33329-139">defaultPriceType</span><span class="sxs-lookup"><span data-stu-id="33329-139">defaultPriceType</span></span>|<span data-ttu-id="33329-140">string</span><span class="sxs-lookup"><span data-stu-id="33329-140">string</span></span>|<span data-ttu-id="33329-141">По умолчанию способ службу оценивается.</span><span class="sxs-lookup"><span data-stu-id="33329-141">The default way the service is charged.</span></span> <span data-ttu-id="33329-142">Возможные значения: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="33329-142">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="33329-143">defaultReminders</span><span class="sxs-lookup"><span data-stu-id="33329-143">defaultReminders</span></span>|<span data-ttu-id="33329-144">[bookingReminder](bookingreminder.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="33329-144">[bookingReminder](bookingreminder.md) collection</span></span>|<span data-ttu-id="33329-145">Значение по умолчанию набора оповещения о встрече этой службы.</span><span class="sxs-lookup"><span data-stu-id="33329-145">The default set of reminders for an appointment of this service.</span></span> <span data-ttu-id="33329-146">Значение этого свойства доступна только при чтении этой **bookingService** по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="33329-146">The value of this property is available only when reading this **bookingService** by its ID.</span></span>|
|<span data-ttu-id="33329-147">description</span><span class="sxs-lookup"><span data-stu-id="33329-147">description</span></span>|<span data-ttu-id="33329-148">Строка</span><span class="sxs-lookup"><span data-stu-id="33329-148">String</span></span>|<span data-ttu-id="33329-149">Текстовое описание для службы.</span><span class="sxs-lookup"><span data-stu-id="33329-149">A text description for the service.</span></span>|
|<span data-ttu-id="33329-150">displayName</span><span class="sxs-lookup"><span data-stu-id="33329-150">displayName</span></span>|<span data-ttu-id="33329-151">String</span><span class="sxs-lookup"><span data-stu-id="33329-151">String</span></span>|<span data-ttu-id="33329-152">Имя службы.</span><span class="sxs-lookup"><span data-stu-id="33329-152">A service name.</span></span>|
|<span data-ttu-id="33329-153">emailAddress</span><span class="sxs-lookup"><span data-stu-id="33329-153">emailAddress</span></span>|<span data-ttu-id="33329-154">String</span><span class="sxs-lookup"><span data-stu-id="33329-154">String</span></span>|<span data-ttu-id="33329-155">Адрес электронной почты</span><span class="sxs-lookup"><span data-stu-id="33329-155">An email address</span></span>|
|<span data-ttu-id="33329-156">id</span><span class="sxs-lookup"><span data-stu-id="33329-156">id</span></span>|<span data-ttu-id="33329-157">String</span><span class="sxs-lookup"><span data-stu-id="33329-157">String</span></span>|<span data-ttu-id="33329-158">Идентификатор службы, в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="33329-158">The ID of that service, in a GUID format.</span></span> <span data-ttu-id="33329-159">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="33329-159">Read-only.</span></span>|
|<span data-ttu-id="33329-160">isHiddenFromCustomers</span><span class="sxs-lookup"><span data-stu-id="33329-160">isHiddenFromCustomers</span></span>|<span data-ttu-id="33329-161">Логическое</span><span class="sxs-lookup"><span data-stu-id="33329-161">Boolean</span></span>|<span data-ttu-id="33329-162">Значение true означает, что эта служба недоступна для клиентов для резервирования.</span><span class="sxs-lookup"><span data-stu-id="33329-162">True means this service is not available to customers for booking.</span></span>|
|<span data-ttu-id="33329-163">notes</span><span class="sxs-lookup"><span data-stu-id="33329-163">notes</span></span>|<span data-ttu-id="33329-164">String</span><span class="sxs-lookup"><span data-stu-id="33329-164">String</span></span>|<span data-ttu-id="33329-165">Дополнительные сведения об этой службы.</span><span class="sxs-lookup"><span data-stu-id="33329-165">Additional information about this service.</span></span>|
|<span data-ttu-id="33329-166">postBuffer</span><span class="sxs-lookup"><span data-stu-id="33329-166">postBuffer</span></span>|<span data-ttu-id="33329-167">Длительность</span><span class="sxs-lookup"><span data-stu-id="33329-167">Duration</span></span>|<span data-ttu-id="33329-168">Заканчивается время буфер после встречи для этой службы и перед следующим встречи клиента можно заранее.</span><span class="sxs-lookup"><span data-stu-id="33329-168">The time to buffer after an appointment for this service ends, and before the next customer appointment can be booked.</span></span>|
|<span data-ttu-id="33329-169">пребуфер</span><span class="sxs-lookup"><span data-stu-id="33329-169">preBuffer</span></span>|<span data-ttu-id="33329-170">Длительность</span><span class="sxs-lookup"><span data-stu-id="33329-170">Duration</span></span>|<span data-ttu-id="33329-171">Время для буфера до начала встречи для этой службы.</span><span class="sxs-lookup"><span data-stu-id="33329-171">The time to buffer before an appointment for this service can start.</span></span>|
|<span data-ttu-id="33329-172">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="33329-172">schedulingPolicy</span></span>|[<span data-ttu-id="33329-173">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="33329-173">bookingSchedulingPolicy</span></span>](bookingschedulingpolicy.md)|<span data-ttu-id="33329-174">Набор политик, определяющие порядок встреч для этого типа службы следует создания и управления.</span><span class="sxs-lookup"><span data-stu-id="33329-174">The set of policies that determine how appointments for this type of service should be created and managed.</span></span>|
|<span data-ttu-id="33329-175">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="33329-175">staffMemberIds</span></span>|<span data-ttu-id="33329-176">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="33329-176">String collection</span></span>|<span data-ttu-id="33329-177">Представляет эти [Сотрудники](bookingstaffmember.md) , предоставляющих этой службы.</span><span class="sxs-lookup"><span data-stu-id="33329-177">Represents those [staff members](bookingstaffmember.md) who provide this service.</span></span> |

## <a name="relationships"></a><span data-ttu-id="33329-178">Отношения</span><span class="sxs-lookup"><span data-stu-id="33329-178">Relationships</span></span>
<span data-ttu-id="33329-179">Нет</span><span class="sxs-lookup"><span data-stu-id="33329-179">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="33329-180">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="33329-180">JSON representation</span></span>

<span data-ttu-id="33329-181">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="33329-181">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingService"
}-->

```json
{
  "defaultDuration": "String (timestamp)",
  "defaultLocation": {"@odata.type": "microsoft.graph.location"},
  "defaultPrice": 1024,
  "defaultPriceType": "string",
  "defaultReminders": [{"@odata.type": "microsoft.graph.bookingReminder"}],
  "description": "String",
  "displayName": "String",
  "emailAddress": "String",
  "id": "String (identifier)",
  "isHiddenFromCustomers": true,
  "notes": "String",
  "postBuffer": "String (timestamp)",
  "preBuffer": "String (timestamp)",
  "schedulingPolicy": {"@odata.type": "microsoft.graph.bookingSchedulingPolicy"},
  "staffMemberIds": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingService resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingservice.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
