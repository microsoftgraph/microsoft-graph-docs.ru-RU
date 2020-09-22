---
title: Тип ресурса Букингсервице
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 37a1e6adb6a4769601d5f9806d1e3b262fe2879f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071747"
---
# <a name="bookingservice-resource-type"></a><span data-ttu-id="d9bde-104">Тип ресурса Букингсервице</span><span class="sxs-lookup"><span data-stu-id="d9bde-104">bookingService resource type</span></span>

<span data-ttu-id="d9bde-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9bde-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="d9bde-106">Представляет сведения о конкретной службе, предоставляемой [букингбусинесс](bookingbusiness.md), такие как имя службы, Цена и сотрудники, которые обычно предоставляют такую службу.</span><span class="sxs-lookup"><span data-stu-id="d9bde-106">Represents information about a particular service provided by a [bookingBusiness](bookingbusiness.md), such as the service name, price, and the staff that usually provides such service.</span></span>

## <a name="methods"></a><span data-ttu-id="d9bde-107">Методы</span><span class="sxs-lookup"><span data-stu-id="d9bde-107">Methods</span></span>

| <span data-ttu-id="d9bde-108">Метод</span><span class="sxs-lookup"><span data-stu-id="d9bde-108">Method</span></span>           | <span data-ttu-id="d9bde-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d9bde-109">Return Type</span></span>    |<span data-ttu-id="d9bde-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d9bde-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d9bde-111">Список служб</span><span class="sxs-lookup"><span data-stu-id="d9bde-111">List services</span></span>](../api/bookingbusiness-list-services.md) | <span data-ttu-id="d9bde-112">Коллекция [букингсервице](bookingservice.md)</span><span class="sxs-lookup"><span data-stu-id="d9bde-112">[bookingService](bookingservice.md) collection</span></span> | <span data-ttu-id="d9bde-113">Получение списка объектов **букингсервице** в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="d9bde-113">Get a list of **bookingService** objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="d9bde-114">Создание Букингсервице</span><span class="sxs-lookup"><span data-stu-id="d9bde-114">Create bookingService</span></span>](../api/bookingbusiness-post-services.md) | [<span data-ttu-id="d9bde-115">bookingService</span><span class="sxs-lookup"><span data-stu-id="d9bde-115">bookingService</span></span>](bookingservice.md) | <span data-ttu-id="d9bde-116">Создайте объект **букингсервице** для указанного [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="d9bde-116">Create a **bookingService** for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="d9bde-117">Получение Букингсервице</span><span class="sxs-lookup"><span data-stu-id="d9bde-117">Get bookingService</span></span>](../api/bookingservice-get.md) | [<span data-ttu-id="d9bde-118">bookingService</span><span class="sxs-lookup"><span data-stu-id="d9bde-118">bookingService</span></span>](bookingservice.md) |<span data-ttu-id="d9bde-119">Получение свойств и связей объекта **букингсервице** в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="d9bde-119">Get the properties and relationships of a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="d9bde-120">Обновление</span><span class="sxs-lookup"><span data-stu-id="d9bde-120">Update</span></span>](../api/bookingservice-update.md) | [<span data-ttu-id="d9bde-121">bookingService</span><span class="sxs-lookup"><span data-stu-id="d9bde-121">bookingService</span></span>](bookingservice.md)    |<span data-ttu-id="d9bde-122">Обновление объекта **букингсервице** в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="d9bde-122">Update a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="d9bde-123">Удаление</span><span class="sxs-lookup"><span data-stu-id="d9bde-123">Delete</span></span>](../api/bookingservice-delete.md) | <span data-ttu-id="d9bde-124">Нет</span><span class="sxs-lookup"><span data-stu-id="d9bde-124">None</span></span> |<span data-ttu-id="d9bde-125">Удаление объекта **букингсервице** в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="d9bde-125">Delete a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |

## <a name="properties"></a><span data-ttu-id="d9bde-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="d9bde-126">Properties</span></span>
| <span data-ttu-id="d9bde-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="d9bde-127">Property</span></span>     | <span data-ttu-id="d9bde-128">Тип</span><span class="sxs-lookup"><span data-stu-id="d9bde-128">Type</span></span>   |<span data-ttu-id="d9bde-129">Описание</span><span class="sxs-lookup"><span data-stu-id="d9bde-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d9bde-130">дефаултдуратион</span><span class="sxs-lookup"><span data-stu-id="d9bde-130">defaultDuration</span></span>|<span data-ttu-id="d9bde-131">Длительность</span><span class="sxs-lookup"><span data-stu-id="d9bde-131">Duration</span></span>|<span data-ttu-id="d9bde-132">Длина службы по умолчанию, представленная в виде числа дней, часов, минут и секунд.</span><span class="sxs-lookup"><span data-stu-id="d9bde-132">The default length of the service, represented in numbers of days, hours, minutes, and seconds.</span></span> <span data-ttu-id="d9bde-133">Например, P11D23H59M 59.999999999999 S.</span><span class="sxs-lookup"><span data-stu-id="d9bde-133">For example, P11D23H59M59.999999999999S.</span></span> |
|<span data-ttu-id="d9bde-134">defaultLocation</span><span class="sxs-lookup"><span data-stu-id="d9bde-134">defaultLocation</span></span>|[<span data-ttu-id="d9bde-135">location</span><span class="sxs-lookup"><span data-stu-id="d9bde-135">location</span></span>](location.md)|<span data-ttu-id="d9bde-136">Физическое расположение службы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="d9bde-136">The default physical location for the service.</span></span>|
|<span data-ttu-id="d9bde-137">дефаултприце</span><span class="sxs-lookup"><span data-stu-id="d9bde-137">defaultPrice</span></span>|<span data-ttu-id="d9bde-138">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="d9bde-138">Double</span></span>|<span data-ttu-id="d9bde-139">Денежная Цена по умолчанию для службы.</span><span class="sxs-lookup"><span data-stu-id="d9bde-139">The default monetary price for the service.</span></span>|
|<span data-ttu-id="d9bde-140">дефаултприцетипе</span><span class="sxs-lookup"><span data-stu-id="d9bde-140">defaultPriceType</span></span>|<span data-ttu-id="d9bde-141">string</span><span class="sxs-lookup"><span data-stu-id="d9bde-141">string</span></span>|<span data-ttu-id="d9bde-142">Способ оплаты службы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="d9bde-142">The default way the service is charged.</span></span> <span data-ttu-id="d9bde-143">Возможные значения: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="d9bde-143">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="d9bde-144">дефаултреминдерс</span><span class="sxs-lookup"><span data-stu-id="d9bde-144">defaultReminders</span></span>|<span data-ttu-id="d9bde-145">Коллекция [букингреминдер](bookingreminder.md)</span><span class="sxs-lookup"><span data-stu-id="d9bde-145">[bookingReminder](bookingreminder.md) collection</span></span>|<span data-ttu-id="d9bde-146">Набор напоминаний по умолчанию для встречи этой службы.</span><span class="sxs-lookup"><span data-stu-id="d9bde-146">The default set of reminders for an appointment of this service.</span></span> <span data-ttu-id="d9bde-147">Значение этого свойства доступно только при чтении этого **букингсервице** с помощью идентификатора.</span><span class="sxs-lookup"><span data-stu-id="d9bde-147">The value of this property is available only when reading this **bookingService** by its ID.</span></span>|
|<span data-ttu-id="d9bde-148">description</span><span class="sxs-lookup"><span data-stu-id="d9bde-148">description</span></span>|<span data-ttu-id="d9bde-149">String</span><span class="sxs-lookup"><span data-stu-id="d9bde-149">String</span></span>|<span data-ttu-id="d9bde-150">Текстовое описание службы.</span><span class="sxs-lookup"><span data-stu-id="d9bde-150">A text description for the service.</span></span>|
|<span data-ttu-id="d9bde-151">displayName</span><span class="sxs-lookup"><span data-stu-id="d9bde-151">displayName</span></span>|<span data-ttu-id="d9bde-152">String</span><span class="sxs-lookup"><span data-stu-id="d9bde-152">String</span></span>|<span data-ttu-id="d9bde-153">Имя службы.</span><span class="sxs-lookup"><span data-stu-id="d9bde-153">A service name.</span></span>|
|<span data-ttu-id="d9bde-154">emailAddress</span><span class="sxs-lookup"><span data-stu-id="d9bde-154">emailAddress</span></span>|<span data-ttu-id="d9bde-155">String</span><span class="sxs-lookup"><span data-stu-id="d9bde-155">String</span></span>|<span data-ttu-id="d9bde-156">Адрес электронной почты</span><span class="sxs-lookup"><span data-stu-id="d9bde-156">An email address</span></span>|
|<span data-ttu-id="d9bde-157">id</span><span class="sxs-lookup"><span data-stu-id="d9bde-157">id</span></span>|<span data-ttu-id="d9bde-158">String</span><span class="sxs-lookup"><span data-stu-id="d9bde-158">String</span></span>|<span data-ttu-id="d9bde-159">Идентификатор этой службы в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="d9bde-159">The ID of that service, in a GUID format.</span></span> <span data-ttu-id="d9bde-160">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d9bde-160">Read-only.</span></span>|
|<span data-ttu-id="d9bde-161">ишидденфромкустомерс</span><span class="sxs-lookup"><span data-stu-id="d9bde-161">isHiddenFromCustomers</span></span>|<span data-ttu-id="d9bde-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9bde-162">Boolean</span></span>|<span data-ttu-id="d9bde-163">Значение true означает, что эта служба недоступна клиентам для резервирования.</span><span class="sxs-lookup"><span data-stu-id="d9bde-163">True means this service is not available to customers for booking.</span></span>|
|<span data-ttu-id="d9bde-164">notes</span><span class="sxs-lookup"><span data-stu-id="d9bde-164">notes</span></span>|<span data-ttu-id="d9bde-165">String</span><span class="sxs-lookup"><span data-stu-id="d9bde-165">String</span></span>|<span data-ttu-id="d9bde-166">Дополнительные сведения об этой службе.</span><span class="sxs-lookup"><span data-stu-id="d9bde-166">Additional information about this service.</span></span>|
|<span data-ttu-id="d9bde-167">Буфер буфера</span><span class="sxs-lookup"><span data-stu-id="d9bde-167">postBuffer</span></span>|<span data-ttu-id="d9bde-168">Длительность</span><span class="sxs-lookup"><span data-stu-id="d9bde-168">Duration</span></span>|<span data-ttu-id="d9bde-169">Время, в течение которого помещается в буфер после встречи для этой службы и до того, как может быть зарезервирована Следующая встреча покупателя.</span><span class="sxs-lookup"><span data-stu-id="d9bde-169">The time to buffer after an appointment for this service ends, and before the next customer appointment can be booked.</span></span>|
|<span data-ttu-id="d9bde-170">пребуфер</span><span class="sxs-lookup"><span data-stu-id="d9bde-170">preBuffer</span></span>|<span data-ttu-id="d9bde-171">Длительность</span><span class="sxs-lookup"><span data-stu-id="d9bde-171">Duration</span></span>|<span data-ttu-id="d9bde-172">Время, в течение которого будет помещено в буфер, прежде чем можно будет запустить встречу для этой службы.</span><span class="sxs-lookup"><span data-stu-id="d9bde-172">The time to buffer before an appointment for this service can start.</span></span>|
|<span data-ttu-id="d9bde-173">счедулингполици</span><span class="sxs-lookup"><span data-stu-id="d9bde-173">schedulingPolicy</span></span>|[<span data-ttu-id="d9bde-174">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="d9bde-174">bookingSchedulingPolicy</span></span>](bookingschedulingpolicy.md)|<span data-ttu-id="d9bde-175">Набор политик, определяющих, как должны создаваться встречи для этого типа службы и управлять ими.</span><span class="sxs-lookup"><span data-stu-id="d9bde-175">The set of policies that determine how appointments for this type of service should be created and managed.</span></span>|
|<span data-ttu-id="d9bde-176">стаффмемберидс</span><span class="sxs-lookup"><span data-stu-id="d9bde-176">staffMemberIds</span></span>|<span data-ttu-id="d9bde-177">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d9bde-177">String collection</span></span>|<span data-ttu-id="d9bde-178">Представляет [сотрудников](bookingstaffmember.md) , которые предоставляют эту службу.</span><span class="sxs-lookup"><span data-stu-id="d9bde-178">Represents those [staff members](bookingstaffmember.md) who provide this service.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d9bde-179">Отношения</span><span class="sxs-lookup"><span data-stu-id="d9bde-179">Relationships</span></span>
<span data-ttu-id="d9bde-180">Нет</span><span class="sxs-lookup"><span data-stu-id="d9bde-180">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d9bde-181">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d9bde-181">JSON representation</span></span>

<span data-ttu-id="d9bde-182">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d9bde-182">The following is a JSON representation of the resource.</span></span>

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


