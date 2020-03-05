---
title: Тип ресурса Букингсервице
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 2bdf2fa686023ce33233722b3cd05f2984d1cabb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507903"
---
# <a name="bookingservice-resource-type"></a><span data-ttu-id="72d97-104">Тип ресурса Букингсервице</span><span class="sxs-lookup"><span data-stu-id="72d97-104">bookingService resource type</span></span>

<span data-ttu-id="72d97-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="72d97-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="72d97-106">Представляет сведения о конкретной службе, предоставляемой [букингбусинесс](bookingbusiness.md), такие как имя службы, Цена и сотрудники, которые обычно предоставляют такую службу.</span><span class="sxs-lookup"><span data-stu-id="72d97-106">Represents information about a particular service provided by a [bookingBusiness](bookingbusiness.md), such as the service name, price, and the staff that usually provides such service.</span></span>

## <a name="methods"></a><span data-ttu-id="72d97-107">Методы</span><span class="sxs-lookup"><span data-stu-id="72d97-107">Methods</span></span>

| <span data-ttu-id="72d97-108">Метод</span><span class="sxs-lookup"><span data-stu-id="72d97-108">Method</span></span>           | <span data-ttu-id="72d97-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="72d97-109">Return Type</span></span>    |<span data-ttu-id="72d97-110">Описание</span><span class="sxs-lookup"><span data-stu-id="72d97-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="72d97-111">Список служб</span><span class="sxs-lookup"><span data-stu-id="72d97-111">List services</span></span>](../api/bookingbusiness-list-services.md) | <span data-ttu-id="72d97-112">Коллекция [букингсервице](bookingservice.md)</span><span class="sxs-lookup"><span data-stu-id="72d97-112">[bookingService](bookingservice.md) collection</span></span> | <span data-ttu-id="72d97-113">Получение списка объектов **букингсервице** в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="72d97-113">Get a list of **bookingService** objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="72d97-114">Создание Букингсервице</span><span class="sxs-lookup"><span data-stu-id="72d97-114">Create bookingService</span></span>](../api/bookingbusiness-post-services.md) | [<span data-ttu-id="72d97-115">bookingService</span><span class="sxs-lookup"><span data-stu-id="72d97-115">bookingService</span></span>](bookingservice.md) | <span data-ttu-id="72d97-116">Создайте объект **букингсервице** для указанного [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="72d97-116">Create a **bookingService** for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="72d97-117">Получение Букингсервице</span><span class="sxs-lookup"><span data-stu-id="72d97-117">Get bookingService</span></span>](../api/bookingservice-get.md) | [<span data-ttu-id="72d97-118">bookingService</span><span class="sxs-lookup"><span data-stu-id="72d97-118">bookingService</span></span>](bookingservice.md) |<span data-ttu-id="72d97-119">Получение свойств и связей объекта **букингсервице** в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="72d97-119">Get the properties and relationships of a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|<span data-ttu-id="72d97-120">[обновление](../api/bookingservice-update.md).</span><span class="sxs-lookup"><span data-stu-id="72d97-120">[Update](../api/bookingservice-update.md)</span></span> | [<span data-ttu-id="72d97-121">bookingService</span><span class="sxs-lookup"><span data-stu-id="72d97-121">bookingService</span></span>](bookingservice.md)    |<span data-ttu-id="72d97-122">Обновление объекта **букингсервице** в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="72d97-122">Update a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|<span data-ttu-id="72d97-123">[удаление](../api/bookingservice-delete.md);</span><span class="sxs-lookup"><span data-stu-id="72d97-123">[Delete](../api/bookingservice-delete.md)</span></span> | <span data-ttu-id="72d97-124">Нет</span><span class="sxs-lookup"><span data-stu-id="72d97-124">None</span></span> |<span data-ttu-id="72d97-125">Удаление объекта **букингсервице** в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="72d97-125">Delete a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |

## <a name="properties"></a><span data-ttu-id="72d97-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="72d97-126">Properties</span></span>
| <span data-ttu-id="72d97-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="72d97-127">Property</span></span>     | <span data-ttu-id="72d97-128">Тип</span><span class="sxs-lookup"><span data-stu-id="72d97-128">Type</span></span>   |<span data-ttu-id="72d97-129">Описание</span><span class="sxs-lookup"><span data-stu-id="72d97-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="72d97-130">дефаултдуратион</span><span class="sxs-lookup"><span data-stu-id="72d97-130">defaultDuration</span></span>|<span data-ttu-id="72d97-131">Длительность</span><span class="sxs-lookup"><span data-stu-id="72d97-131">Duration</span></span>|<span data-ttu-id="72d97-132">Длина службы по умолчанию, представленная в виде числа дней, часов, минут и секунд.</span><span class="sxs-lookup"><span data-stu-id="72d97-132">The default length of the service, represented in numbers of days, hours, minutes, and seconds.</span></span> <span data-ttu-id="72d97-133">Например, P11D23H59M 59.999999999999 S.</span><span class="sxs-lookup"><span data-stu-id="72d97-133">For example, P11D23H59M59.999999999999S.</span></span> |
|<span data-ttu-id="72d97-134">defaultLocation</span><span class="sxs-lookup"><span data-stu-id="72d97-134">defaultLocation</span></span>|[<span data-ttu-id="72d97-135">location</span><span class="sxs-lookup"><span data-stu-id="72d97-135">location</span></span>](location.md)|<span data-ttu-id="72d97-136">Физическое расположение службы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="72d97-136">The default physical location for the service.</span></span>|
|<span data-ttu-id="72d97-137">дефаултприце</span><span class="sxs-lookup"><span data-stu-id="72d97-137">defaultPrice</span></span>|<span data-ttu-id="72d97-138">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="72d97-138">Double</span></span>|<span data-ttu-id="72d97-139">Денежная Цена по умолчанию для службы.</span><span class="sxs-lookup"><span data-stu-id="72d97-139">The default monetary price for the service.</span></span>|
|<span data-ttu-id="72d97-140">дефаултприцетипе</span><span class="sxs-lookup"><span data-stu-id="72d97-140">defaultPriceType</span></span>|<span data-ttu-id="72d97-141">строка</span><span class="sxs-lookup"><span data-stu-id="72d97-141">string</span></span>|<span data-ttu-id="72d97-142">Способ оплаты службы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="72d97-142">The default way the service is charged.</span></span> <span data-ttu-id="72d97-143">Возможные значения: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="72d97-143">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="72d97-144">дефаултреминдерс</span><span class="sxs-lookup"><span data-stu-id="72d97-144">defaultReminders</span></span>|<span data-ttu-id="72d97-145">Коллекция [букингреминдер](bookingreminder.md)</span><span class="sxs-lookup"><span data-stu-id="72d97-145">[bookingReminder](bookingreminder.md) collection</span></span>|<span data-ttu-id="72d97-146">Набор напоминаний по умолчанию для встречи этой службы.</span><span class="sxs-lookup"><span data-stu-id="72d97-146">The default set of reminders for an appointment of this service.</span></span> <span data-ttu-id="72d97-147">Значение этого свойства доступно только при чтении этого **букингсервице** с помощью идентификатора.</span><span class="sxs-lookup"><span data-stu-id="72d97-147">The value of this property is available only when reading this **bookingService** by its ID.</span></span>|
|<span data-ttu-id="72d97-148">description</span><span class="sxs-lookup"><span data-stu-id="72d97-148">description</span></span>|<span data-ttu-id="72d97-149">String</span><span class="sxs-lookup"><span data-stu-id="72d97-149">String</span></span>|<span data-ttu-id="72d97-150">Текстовое описание службы.</span><span class="sxs-lookup"><span data-stu-id="72d97-150">A text description for the service.</span></span>|
|<span data-ttu-id="72d97-151">displayName</span><span class="sxs-lookup"><span data-stu-id="72d97-151">displayName</span></span>|<span data-ttu-id="72d97-152">Строка</span><span class="sxs-lookup"><span data-stu-id="72d97-152">String</span></span>|<span data-ttu-id="72d97-153">Имя службы.</span><span class="sxs-lookup"><span data-stu-id="72d97-153">A service name.</span></span>|
|<span data-ttu-id="72d97-154">emailAddress</span><span class="sxs-lookup"><span data-stu-id="72d97-154">emailAddress</span></span>|<span data-ttu-id="72d97-155">String</span><span class="sxs-lookup"><span data-stu-id="72d97-155">String</span></span>|<span data-ttu-id="72d97-156">Адрес электронной почты</span><span class="sxs-lookup"><span data-stu-id="72d97-156">An email address</span></span>|
|<span data-ttu-id="72d97-157">id</span><span class="sxs-lookup"><span data-stu-id="72d97-157">id</span></span>|<span data-ttu-id="72d97-158">Строка</span><span class="sxs-lookup"><span data-stu-id="72d97-158">String</span></span>|<span data-ttu-id="72d97-159">Идентификатор этой службы в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="72d97-159">The ID of that service, in a GUID format.</span></span> <span data-ttu-id="72d97-160">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="72d97-160">Read-only.</span></span>|
|<span data-ttu-id="72d97-161">ишидденфромкустомерс</span><span class="sxs-lookup"><span data-stu-id="72d97-161">isHiddenFromCustomers</span></span>|<span data-ttu-id="72d97-162">Логический</span><span class="sxs-lookup"><span data-stu-id="72d97-162">Boolean</span></span>|<span data-ttu-id="72d97-163">Значение true означает, что эта служба недоступна клиентам для резервирования.</span><span class="sxs-lookup"><span data-stu-id="72d97-163">True means this service is not available to customers for booking.</span></span>|
|<span data-ttu-id="72d97-164">notes</span><span class="sxs-lookup"><span data-stu-id="72d97-164">notes</span></span>|<span data-ttu-id="72d97-165">String</span><span class="sxs-lookup"><span data-stu-id="72d97-165">String</span></span>|<span data-ttu-id="72d97-166">Дополнительные сведения об этой службе.</span><span class="sxs-lookup"><span data-stu-id="72d97-166">Additional information about this service.</span></span>|
|<span data-ttu-id="72d97-167">Буфер буфера</span><span class="sxs-lookup"><span data-stu-id="72d97-167">postBuffer</span></span>|<span data-ttu-id="72d97-168">Длительность</span><span class="sxs-lookup"><span data-stu-id="72d97-168">Duration</span></span>|<span data-ttu-id="72d97-169">Время, в течение которого помещается в буфер после встречи для этой службы и до того, как может быть зарезервирована Следующая встреча покупателя.</span><span class="sxs-lookup"><span data-stu-id="72d97-169">The time to buffer after an appointment for this service ends, and before the next customer appointment can be booked.</span></span>|
|<span data-ttu-id="72d97-170">пребуфер</span><span class="sxs-lookup"><span data-stu-id="72d97-170">preBuffer</span></span>|<span data-ttu-id="72d97-171">Длительность</span><span class="sxs-lookup"><span data-stu-id="72d97-171">Duration</span></span>|<span data-ttu-id="72d97-172">Время, в течение которого будет помещено в буфер, прежде чем можно будет запустить встречу для этой службы.</span><span class="sxs-lookup"><span data-stu-id="72d97-172">The time to buffer before an appointment for this service can start.</span></span>|
|<span data-ttu-id="72d97-173">счедулингполици</span><span class="sxs-lookup"><span data-stu-id="72d97-173">schedulingPolicy</span></span>|[<span data-ttu-id="72d97-174">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="72d97-174">bookingSchedulingPolicy</span></span>](bookingschedulingpolicy.md)|<span data-ttu-id="72d97-175">Набор политик, определяющих, как должны создаваться встречи для этого типа службы и управлять ими.</span><span class="sxs-lookup"><span data-stu-id="72d97-175">The set of policies that determine how appointments for this type of service should be created and managed.</span></span>|
|<span data-ttu-id="72d97-176">стаффмемберидс</span><span class="sxs-lookup"><span data-stu-id="72d97-176">staffMemberIds</span></span>|<span data-ttu-id="72d97-177">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="72d97-177">String collection</span></span>|<span data-ttu-id="72d97-178">Представляет [сотрудников](bookingstaffmember.md) , которые предоставляют эту службу.</span><span class="sxs-lookup"><span data-stu-id="72d97-178">Represents those [staff members](bookingstaffmember.md) who provide this service.</span></span> |

## <a name="relationships"></a><span data-ttu-id="72d97-179">Связи</span><span class="sxs-lookup"><span data-stu-id="72d97-179">Relationships</span></span>
<span data-ttu-id="72d97-180">Нет</span><span class="sxs-lookup"><span data-stu-id="72d97-180">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="72d97-181">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="72d97-181">JSON representation</span></span>

<span data-ttu-id="72d97-182">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="72d97-182">The following is a JSON representation of the resource.</span></span>

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
