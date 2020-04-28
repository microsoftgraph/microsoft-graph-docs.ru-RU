---
title: Тип ресурса Букингсервице
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 53c5bc6be0953c68dc431be04b17f582715582c0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43448369"
---
# <a name="bookingservice-resource-type"></a><span data-ttu-id="093cf-104">Тип ресурса Букингсервице</span><span class="sxs-lookup"><span data-stu-id="093cf-104">bookingService resource type</span></span>

<span data-ttu-id="093cf-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="093cf-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="093cf-106">Представляет сведения о конкретной службе, предоставляемой [букингбусинесс](bookingbusiness.md), такие как имя службы, Цена и сотрудники, которые обычно предоставляют такую службу.</span><span class="sxs-lookup"><span data-stu-id="093cf-106">Represents information about a particular service provided by a [bookingBusiness](bookingbusiness.md), such as the service name, price, and the staff that usually provides such service.</span></span>

## <a name="methods"></a><span data-ttu-id="093cf-107">Методы</span><span class="sxs-lookup"><span data-stu-id="093cf-107">Methods</span></span>

| <span data-ttu-id="093cf-108">Метод</span><span class="sxs-lookup"><span data-stu-id="093cf-108">Method</span></span>           | <span data-ttu-id="093cf-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="093cf-109">Return Type</span></span>    |<span data-ttu-id="093cf-110">Описание</span><span class="sxs-lookup"><span data-stu-id="093cf-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="093cf-111">Список служб</span><span class="sxs-lookup"><span data-stu-id="093cf-111">List services</span></span>](../api/bookingbusiness-list-services.md) | <span data-ttu-id="093cf-112">Коллекция [букингсервице](bookingservice.md)</span><span class="sxs-lookup"><span data-stu-id="093cf-112">[bookingService](bookingservice.md) collection</span></span> | <span data-ttu-id="093cf-113">Получение списка объектов **букингсервице** в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="093cf-113">Get a list of **bookingService** objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="093cf-114">Создание Букингсервице</span><span class="sxs-lookup"><span data-stu-id="093cf-114">Create bookingService</span></span>](../api/bookingbusiness-post-services.md) | [<span data-ttu-id="093cf-115">bookingService</span><span class="sxs-lookup"><span data-stu-id="093cf-115">bookingService</span></span>](bookingservice.md) | <span data-ttu-id="093cf-116">Создайте объект **букингсервице** для указанного [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="093cf-116">Create a **bookingService** for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="093cf-117">Получение Букингсервице</span><span class="sxs-lookup"><span data-stu-id="093cf-117">Get bookingService</span></span>](../api/bookingservice-get.md) | [<span data-ttu-id="093cf-118">bookingService</span><span class="sxs-lookup"><span data-stu-id="093cf-118">bookingService</span></span>](bookingservice.md) |<span data-ttu-id="093cf-119">Получение свойств и связей объекта **букингсервице** в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="093cf-119">Get the properties and relationships of a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|<span data-ttu-id="093cf-120">[обновление](../api/bookingservice-update.md).</span><span class="sxs-lookup"><span data-stu-id="093cf-120">[Update](../api/bookingservice-update.md)</span></span> | [<span data-ttu-id="093cf-121">bookingService</span><span class="sxs-lookup"><span data-stu-id="093cf-121">bookingService</span></span>](bookingservice.md)    |<span data-ttu-id="093cf-122">Обновление объекта **букингсервице** в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="093cf-122">Update a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|<span data-ttu-id="093cf-123">[удаление](../api/bookingservice-delete.md);</span><span class="sxs-lookup"><span data-stu-id="093cf-123">[Delete](../api/bookingservice-delete.md)</span></span> | <span data-ttu-id="093cf-124">Нет</span><span class="sxs-lookup"><span data-stu-id="093cf-124">None</span></span> |<span data-ttu-id="093cf-125">Удаление объекта **букингсервице** в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="093cf-125">Delete a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |

## <a name="properties"></a><span data-ttu-id="093cf-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="093cf-126">Properties</span></span>
| <span data-ttu-id="093cf-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="093cf-127">Property</span></span>     | <span data-ttu-id="093cf-128">Тип</span><span class="sxs-lookup"><span data-stu-id="093cf-128">Type</span></span>   |<span data-ttu-id="093cf-129">Описание</span><span class="sxs-lookup"><span data-stu-id="093cf-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="093cf-130">дефаултдуратион</span><span class="sxs-lookup"><span data-stu-id="093cf-130">defaultDuration</span></span>|<span data-ttu-id="093cf-131">Длительность</span><span class="sxs-lookup"><span data-stu-id="093cf-131">Duration</span></span>|<span data-ttu-id="093cf-132">Длина службы по умолчанию, представленная в виде числа дней, часов, минут и секунд.</span><span class="sxs-lookup"><span data-stu-id="093cf-132">The default length of the service, represented in numbers of days, hours, minutes, and seconds.</span></span> <span data-ttu-id="093cf-133">Например, P11D23H59M 59.999999999999 S.</span><span class="sxs-lookup"><span data-stu-id="093cf-133">For example, P11D23H59M59.999999999999S.</span></span> |
|<span data-ttu-id="093cf-134">defaultLocation</span><span class="sxs-lookup"><span data-stu-id="093cf-134">defaultLocation</span></span>|[<span data-ttu-id="093cf-135">location</span><span class="sxs-lookup"><span data-stu-id="093cf-135">location</span></span>](location.md)|<span data-ttu-id="093cf-136">Физическое расположение службы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="093cf-136">The default physical location for the service.</span></span>|
|<span data-ttu-id="093cf-137">дефаултприце</span><span class="sxs-lookup"><span data-stu-id="093cf-137">defaultPrice</span></span>|<span data-ttu-id="093cf-138">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="093cf-138">Double</span></span>|<span data-ttu-id="093cf-139">Денежная Цена по умолчанию для службы.</span><span class="sxs-lookup"><span data-stu-id="093cf-139">The default monetary price for the service.</span></span>|
|<span data-ttu-id="093cf-140">дефаултприцетипе</span><span class="sxs-lookup"><span data-stu-id="093cf-140">defaultPriceType</span></span>|<span data-ttu-id="093cf-141">string</span><span class="sxs-lookup"><span data-stu-id="093cf-141">string</span></span>|<span data-ttu-id="093cf-142">Способ оплаты службы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="093cf-142">The default way the service is charged.</span></span> <span data-ttu-id="093cf-143">Возможные значения: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="093cf-143">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="093cf-144">дефаултреминдерс</span><span class="sxs-lookup"><span data-stu-id="093cf-144">defaultReminders</span></span>|<span data-ttu-id="093cf-145">Коллекция [букингреминдер](bookingreminder.md)</span><span class="sxs-lookup"><span data-stu-id="093cf-145">[bookingReminder](bookingreminder.md) collection</span></span>|<span data-ttu-id="093cf-146">Набор напоминаний по умолчанию для встречи этой службы.</span><span class="sxs-lookup"><span data-stu-id="093cf-146">The default set of reminders for an appointment of this service.</span></span> <span data-ttu-id="093cf-147">Значение этого свойства доступно только при чтении этого **букингсервице** с помощью идентификатора.</span><span class="sxs-lookup"><span data-stu-id="093cf-147">The value of this property is available only when reading this **bookingService** by its ID.</span></span>|
|<span data-ttu-id="093cf-148">description</span><span class="sxs-lookup"><span data-stu-id="093cf-148">description</span></span>|<span data-ttu-id="093cf-149">String</span><span class="sxs-lookup"><span data-stu-id="093cf-149">String</span></span>|<span data-ttu-id="093cf-150">Текстовое описание службы.</span><span class="sxs-lookup"><span data-stu-id="093cf-150">A text description for the service.</span></span>|
|<span data-ttu-id="093cf-151">displayName</span><span class="sxs-lookup"><span data-stu-id="093cf-151">displayName</span></span>|<span data-ttu-id="093cf-152">Строка</span><span class="sxs-lookup"><span data-stu-id="093cf-152">String</span></span>|<span data-ttu-id="093cf-153">Имя службы.</span><span class="sxs-lookup"><span data-stu-id="093cf-153">A service name.</span></span>|
|<span data-ttu-id="093cf-154">emailAddress</span><span class="sxs-lookup"><span data-stu-id="093cf-154">emailAddress</span></span>|<span data-ttu-id="093cf-155">String</span><span class="sxs-lookup"><span data-stu-id="093cf-155">String</span></span>|<span data-ttu-id="093cf-156">Адрес электронной почты</span><span class="sxs-lookup"><span data-stu-id="093cf-156">An email address</span></span>|
|<span data-ttu-id="093cf-157">id</span><span class="sxs-lookup"><span data-stu-id="093cf-157">id</span></span>|<span data-ttu-id="093cf-158">Строка</span><span class="sxs-lookup"><span data-stu-id="093cf-158">String</span></span>|<span data-ttu-id="093cf-159">Идентификатор этой службы в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="093cf-159">The ID of that service, in a GUID format.</span></span> <span data-ttu-id="093cf-160">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="093cf-160">Read-only.</span></span>|
|<span data-ttu-id="093cf-161">ишидденфромкустомерс</span><span class="sxs-lookup"><span data-stu-id="093cf-161">isHiddenFromCustomers</span></span>|<span data-ttu-id="093cf-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="093cf-162">Boolean</span></span>|<span data-ttu-id="093cf-163">Значение true означает, что эта служба недоступна клиентам для резервирования.</span><span class="sxs-lookup"><span data-stu-id="093cf-163">True means this service is not available to customers for booking.</span></span>|
|<span data-ttu-id="093cf-164">notes</span><span class="sxs-lookup"><span data-stu-id="093cf-164">notes</span></span>|<span data-ttu-id="093cf-165">String</span><span class="sxs-lookup"><span data-stu-id="093cf-165">String</span></span>|<span data-ttu-id="093cf-166">Дополнительные сведения об этой службе.</span><span class="sxs-lookup"><span data-stu-id="093cf-166">Additional information about this service.</span></span>|
|<span data-ttu-id="093cf-167">Буфер буфера</span><span class="sxs-lookup"><span data-stu-id="093cf-167">postBuffer</span></span>|<span data-ttu-id="093cf-168">Длительность</span><span class="sxs-lookup"><span data-stu-id="093cf-168">Duration</span></span>|<span data-ttu-id="093cf-169">Время, в течение которого помещается в буфер после встречи для этой службы и до того, как может быть зарезервирована Следующая встреча покупателя.</span><span class="sxs-lookup"><span data-stu-id="093cf-169">The time to buffer after an appointment for this service ends, and before the next customer appointment can be booked.</span></span>|
|<span data-ttu-id="093cf-170">пребуфер</span><span class="sxs-lookup"><span data-stu-id="093cf-170">preBuffer</span></span>|<span data-ttu-id="093cf-171">Длительность</span><span class="sxs-lookup"><span data-stu-id="093cf-171">Duration</span></span>|<span data-ttu-id="093cf-172">Время, в течение которого будет помещено в буфер, прежде чем можно будет запустить встречу для этой службы.</span><span class="sxs-lookup"><span data-stu-id="093cf-172">The time to buffer before an appointment for this service can start.</span></span>|
|<span data-ttu-id="093cf-173">счедулингполици</span><span class="sxs-lookup"><span data-stu-id="093cf-173">schedulingPolicy</span></span>|[<span data-ttu-id="093cf-174">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="093cf-174">bookingSchedulingPolicy</span></span>](bookingschedulingpolicy.md)|<span data-ttu-id="093cf-175">Набор политик, определяющих, как должны создаваться встречи для этого типа службы и управлять ими.</span><span class="sxs-lookup"><span data-stu-id="093cf-175">The set of policies that determine how appointments for this type of service should be created and managed.</span></span>|
|<span data-ttu-id="093cf-176">стаффмемберидс</span><span class="sxs-lookup"><span data-stu-id="093cf-176">staffMemberIds</span></span>|<span data-ttu-id="093cf-177">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="093cf-177">String collection</span></span>|<span data-ttu-id="093cf-178">Представляет [сотрудников](bookingstaffmember.md) , которые предоставляют эту службу.</span><span class="sxs-lookup"><span data-stu-id="093cf-178">Represents those [staff members](bookingstaffmember.md) who provide this service.</span></span> |

## <a name="relationships"></a><span data-ttu-id="093cf-179">Связи</span><span class="sxs-lookup"><span data-stu-id="093cf-179">Relationships</span></span>
<span data-ttu-id="093cf-180">Нет</span><span class="sxs-lookup"><span data-stu-id="093cf-180">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="093cf-181">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="093cf-181">JSON representation</span></span>

<span data-ttu-id="093cf-182">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="093cf-182">The following is a JSON representation of the resource.</span></span>

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
