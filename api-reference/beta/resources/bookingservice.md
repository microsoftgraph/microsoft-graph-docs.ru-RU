---
title: Тип ресурса Букингсервице
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 5f51ec999f0a2048b8dbcbdd533c609eb5a86757
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974131"
---
# <a name="bookingservice-resource-type"></a><span data-ttu-id="b5b75-104">Тип ресурса Букингсервице</span><span class="sxs-lookup"><span data-stu-id="b5b75-104">bookingService resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="b5b75-105">Представляет сведения о конкретной службе, предоставляемой [букингбусинесс](bookingbusiness.md), такие как имя службы, Цена и сотрудники, которые обычно предоставляют такую службу.</span><span class="sxs-lookup"><span data-stu-id="b5b75-105">Represents information about a particular service provided by a [bookingBusiness](bookingbusiness.md), such as the service name, price, and the staff that usually provides such service.</span></span>

## <a name="methods"></a><span data-ttu-id="b5b75-106">Методы</span><span class="sxs-lookup"><span data-stu-id="b5b75-106">Methods</span></span>

| <span data-ttu-id="b5b75-107">Метод</span><span class="sxs-lookup"><span data-stu-id="b5b75-107">Method</span></span>           | <span data-ttu-id="b5b75-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b5b75-108">Return Type</span></span>    |<span data-ttu-id="b5b75-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b5b75-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b5b75-110">Список служб</span><span class="sxs-lookup"><span data-stu-id="b5b75-110">List services</span></span>](../api/bookingbusiness-list-services.md) | <span data-ttu-id="b5b75-111">Коллекция [букингсервице](bookingservice.md)</span><span class="sxs-lookup"><span data-stu-id="b5b75-111">[bookingService](bookingservice.md) collection</span></span> | <span data-ttu-id="b5b75-112">Получение списка объектов **букингсервице** в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="b5b75-112">Get a list of **bookingService** objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="b5b75-113">Создание Букингсервице</span><span class="sxs-lookup"><span data-stu-id="b5b75-113">Create bookingService</span></span>](../api/bookingbusiness-post-services.md) | [<span data-ttu-id="b5b75-114">bookingService</span><span class="sxs-lookup"><span data-stu-id="b5b75-114">bookingService</span></span>](bookingservice.md) | <span data-ttu-id="b5b75-115">Создайте объект **букингсервице** для указанного [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="b5b75-115">Create a **bookingService** for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="b5b75-116">Получение Букингсервице</span><span class="sxs-lookup"><span data-stu-id="b5b75-116">Get bookingService</span></span>](../api/bookingservice-get.md) | [<span data-ttu-id="b5b75-117">bookingService</span><span class="sxs-lookup"><span data-stu-id="b5b75-117">bookingService</span></span>](bookingservice.md) |<span data-ttu-id="b5b75-118">Получение свойств и связей объекта **букингсервице** в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="b5b75-118">Get the properties and relationships of a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|<span data-ttu-id="b5b75-119">[обновление](../api/bookingservice-update.md);</span><span class="sxs-lookup"><span data-stu-id="b5b75-119">[Update](../api/bookingservice-update.md)</span></span> | [<span data-ttu-id="b5b75-120">bookingService</span><span class="sxs-lookup"><span data-stu-id="b5b75-120">bookingService</span></span>](bookingservice.md)    |<span data-ttu-id="b5b75-121">Обновление объекта **букингсервице** в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="b5b75-121">Update a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="b5b75-122">Удаление</span><span class="sxs-lookup"><span data-stu-id="b5b75-122">Delete</span></span>](../api/bookingservice-delete.md) | <span data-ttu-id="b5b75-123">Нет</span><span class="sxs-lookup"><span data-stu-id="b5b75-123">None</span></span> |<span data-ttu-id="b5b75-124">Удаление объекта **букингсервице** в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="b5b75-124">Delete a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |

## <a name="properties"></a><span data-ttu-id="b5b75-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="b5b75-125">Properties</span></span>
| <span data-ttu-id="b5b75-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="b5b75-126">Property</span></span>     | <span data-ttu-id="b5b75-127">Тип</span><span class="sxs-lookup"><span data-stu-id="b5b75-127">Type</span></span>   |<span data-ttu-id="b5b75-128">Описание</span><span class="sxs-lookup"><span data-stu-id="b5b75-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b5b75-129">Дефаултдуратион</span><span class="sxs-lookup"><span data-stu-id="b5b75-129">defaultDuration</span></span>|<span data-ttu-id="b5b75-130">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="b5b75-130">Duration</span></span>|<span data-ttu-id="b5b75-131">Длина службы по умолчанию, представленная в виде числа дней, часов, минут и секунд.</span><span class="sxs-lookup"><span data-stu-id="b5b75-131">The default length of the service, represented in numbers of days, hours, minutes, and seconds.</span></span> <span data-ttu-id="b5b75-132">Например, P11D23H59M 59.999999999999 S.</span><span class="sxs-lookup"><span data-stu-id="b5b75-132">For example, P11D23H59M59.999999999999S.</span></span> |
|<span data-ttu-id="b5b75-133">defaultLocation</span><span class="sxs-lookup"><span data-stu-id="b5b75-133">defaultLocation</span></span>|[<span data-ttu-id="b5b75-134">location</span><span class="sxs-lookup"><span data-stu-id="b5b75-134">location</span></span>](location.md)|<span data-ttu-id="b5b75-135">Физическое расположение службы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b5b75-135">The default physical location for the service.</span></span>|
|<span data-ttu-id="b5b75-136">Дефаултприце</span><span class="sxs-lookup"><span data-stu-id="b5b75-136">defaultPrice</span></span>|<span data-ttu-id="b5b75-137">Двойное</span><span class="sxs-lookup"><span data-stu-id="b5b75-137">Double</span></span>|<span data-ttu-id="b5b75-138">Денежная Цена по умолчанию для службы.</span><span class="sxs-lookup"><span data-stu-id="b5b75-138">The default monetary price for the service.</span></span>|
|<span data-ttu-id="b5b75-139">Дефаултприцетипе</span><span class="sxs-lookup"><span data-stu-id="b5b75-139">defaultPriceType</span></span>|<span data-ttu-id="b5b75-140">string</span><span class="sxs-lookup"><span data-stu-id="b5b75-140">string</span></span>|<span data-ttu-id="b5b75-141">Способ оплаты службы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b5b75-141">The default way the service is charged.</span></span> <span data-ttu-id="b5b75-142">Возможные значения: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="b5b75-142">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="b5b75-143">Дефаултреминдерс</span><span class="sxs-lookup"><span data-stu-id="b5b75-143">defaultReminders</span></span>|<span data-ttu-id="b5b75-144">Коллекция [букингреминдер](bookingreminder.md)</span><span class="sxs-lookup"><span data-stu-id="b5b75-144">[bookingReminder](bookingreminder.md) collection</span></span>|<span data-ttu-id="b5b75-145">Набор напоминаний по умолчанию для встречи этой службы.</span><span class="sxs-lookup"><span data-stu-id="b5b75-145">The default set of reminders for an appointment of this service.</span></span> <span data-ttu-id="b5b75-146">Значение этого свойства доступно только при чтении этого **букингсервице** с помощью идентификатора.</span><span class="sxs-lookup"><span data-stu-id="b5b75-146">The value of this property is available only when reading this **bookingService** by its ID.</span></span>|
|<span data-ttu-id="b5b75-147">description</span><span class="sxs-lookup"><span data-stu-id="b5b75-147">description</span></span>|<span data-ttu-id="b5b75-148">String</span><span class="sxs-lookup"><span data-stu-id="b5b75-148">String</span></span>|<span data-ttu-id="b5b75-149">Текстовое описание службы.</span><span class="sxs-lookup"><span data-stu-id="b5b75-149">A text description for the service.</span></span>|
|<span data-ttu-id="b5b75-150">displayName</span><span class="sxs-lookup"><span data-stu-id="b5b75-150">displayName</span></span>|<span data-ttu-id="b5b75-151">Строка</span><span class="sxs-lookup"><span data-stu-id="b5b75-151">String</span></span>|<span data-ttu-id="b5b75-152">Имя службы.</span><span class="sxs-lookup"><span data-stu-id="b5b75-152">A service name.</span></span>|
|<span data-ttu-id="b5b75-153">emailAddress</span><span class="sxs-lookup"><span data-stu-id="b5b75-153">emailAddress</span></span>|<span data-ttu-id="b5b75-154">String</span><span class="sxs-lookup"><span data-stu-id="b5b75-154">String</span></span>|<span data-ttu-id="b5b75-155">Адрес электронной почты</span><span class="sxs-lookup"><span data-stu-id="b5b75-155">An email address</span></span>|
|<span data-ttu-id="b5b75-156">id</span><span class="sxs-lookup"><span data-stu-id="b5b75-156">id</span></span>|<span data-ttu-id="b5b75-157">Строка</span><span class="sxs-lookup"><span data-stu-id="b5b75-157">String</span></span>|<span data-ttu-id="b5b75-158">Идентификатор этой службы в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="b5b75-158">The ID of that service, in a GUID format.</span></span> <span data-ttu-id="b5b75-159">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b5b75-159">Read-only.</span></span>|
|<span data-ttu-id="b5b75-160">Ишидденфромкустомерс</span><span class="sxs-lookup"><span data-stu-id="b5b75-160">isHiddenFromCustomers</span></span>|<span data-ttu-id="b5b75-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5b75-161">Boolean</span></span>|<span data-ttu-id="b5b75-162">Значение true означает, что эта служба недоступна клиентам для резервирования.</span><span class="sxs-lookup"><span data-stu-id="b5b75-162">True means this service is not available to customers for booking.</span></span>|
|<span data-ttu-id="b5b75-163">notes</span><span class="sxs-lookup"><span data-stu-id="b5b75-163">notes</span></span>|<span data-ttu-id="b5b75-164">String</span><span class="sxs-lookup"><span data-stu-id="b5b75-164">String</span></span>|<span data-ttu-id="b5b75-165">Дополнительные сведения об этой службе.</span><span class="sxs-lookup"><span data-stu-id="b5b75-165">Additional information about this service.</span></span>|
|<span data-ttu-id="b5b75-166">Буфер буфера</span><span class="sxs-lookup"><span data-stu-id="b5b75-166">postBuffer</span></span>|<span data-ttu-id="b5b75-167">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="b5b75-167">Duration</span></span>|<span data-ttu-id="b5b75-168">Время, в течение которого помещается в буфер после встречи для этой службы и до того, как может быть зарезервирована Следующая встреча покупателя.</span><span class="sxs-lookup"><span data-stu-id="b5b75-168">The time to buffer after an appointment for this service ends, and before the next customer appointment can be booked.</span></span>|
|<span data-ttu-id="b5b75-169">пребуфер</span><span class="sxs-lookup"><span data-stu-id="b5b75-169">preBuffer</span></span>|<span data-ttu-id="b5b75-170">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="b5b75-170">Duration</span></span>|<span data-ttu-id="b5b75-171">Время, в течение которого будет помещено в буфер, прежде чем можно будет запустить встречу для этой службы.</span><span class="sxs-lookup"><span data-stu-id="b5b75-171">The time to buffer before an appointment for this service can start.</span></span>|
|<span data-ttu-id="b5b75-172">Счедулингполици</span><span class="sxs-lookup"><span data-stu-id="b5b75-172">schedulingPolicy</span></span>|[<span data-ttu-id="b5b75-173">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="b5b75-173">bookingSchedulingPolicy</span></span>](bookingschedulingpolicy.md)|<span data-ttu-id="b5b75-174">Набор политик, определяющих, как должны создаваться встречи для этого типа службы и управлять ими.</span><span class="sxs-lookup"><span data-stu-id="b5b75-174">The set of policies that determine how appointments for this type of service should be created and managed.</span></span>|
|<span data-ttu-id="b5b75-175">Стаффмемберидс</span><span class="sxs-lookup"><span data-stu-id="b5b75-175">staffMemberIds</span></span>|<span data-ttu-id="b5b75-176">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b5b75-176">String collection</span></span>|<span data-ttu-id="b5b75-177">Представляет [сотрудников](bookingstaffmember.md) , которые предоставляют эту службу.</span><span class="sxs-lookup"><span data-stu-id="b5b75-177">Represents those [staff members](bookingstaffmember.md) who provide this service.</span></span> |

## <a name="relationships"></a><span data-ttu-id="b5b75-178">Отношения</span><span class="sxs-lookup"><span data-stu-id="b5b75-178">Relationships</span></span>
<span data-ttu-id="b5b75-179">Нет</span><span class="sxs-lookup"><span data-stu-id="b5b75-179">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="b5b75-180">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b5b75-180">JSON representation</span></span>

<span data-ttu-id="b5b75-181">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b5b75-181">The following is a JSON representation of the resource.</span></span>

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
