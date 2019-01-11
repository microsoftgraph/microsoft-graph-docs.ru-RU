---
title: Тип ресурса bookingService
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: 63eae84249501426c43ad73326cbf005009753be
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815444"
---
# <a name="bookingservice-resource-type"></a><span data-ttu-id="bcddf-104">Тип ресурса bookingService</span><span class="sxs-lookup"><span data-stu-id="bcddf-104">bookingService resource type</span></span>

 > <span data-ttu-id="bcddf-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bcddf-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bcddf-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bcddf-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="bcddf-107">Представляет сведения об определенной службы, предоставляемые [bookingBusiness](bookingbusiness.md), такие как имя службы, цены и персонала, который обычно предоставляет такие службы.</span><span class="sxs-lookup"><span data-stu-id="bcddf-107">Represents information about a particular service provided by a [bookingBusiness](bookingbusiness.md), such as the service name, price, and the staff that usually provides such service.</span></span>

## <a name="methods"></a><span data-ttu-id="bcddf-108">Методы</span><span class="sxs-lookup"><span data-stu-id="bcddf-108">Methods</span></span>

| <span data-ttu-id="bcddf-109">Метод</span><span class="sxs-lookup"><span data-stu-id="bcddf-109">Method</span></span>           | <span data-ttu-id="bcddf-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bcddf-110">Return Type</span></span>    |<span data-ttu-id="bcddf-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bcddf-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bcddf-112">Список служб</span><span class="sxs-lookup"><span data-stu-id="bcddf-112">List services</span></span>](../api/bookingbusiness-list-services.md) | <span data-ttu-id="bcddf-113">[bookingService](bookingservice.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="bcddf-113">[bookingService](bookingservice.md) collection</span></span> | <span data-ttu-id="bcddf-114">Получите список объектов **bookingService** в указанном [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="bcddf-114">Get a list of **bookingService** objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="bcddf-115">Создание bookingService</span><span class="sxs-lookup"><span data-stu-id="bcddf-115">Create bookingService</span></span>](../api/bookingbusiness-post-services.md) | [<span data-ttu-id="bcddf-116">bookingService</span><span class="sxs-lookup"><span data-stu-id="bcddf-116">bookingService</span></span>](bookingservice.md) | <span data-ttu-id="bcddf-117">Создание **bookingService** для указанного [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="bcddf-117">Create a **bookingService** for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="bcddf-118">Получение bookingService</span><span class="sxs-lookup"><span data-stu-id="bcddf-118">Get bookingService</span></span>](../api/bookingservice-get.md) | [<span data-ttu-id="bcddf-119">bookingService</span><span class="sxs-lookup"><span data-stu-id="bcddf-119">bookingService</span></span>](bookingservice.md) |<span data-ttu-id="bcddf-120">Получите свойства и связи объекта **bookingService** в указанном [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="bcddf-120">Get the properties and relationships of a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|<span data-ttu-id="bcddf-121">[обновление](../api/bookingservice-update.md).</span><span class="sxs-lookup"><span data-stu-id="bcddf-121">[Update](../api/bookingservice-update.md)</span></span> | [<span data-ttu-id="bcddf-122">bookingService</span><span class="sxs-lookup"><span data-stu-id="bcddf-122">bookingService</span></span>](bookingservice.md)    |<span data-ttu-id="bcddf-123">Обновление объекта **bookingService** в указанном [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="bcddf-123">Update a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="bcddf-124">Delete</span><span class="sxs-lookup"><span data-stu-id="bcddf-124">Delete</span></span>](../api/bookingservice-delete.md) | <span data-ttu-id="bcddf-125">Нет</span><span class="sxs-lookup"><span data-stu-id="bcddf-125">None</span></span> |<span data-ttu-id="bcddf-126">Удаление объекта **bookingService** в указанном [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="bcddf-126">Delete a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |

## <a name="properties"></a><span data-ttu-id="bcddf-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="bcddf-127">Properties</span></span>
| <span data-ttu-id="bcddf-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="bcddf-128">Property</span></span>     | <span data-ttu-id="bcddf-129">Тип</span><span class="sxs-lookup"><span data-stu-id="bcddf-129">Type</span></span>   |<span data-ttu-id="bcddf-130">Описание</span><span class="sxs-lookup"><span data-stu-id="bcddf-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bcddf-131">defaultDuration</span><span class="sxs-lookup"><span data-stu-id="bcddf-131">defaultDuration</span></span>|<span data-ttu-id="bcddf-132">Продолжительность</span><span class="sxs-lookup"><span data-stu-id="bcddf-132">Duration</span></span>|<span data-ttu-id="bcddf-133">Длина по умолчанию службы, представленный в числа дней, часов, минут и секунд.</span><span class="sxs-lookup"><span data-stu-id="bcddf-133">The default length of the service, represented in numbers of days, hours, minutes, and seconds.</span></span> <span data-ttu-id="bcddf-134">Например P11D23H59M59.999999999999S.</span><span class="sxs-lookup"><span data-stu-id="bcddf-134">For example, P11D23H59M59.999999999999S.</span></span> |
|<span data-ttu-id="bcddf-135">defaultLocation</span><span class="sxs-lookup"><span data-stu-id="bcddf-135">defaultLocation</span></span>|[<span data-ttu-id="bcddf-136">location</span><span class="sxs-lookup"><span data-stu-id="bcddf-136">location</span></span>](location.md)|<span data-ttu-id="bcddf-137">Физическое расположение по умолчанию для службы.</span><span class="sxs-lookup"><span data-stu-id="bcddf-137">The default physical location for the service.</span></span>|
|<span data-ttu-id="bcddf-138">defaultPrice</span><span class="sxs-lookup"><span data-stu-id="bcddf-138">defaultPrice</span></span>|<span data-ttu-id="bcddf-139">Double</span><span class="sxs-lookup"><span data-stu-id="bcddf-139">Double</span></span>|<span data-ttu-id="bcddf-140">Денежные Цена по умолчанию для службы.</span><span class="sxs-lookup"><span data-stu-id="bcddf-140">The default monetary price for the service.</span></span>|
|<span data-ttu-id="bcddf-141">defaultPriceType</span><span class="sxs-lookup"><span data-stu-id="bcddf-141">defaultPriceType</span></span>|<span data-ttu-id="bcddf-142">string</span><span class="sxs-lookup"><span data-stu-id="bcddf-142">string</span></span>|<span data-ttu-id="bcddf-143">По умолчанию способ службу оценивается.</span><span class="sxs-lookup"><span data-stu-id="bcddf-143">The default way the service is charged.</span></span> <span data-ttu-id="bcddf-144">Возможные значения: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="bcddf-144">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="bcddf-145">defaultReminders</span><span class="sxs-lookup"><span data-stu-id="bcddf-145">defaultReminders</span></span>|<span data-ttu-id="bcddf-146">[bookingReminder](bookingreminder.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="bcddf-146">[bookingReminder](bookingreminder.md) collection</span></span>|<span data-ttu-id="bcddf-147">Значение по умолчанию набора оповещения о встрече этой службы.</span><span class="sxs-lookup"><span data-stu-id="bcddf-147">The default set of reminders for an appointment of this service.</span></span> <span data-ttu-id="bcddf-148">Значение этого свойства доступна только при чтении этой **bookingService** по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="bcddf-148">The value of this property is available only when reading this **bookingService** by its ID.</span></span>|
|<span data-ttu-id="bcddf-149">описание</span><span class="sxs-lookup"><span data-stu-id="bcddf-149">description</span></span>|<span data-ttu-id="bcddf-150">Строка</span><span class="sxs-lookup"><span data-stu-id="bcddf-150">String</span></span>|<span data-ttu-id="bcddf-151">Текстовое описание для службы.</span><span class="sxs-lookup"><span data-stu-id="bcddf-151">A text description for the service.</span></span>|
|<span data-ttu-id="bcddf-152">displayName</span><span class="sxs-lookup"><span data-stu-id="bcddf-152">displayName</span></span>|<span data-ttu-id="bcddf-153">Строка</span><span class="sxs-lookup"><span data-stu-id="bcddf-153">String</span></span>|<span data-ttu-id="bcddf-154">Имя службы.</span><span class="sxs-lookup"><span data-stu-id="bcddf-154">A service name.</span></span>|
|<span data-ttu-id="bcddf-155">emailAddress</span><span class="sxs-lookup"><span data-stu-id="bcddf-155">emailAddress</span></span>|<span data-ttu-id="bcddf-156">String</span><span class="sxs-lookup"><span data-stu-id="bcddf-156">String</span></span>|<span data-ttu-id="bcddf-157">Адрес электронной почты</span><span class="sxs-lookup"><span data-stu-id="bcddf-157">An email address</span></span>|
|<span data-ttu-id="bcddf-158">id</span><span class="sxs-lookup"><span data-stu-id="bcddf-158">id</span></span>|<span data-ttu-id="bcddf-159">Строка</span><span class="sxs-lookup"><span data-stu-id="bcddf-159">String</span></span>|<span data-ttu-id="bcddf-160">Идентификатор службы, в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="bcddf-160">The ID of that service, in a GUID format.</span></span> <span data-ttu-id="bcddf-161">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bcddf-161">Read-only.</span></span>|
|<span data-ttu-id="bcddf-162">isHiddenFromCustomers</span><span class="sxs-lookup"><span data-stu-id="bcddf-162">isHiddenFromCustomers</span></span>|<span data-ttu-id="bcddf-163">Логический</span><span class="sxs-lookup"><span data-stu-id="bcddf-163">Boolean</span></span>|<span data-ttu-id="bcddf-164">Значение true означает, что эта служба недоступна для клиентов для резервирования.</span><span class="sxs-lookup"><span data-stu-id="bcddf-164">True means this service is not available to customers for booking.</span></span>|
|<span data-ttu-id="bcddf-165">notes</span><span class="sxs-lookup"><span data-stu-id="bcddf-165">notes</span></span>|<span data-ttu-id="bcddf-166">String</span><span class="sxs-lookup"><span data-stu-id="bcddf-166">String</span></span>|<span data-ttu-id="bcddf-167">Дополнительные сведения об этой службы.</span><span class="sxs-lookup"><span data-stu-id="bcddf-167">Additional information about this service.</span></span>|
|<span data-ttu-id="bcddf-168">postBuffer</span><span class="sxs-lookup"><span data-stu-id="bcddf-168">postBuffer</span></span>|<span data-ttu-id="bcddf-169">Продолжительность</span><span class="sxs-lookup"><span data-stu-id="bcddf-169">Duration</span></span>|<span data-ttu-id="bcddf-170">Заканчивается время буфер после встречи для этой службы и перед следующим встречи клиента можно заранее.</span><span class="sxs-lookup"><span data-stu-id="bcddf-170">The time to buffer after an appointment for this service ends, and before the next customer appointment can be booked.</span></span>|
|<span data-ttu-id="bcddf-171">пребуфер</span><span class="sxs-lookup"><span data-stu-id="bcddf-171">preBuffer</span></span>|<span data-ttu-id="bcddf-172">Продолжительность</span><span class="sxs-lookup"><span data-stu-id="bcddf-172">Duration</span></span>|<span data-ttu-id="bcddf-173">Время для буфера до начала встречи для этой службы.</span><span class="sxs-lookup"><span data-stu-id="bcddf-173">The time to buffer before an appointment for this service can start.</span></span>|
|<span data-ttu-id="bcddf-174">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="bcddf-174">schedulingPolicy</span></span>|[<span data-ttu-id="bcddf-175">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="bcddf-175">bookingSchedulingPolicy</span></span>](bookingschedulingpolicy.md)|<span data-ttu-id="bcddf-176">Набор политик, определяющие порядок встреч для этого типа службы следует создания и управления.</span><span class="sxs-lookup"><span data-stu-id="bcddf-176">The set of policies that determine how appointments for this type of service should be created and managed.</span></span>|
|<span data-ttu-id="bcddf-177">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="bcddf-177">staffMemberIds</span></span>|<span data-ttu-id="bcddf-178">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="bcddf-178">String collection</span></span>|<span data-ttu-id="bcddf-179">Представляет эти [Сотрудники](bookingstaffmember.md) , предоставляющих этой службы.</span><span class="sxs-lookup"><span data-stu-id="bcddf-179">Represents those [staff members](bookingstaffmember.md) who provide this service.</span></span> |

## <a name="relationships"></a><span data-ttu-id="bcddf-180">Связи</span><span class="sxs-lookup"><span data-stu-id="bcddf-180">Relationships</span></span>
<span data-ttu-id="bcddf-181">Нет</span><span class="sxs-lookup"><span data-stu-id="bcddf-181">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="bcddf-182">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bcddf-182">JSON representation</span></span>

<span data-ttu-id="bcddf-183">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bcddf-183">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "bookingService resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
