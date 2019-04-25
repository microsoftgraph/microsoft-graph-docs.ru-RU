---
title: Тип ресурса Букингсервице
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 35e439888b39c81451242f01d2aaae89b65ad8ee
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535499"
---
# <a name="bookingservice-resource-type"></a><span data-ttu-id="062b7-104">Тип ресурса Букингсервице</span><span class="sxs-lookup"><span data-stu-id="062b7-104">bookingService resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="062b7-105">Представляет сведения о конкретной службе, предоставляемой [букингбусинесс](bookingbusiness.md), такие как имя службы, Цена и сотрудники, которые обычно предоставляют такую службу.</span><span class="sxs-lookup"><span data-stu-id="062b7-105">Represents information about a particular service provided by a [bookingBusiness](bookingbusiness.md), such as the service name, price, and the staff that usually provides such service.</span></span>

## <a name="methods"></a><span data-ttu-id="062b7-106">Методы</span><span class="sxs-lookup"><span data-stu-id="062b7-106">Methods</span></span>

| <span data-ttu-id="062b7-107">Метод</span><span class="sxs-lookup"><span data-stu-id="062b7-107">Method</span></span>           | <span data-ttu-id="062b7-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="062b7-108">Return Type</span></span>    |<span data-ttu-id="062b7-109">Описание</span><span class="sxs-lookup"><span data-stu-id="062b7-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="062b7-110">Список служб</span><span class="sxs-lookup"><span data-stu-id="062b7-110">List services</span></span>](../api/bookingbusiness-list-services.md) | <span data-ttu-id="062b7-111">Коллекция [букингсервице](bookingservice.md)</span><span class="sxs-lookup"><span data-stu-id="062b7-111">[bookingService](bookingservice.md) collection</span></span> | <span data-ttu-id="062b7-112">Получение списка объектов **букингсервице** в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="062b7-112">Get a list of **bookingService** objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="062b7-113">Создание Букингсервице</span><span class="sxs-lookup"><span data-stu-id="062b7-113">Create bookingService</span></span>](../api/bookingbusiness-post-services.md) | [<span data-ttu-id="062b7-114">bookingService</span><span class="sxs-lookup"><span data-stu-id="062b7-114">bookingService</span></span>](bookingservice.md) | <span data-ttu-id="062b7-115">Создайте объект **букингсервице** для указанного [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="062b7-115">Create a **bookingService** for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="062b7-116">Получение Букингсервице</span><span class="sxs-lookup"><span data-stu-id="062b7-116">Get bookingService</span></span>](../api/bookingservice-get.md) | [<span data-ttu-id="062b7-117">bookingService</span><span class="sxs-lookup"><span data-stu-id="062b7-117">bookingService</span></span>](bookingservice.md) |<span data-ttu-id="062b7-118">Получение свойств и связей объекта **букингсервице** в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="062b7-118">Get the properties and relationships of a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="062b7-119">Обновление</span><span class="sxs-lookup"><span data-stu-id="062b7-119">Update</span></span>](../api/bookingservice-update.md) | [<span data-ttu-id="062b7-120">bookingService</span><span class="sxs-lookup"><span data-stu-id="062b7-120">bookingService</span></span>](bookingservice.md)    |<span data-ttu-id="062b7-121">Обновление объекта **букингсервице** в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="062b7-121">Update a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="062b7-122">Удаление</span><span class="sxs-lookup"><span data-stu-id="062b7-122">Delete</span></span>](../api/bookingservice-delete.md) | <span data-ttu-id="062b7-123">Нет</span><span class="sxs-lookup"><span data-stu-id="062b7-123">None</span></span> |<span data-ttu-id="062b7-124">Удаление объекта **букингсервице** в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="062b7-124">Delete a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |

## <a name="properties"></a><span data-ttu-id="062b7-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="062b7-125">Properties</span></span>
| <span data-ttu-id="062b7-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="062b7-126">Property</span></span>     | <span data-ttu-id="062b7-127">Тип</span><span class="sxs-lookup"><span data-stu-id="062b7-127">Type</span></span>   |<span data-ttu-id="062b7-128">Описание</span><span class="sxs-lookup"><span data-stu-id="062b7-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="062b7-129">Дефаултдуратион</span><span class="sxs-lookup"><span data-stu-id="062b7-129">defaultDuration</span></span>|<span data-ttu-id="062b7-130">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="062b7-130">Duration</span></span>|<span data-ttu-id="062b7-131">Длина службы по умолчанию, представленная в виде числа дней, часов, минут и секунд.</span><span class="sxs-lookup"><span data-stu-id="062b7-131">The default length of the service, represented in numbers of days, hours, minutes, and seconds.</span></span> <span data-ttu-id="062b7-132">Например, P11D23H59M 59.999999999999 S.</span><span class="sxs-lookup"><span data-stu-id="062b7-132">For example, P11D23H59M59.999999999999S.</span></span> |
|<span data-ttu-id="062b7-133">defaultLocation</span><span class="sxs-lookup"><span data-stu-id="062b7-133">defaultLocation</span></span>|[<span data-ttu-id="062b7-134">location</span><span class="sxs-lookup"><span data-stu-id="062b7-134">location</span></span>](location.md)|<span data-ttu-id="062b7-135">Физическое расположение службы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="062b7-135">The default physical location for the service.</span></span>|
|<span data-ttu-id="062b7-136">Дефаултприце</span><span class="sxs-lookup"><span data-stu-id="062b7-136">defaultPrice</span></span>|<span data-ttu-id="062b7-137">Двойное</span><span class="sxs-lookup"><span data-stu-id="062b7-137">Double</span></span>|<span data-ttu-id="062b7-138">Денежная Цена по умолчанию для службы.</span><span class="sxs-lookup"><span data-stu-id="062b7-138">The default monetary price for the service.</span></span>|
|<span data-ttu-id="062b7-139">Дефаултприцетипе</span><span class="sxs-lookup"><span data-stu-id="062b7-139">defaultPriceType</span></span>|<span data-ttu-id="062b7-140">string</span><span class="sxs-lookup"><span data-stu-id="062b7-140">string</span></span>|<span data-ttu-id="062b7-141">Способ оплаты службы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="062b7-141">The default way the service is charged.</span></span> <span data-ttu-id="062b7-142">Возможные значения: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="062b7-142">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="062b7-143">Дефаултреминдерс</span><span class="sxs-lookup"><span data-stu-id="062b7-143">defaultReminders</span></span>|<span data-ttu-id="062b7-144">Коллекция [букингреминдер](bookingreminder.md)</span><span class="sxs-lookup"><span data-stu-id="062b7-144">[bookingReminder](bookingreminder.md) collection</span></span>|<span data-ttu-id="062b7-145">Набор напоминаний по умолчанию для встречи этой службы.</span><span class="sxs-lookup"><span data-stu-id="062b7-145">The default set of reminders for an appointment of this service.</span></span> <span data-ttu-id="062b7-146">Значение этого свойства доступно только при чтении этого **букингсервице** с помощью идентификатора.</span><span class="sxs-lookup"><span data-stu-id="062b7-146">The value of this property is available only when reading this **bookingService** by its ID.</span></span>|
|<span data-ttu-id="062b7-147">description</span><span class="sxs-lookup"><span data-stu-id="062b7-147">description</span></span>|<span data-ttu-id="062b7-148">String</span><span class="sxs-lookup"><span data-stu-id="062b7-148">String</span></span>|<span data-ttu-id="062b7-149">Текстовое описание службы.</span><span class="sxs-lookup"><span data-stu-id="062b7-149">A text description for the service.</span></span>|
|<span data-ttu-id="062b7-150">displayName</span><span class="sxs-lookup"><span data-stu-id="062b7-150">displayName</span></span>|<span data-ttu-id="062b7-151">Строка</span><span class="sxs-lookup"><span data-stu-id="062b7-151">String</span></span>|<span data-ttu-id="062b7-152">Имя службы.</span><span class="sxs-lookup"><span data-stu-id="062b7-152">A service name.</span></span>|
|<span data-ttu-id="062b7-153">emailAddress</span><span class="sxs-lookup"><span data-stu-id="062b7-153">emailAddress</span></span>|<span data-ttu-id="062b7-154">String</span><span class="sxs-lookup"><span data-stu-id="062b7-154">String</span></span>|<span data-ttu-id="062b7-155">Адрес электронной почты</span><span class="sxs-lookup"><span data-stu-id="062b7-155">An email address</span></span>|
|<span data-ttu-id="062b7-156">id</span><span class="sxs-lookup"><span data-stu-id="062b7-156">id</span></span>|<span data-ttu-id="062b7-157">Строка</span><span class="sxs-lookup"><span data-stu-id="062b7-157">String</span></span>|<span data-ttu-id="062b7-158">Идентификатор этой службы в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="062b7-158">The ID of that service, in a GUID format.</span></span> <span data-ttu-id="062b7-159">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="062b7-159">Read-only.</span></span>|
|<span data-ttu-id="062b7-160">Ишидденфромкустомерс</span><span class="sxs-lookup"><span data-stu-id="062b7-160">isHiddenFromCustomers</span></span>|<span data-ttu-id="062b7-161">Логический</span><span class="sxs-lookup"><span data-stu-id="062b7-161">Boolean</span></span>|<span data-ttu-id="062b7-162">Значение true означает, что эта служба недоступна клиентам для резервирования.</span><span class="sxs-lookup"><span data-stu-id="062b7-162">True means this service is not available to customers for booking.</span></span>|
|<span data-ttu-id="062b7-163">notes</span><span class="sxs-lookup"><span data-stu-id="062b7-163">notes</span></span>|<span data-ttu-id="062b7-164">String</span><span class="sxs-lookup"><span data-stu-id="062b7-164">String</span></span>|<span data-ttu-id="062b7-165">Дополнительные сведения об этой службе.</span><span class="sxs-lookup"><span data-stu-id="062b7-165">Additional information about this service.</span></span>|
|<span data-ttu-id="062b7-166">Буфер буфера</span><span class="sxs-lookup"><span data-stu-id="062b7-166">postBuffer</span></span>|<span data-ttu-id="062b7-167">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="062b7-167">Duration</span></span>|<span data-ttu-id="062b7-168">Время, в течение которого помещается в буфер после встречи для этой службы и до того, как может быть зарезервирована Следующая встреча покупателя.</span><span class="sxs-lookup"><span data-stu-id="062b7-168">The time to buffer after an appointment for this service ends, and before the next customer appointment can be booked.</span></span>|
|<span data-ttu-id="062b7-169">преБуфер</span><span class="sxs-lookup"><span data-stu-id="062b7-169">preBuffer</span></span>|<span data-ttu-id="062b7-170">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="062b7-170">Duration</span></span>|<span data-ttu-id="062b7-171">Время, в течение которого будет помещено в буфер, прежде чем можно будет запустить встречу для этой службы.</span><span class="sxs-lookup"><span data-stu-id="062b7-171">The time to buffer before an appointment for this service can start.</span></span>|
|<span data-ttu-id="062b7-172">Счедулингполици</span><span class="sxs-lookup"><span data-stu-id="062b7-172">schedulingPolicy</span></span>|[<span data-ttu-id="062b7-173">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="062b7-173">bookingSchedulingPolicy</span></span>](bookingschedulingpolicy.md)|<span data-ttu-id="062b7-174">Набор политик, определяющих, как должны создаваться встречи для этого типа службы и управлять ими.</span><span class="sxs-lookup"><span data-stu-id="062b7-174">The set of policies that determine how appointments for this type of service should be created and managed.</span></span>|
|<span data-ttu-id="062b7-175">Стаффмемберидс</span><span class="sxs-lookup"><span data-stu-id="062b7-175">staffMemberIds</span></span>|<span data-ttu-id="062b7-176">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="062b7-176">String collection</span></span>|<span data-ttu-id="062b7-177">Представляет [сотрудников](bookingstaffmember.md) , которые предоставляют эту службу.</span><span class="sxs-lookup"><span data-stu-id="062b7-177">Represents those [staff members](bookingstaffmember.md) who provide this service.</span></span> |

## <a name="relationships"></a><span data-ttu-id="062b7-178">Отношения</span><span class="sxs-lookup"><span data-stu-id="062b7-178">Relationships</span></span>
<span data-ttu-id="062b7-179">Нет</span><span class="sxs-lookup"><span data-stu-id="062b7-179">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="062b7-180">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="062b7-180">JSON representation</span></span>

<span data-ttu-id="062b7-181">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="062b7-181">The following is a JSON representation of the resource.</span></span>

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
