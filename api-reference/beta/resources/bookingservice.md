---
title: Тип ресурса Букингсервице
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: c6cf62320a6cfd8e96455e95e1d17c0621d261f8
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328320"
---
# <a name="bookingservice-resource-type"></a><span data-ttu-id="a2a72-104">Тип ресурса Букингсервице</span><span class="sxs-lookup"><span data-stu-id="a2a72-104">bookingService resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="a2a72-105">Представляет сведения о конкретной службе, предоставляемой [букингбусинесс](bookingbusiness.md), такие как имя службы, Цена и сотрудники, которые обычно предоставляют такую службу.</span><span class="sxs-lookup"><span data-stu-id="a2a72-105">Represents information about a particular service provided by a [bookingBusiness](bookingbusiness.md), such as the service name, price, and the staff that usually provides such service.</span></span>

## <a name="methods"></a><span data-ttu-id="a2a72-106">Методы</span><span class="sxs-lookup"><span data-stu-id="a2a72-106">Methods</span></span>

| <span data-ttu-id="a2a72-107">Метод</span><span class="sxs-lookup"><span data-stu-id="a2a72-107">Method</span></span>           | <span data-ttu-id="a2a72-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a2a72-108">Return Type</span></span>    |<span data-ttu-id="a2a72-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a2a72-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a2a72-110">Список служб</span><span class="sxs-lookup"><span data-stu-id="a2a72-110">List services</span></span>](../api/bookingbusiness-list-services.md) | <span data-ttu-id="a2a72-111">Коллекция [букингсервице](bookingservice.md)</span><span class="sxs-lookup"><span data-stu-id="a2a72-111">[bookingService](bookingservice.md) collection</span></span> | <span data-ttu-id="a2a72-112">Получение списка объектов **букингсервице** в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="a2a72-112">Get a list of **bookingService** objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="a2a72-113">Создание Букингсервице</span><span class="sxs-lookup"><span data-stu-id="a2a72-113">Create bookingService</span></span>](../api/bookingbusiness-post-services.md) | [<span data-ttu-id="a2a72-114">bookingService</span><span class="sxs-lookup"><span data-stu-id="a2a72-114">bookingService</span></span>](bookingservice.md) | <span data-ttu-id="a2a72-115">Создайте объект **букингсервице** для указанного [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="a2a72-115">Create a **bookingService** for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="a2a72-116">Получение Букингсервице</span><span class="sxs-lookup"><span data-stu-id="a2a72-116">Get bookingService</span></span>](../api/bookingservice-get.md) | [<span data-ttu-id="a2a72-117">bookingService</span><span class="sxs-lookup"><span data-stu-id="a2a72-117">bookingService</span></span>](bookingservice.md) |<span data-ttu-id="a2a72-118">Получение свойств и связей объекта **букингсервице** в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="a2a72-118">Get the properties and relationships of a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="a2a72-119">Update</span><span class="sxs-lookup"><span data-stu-id="a2a72-119">Update</span></span>](../api/bookingservice-update.md) | [<span data-ttu-id="a2a72-120">bookingService</span><span class="sxs-lookup"><span data-stu-id="a2a72-120">bookingService</span></span>](bookingservice.md)    |<span data-ttu-id="a2a72-121">Обновление объекта **букингсервице** в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="a2a72-121">Update a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="a2a72-122">Delete</span><span class="sxs-lookup"><span data-stu-id="a2a72-122">Delete</span></span>](../api/bookingservice-delete.md) | <span data-ttu-id="a2a72-123">Нет</span><span class="sxs-lookup"><span data-stu-id="a2a72-123">None</span></span> |<span data-ttu-id="a2a72-124">Удаление объекта **букингсервице** в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="a2a72-124">Delete a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |

## <a name="properties"></a><span data-ttu-id="a2a72-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="a2a72-125">Properties</span></span>
| <span data-ttu-id="a2a72-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="a2a72-126">Property</span></span>     | <span data-ttu-id="a2a72-127">Тип</span><span class="sxs-lookup"><span data-stu-id="a2a72-127">Type</span></span>   |<span data-ttu-id="a2a72-128">Описание</span><span class="sxs-lookup"><span data-stu-id="a2a72-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a2a72-129">Дефаултдуратион</span><span class="sxs-lookup"><span data-stu-id="a2a72-129">defaultDuration</span></span>|<span data-ttu-id="a2a72-130">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="a2a72-130">Duration</span></span>|<span data-ttu-id="a2a72-131">Длина службы по умолчанию, представленная в виде числа дней, часов, минут и секунд.</span><span class="sxs-lookup"><span data-stu-id="a2a72-131">The default length of the service, represented in numbers of days, hours, minutes, and seconds.</span></span> <span data-ttu-id="a2a72-132">Например, P11D23H59M 59.999999999999 S.</span><span class="sxs-lookup"><span data-stu-id="a2a72-132">For example, P11D23H59M59.999999999999S.</span></span> |
|<span data-ttu-id="a2a72-133">defaultLocation</span><span class="sxs-lookup"><span data-stu-id="a2a72-133">defaultLocation</span></span>|[<span data-ttu-id="a2a72-134">location</span><span class="sxs-lookup"><span data-stu-id="a2a72-134">location</span></span>](location.md)|<span data-ttu-id="a2a72-135">Физическое расположение службы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a2a72-135">The default physical location for the service.</span></span>|
|<span data-ttu-id="a2a72-136">Дефаултприце</span><span class="sxs-lookup"><span data-stu-id="a2a72-136">defaultPrice</span></span>|<span data-ttu-id="a2a72-137">Двойное</span><span class="sxs-lookup"><span data-stu-id="a2a72-137">Double</span></span>|<span data-ttu-id="a2a72-138">Денежная Цена по умолчанию для службы.</span><span class="sxs-lookup"><span data-stu-id="a2a72-138">The default monetary price for the service.</span></span>|
|<span data-ttu-id="a2a72-139">Дефаултприцетипе</span><span class="sxs-lookup"><span data-stu-id="a2a72-139">defaultPriceType</span></span>|<span data-ttu-id="a2a72-140">string</span><span class="sxs-lookup"><span data-stu-id="a2a72-140">string</span></span>|<span data-ttu-id="a2a72-141">Способ оплаты службы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a2a72-141">The default way the service is charged.</span></span> <span data-ttu-id="a2a72-142">Возможные значения: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="a2a72-142">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="a2a72-143">Дефаултреминдерс</span><span class="sxs-lookup"><span data-stu-id="a2a72-143">defaultReminders</span></span>|<span data-ttu-id="a2a72-144">Коллекция [букингреминдер](bookingreminder.md)</span><span class="sxs-lookup"><span data-stu-id="a2a72-144">[bookingReminder](bookingreminder.md) collection</span></span>|<span data-ttu-id="a2a72-145">Набор напоминаний по умолчанию для встречи этой службы.</span><span class="sxs-lookup"><span data-stu-id="a2a72-145">The default set of reminders for an appointment of this service.</span></span> <span data-ttu-id="a2a72-146">Значение этого свойства доступно только при чтении этого **букингсервице** с помощью идентификатора.</span><span class="sxs-lookup"><span data-stu-id="a2a72-146">The value of this property is available only when reading this **bookingService** by its ID.</span></span>|
|<span data-ttu-id="a2a72-147">description</span><span class="sxs-lookup"><span data-stu-id="a2a72-147">description</span></span>|<span data-ttu-id="a2a72-148">String</span><span class="sxs-lookup"><span data-stu-id="a2a72-148">String</span></span>|<span data-ttu-id="a2a72-149">Текстовое описание службы.</span><span class="sxs-lookup"><span data-stu-id="a2a72-149">A text description for the service.</span></span>|
|<span data-ttu-id="a2a72-150">displayName</span><span class="sxs-lookup"><span data-stu-id="a2a72-150">displayName</span></span>|<span data-ttu-id="a2a72-151">Строка</span><span class="sxs-lookup"><span data-stu-id="a2a72-151">String</span></span>|<span data-ttu-id="a2a72-152">Имя службы.</span><span class="sxs-lookup"><span data-stu-id="a2a72-152">A service name.</span></span>|
|<span data-ttu-id="a2a72-153">emailAddress</span><span class="sxs-lookup"><span data-stu-id="a2a72-153">emailAddress</span></span>|<span data-ttu-id="a2a72-154">String</span><span class="sxs-lookup"><span data-stu-id="a2a72-154">String</span></span>|<span data-ttu-id="a2a72-155">Адрес электронной почты</span><span class="sxs-lookup"><span data-stu-id="a2a72-155">An email address</span></span>|
|<span data-ttu-id="a2a72-156">id</span><span class="sxs-lookup"><span data-stu-id="a2a72-156">id</span></span>|<span data-ttu-id="a2a72-157">Строка</span><span class="sxs-lookup"><span data-stu-id="a2a72-157">String</span></span>|<span data-ttu-id="a2a72-158">Идентификатор этой службы в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="a2a72-158">The ID of that service, in a GUID format.</span></span> <span data-ttu-id="a2a72-159">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a2a72-159">Read-only.</span></span>|
|<span data-ttu-id="a2a72-160">Ишидденфромкустомерс</span><span class="sxs-lookup"><span data-stu-id="a2a72-160">isHiddenFromCustomers</span></span>|<span data-ttu-id="a2a72-161">Логический</span><span class="sxs-lookup"><span data-stu-id="a2a72-161">Boolean</span></span>|<span data-ttu-id="a2a72-162">Значение true означает, что эта служба недоступна клиентам для резервирования.</span><span class="sxs-lookup"><span data-stu-id="a2a72-162">True means this service is not available to customers for booking.</span></span>|
|<span data-ttu-id="a2a72-163">notes</span><span class="sxs-lookup"><span data-stu-id="a2a72-163">notes</span></span>|<span data-ttu-id="a2a72-164">String</span><span class="sxs-lookup"><span data-stu-id="a2a72-164">String</span></span>|<span data-ttu-id="a2a72-165">Дополнительные сведения об этой службе.</span><span class="sxs-lookup"><span data-stu-id="a2a72-165">Additional information about this service.</span></span>|
|<span data-ttu-id="a2a72-166">Буфер буфера</span><span class="sxs-lookup"><span data-stu-id="a2a72-166">postBuffer</span></span>|<span data-ttu-id="a2a72-167">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="a2a72-167">Duration</span></span>|<span data-ttu-id="a2a72-168">Время, в течение которого помещается в буфер после встречи для этой службы и до того, как может быть зарезервирована Следующая встреча покупателя.</span><span class="sxs-lookup"><span data-stu-id="a2a72-168">The time to buffer after an appointment for this service ends, and before the next customer appointment can be booked.</span></span>|
|<span data-ttu-id="a2a72-169">преБуфер</span><span class="sxs-lookup"><span data-stu-id="a2a72-169">preBuffer</span></span>|<span data-ttu-id="a2a72-170">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="a2a72-170">Duration</span></span>|<span data-ttu-id="a2a72-171">Время, в течение которого будет помещено в буфер, прежде чем можно будет запустить встречу для этой службы.</span><span class="sxs-lookup"><span data-stu-id="a2a72-171">The time to buffer before an appointment for this service can start.</span></span>|
|<span data-ttu-id="a2a72-172">Счедулингполици</span><span class="sxs-lookup"><span data-stu-id="a2a72-172">schedulingPolicy</span></span>|[<span data-ttu-id="a2a72-173">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="a2a72-173">bookingSchedulingPolicy</span></span>](bookingschedulingpolicy.md)|<span data-ttu-id="a2a72-174">Набор политик, определяющих, как должны создаваться встречи для этого типа службы и управлять ими.</span><span class="sxs-lookup"><span data-stu-id="a2a72-174">The set of policies that determine how appointments for this type of service should be created and managed.</span></span>|
|<span data-ttu-id="a2a72-175">Стаффмемберидс</span><span class="sxs-lookup"><span data-stu-id="a2a72-175">staffMemberIds</span></span>|<span data-ttu-id="a2a72-176">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a2a72-176">String collection</span></span>|<span data-ttu-id="a2a72-177">Представляет [сотрудников](bookingstaffmember.md) , которые предоставляют эту службу.</span><span class="sxs-lookup"><span data-stu-id="a2a72-177">Represents those [staff members](bookingstaffmember.md) who provide this service.</span></span> |

## <a name="relationships"></a><span data-ttu-id="a2a72-178">Отношения</span><span class="sxs-lookup"><span data-stu-id="a2a72-178">Relationships</span></span>
<span data-ttu-id="a2a72-179">Нет</span><span class="sxs-lookup"><span data-stu-id="a2a72-179">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a2a72-180">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a2a72-180">JSON representation</span></span>

<span data-ttu-id="a2a72-181">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a2a72-181">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
