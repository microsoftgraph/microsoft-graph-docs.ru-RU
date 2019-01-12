---
title: Обновление bookingservice
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 6830ebc8fc101c4c9ce60f6157ed6bfdab82748c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937042"
---
# <a name="update-bookingservice"></a><span data-ttu-id="48f3f-104">Обновление bookingservice</span><span class="sxs-lookup"><span data-stu-id="48f3f-104">Update bookingservice</span></span>

 > <span data-ttu-id="48f3f-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="48f3f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="48f3f-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48f3f-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="48f3f-107">Обновление свойства объекта [bookingService](../resources/bookingservice.md) в указанном [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="48f3f-107">Update the properties of a [bookingService](../resources/bookingservice.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>

<span data-ttu-id="48f3f-108">Ниже приведены некоторые примеры, которые можно настроить для службы:</span><span class="sxs-lookup"><span data-stu-id="48f3f-108">The following are some examples you can customize for a service:</span></span>
- <span data-ttu-id="48f3f-109">Price</span><span class="sxs-lookup"><span data-stu-id="48f3f-109">Price</span></span>
- <span data-ttu-id="48f3f-110">Типичная длина встречи</span><span class="sxs-lookup"><span data-stu-id="48f3f-110">Typical length of an appointment</span></span>
- <span data-ttu-id="48f3f-111">Reminders</span><span class="sxs-lookup"><span data-stu-id="48f3f-111">Reminders</span></span>
- <span data-ttu-id="48f3f-112">Любой буфер времени для настройки перед или завершить после службы</span><span class="sxs-lookup"><span data-stu-id="48f3f-112">Any time buffer to set up before or finish up after the service</span></span>
- <span data-ttu-id="48f3f-113">[Планирование политики](../resources/bookingschedulingpolicy.md) параметров, таких как минимальные уведомление о книги или отменить, и ли клиенты могут выбрать элементы определенного персонала для встречи.</span><span class="sxs-lookup"><span data-stu-id="48f3f-113">[Scheduling policy](../resources/bookingschedulingpolicy.md) parameters such as minimum notice to book or cancel, and whether customers can select specific staff members for an appointment.</span></span>

## <a name="permissions"></a><span data-ttu-id="48f3f-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="48f3f-114">Permissions</span></span>
<span data-ttu-id="48f3f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48f3f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48f3f-117">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48f3f-117">Permission type</span></span>      | <span data-ttu-id="48f3f-118">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="48f3f-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48f3f-119">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48f3f-119">Delegated (work or school account)</span></span> |  <span data-ttu-id="48f3f-120">Bookings.ReadWrite.All Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="48f3f-120">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="48f3f-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48f3f-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48f3f-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48f3f-122">Not supported.</span></span>   |
|<span data-ttu-id="48f3f-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="48f3f-123">Application</span></span> | <span data-ttu-id="48f3f-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48f3f-124">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="48f3f-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48f3f-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/services/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="48f3f-126">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="48f3f-126">Optional request headers</span></span>
| <span data-ttu-id="48f3f-127">Имя</span><span class="sxs-lookup"><span data-stu-id="48f3f-127">Name</span></span>       | <span data-ttu-id="48f3f-128">Описание</span><span class="sxs-lookup"><span data-stu-id="48f3f-128">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="48f3f-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="48f3f-129">Authorization</span></span>  | <span data-ttu-id="48f3f-130">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="48f3f-130">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="48f3f-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="48f3f-131">Request body</span></span>
<span data-ttu-id="48f3f-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="48f3f-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="48f3f-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="48f3f-135">Property</span></span>     | <span data-ttu-id="48f3f-136">Тип</span><span class="sxs-lookup"><span data-stu-id="48f3f-136">Type</span></span>   |<span data-ttu-id="48f3f-137">Описание</span><span class="sxs-lookup"><span data-stu-id="48f3f-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="48f3f-138">defaultDuration</span><span class="sxs-lookup"><span data-stu-id="48f3f-138">defaultDuration</span></span>|<span data-ttu-id="48f3f-139">Продолжительность</span><span class="sxs-lookup"><span data-stu-id="48f3f-139">Duration</span></span>|<span data-ttu-id="48f3f-140">Длина по умолчанию службы, представленный в числа дней, часов, минут и секунд.</span><span class="sxs-lookup"><span data-stu-id="48f3f-140">The default length of the service, represented in numbers of days, hours, minutes, and seconds.</span></span> <span data-ttu-id="48f3f-141">Например P11D23H59M59.999999999999S.</span><span class="sxs-lookup"><span data-stu-id="48f3f-141">For example, P11D23H59M59.999999999999S.</span></span> |
|<span data-ttu-id="48f3f-142">defaultLocation</span><span class="sxs-lookup"><span data-stu-id="48f3f-142">defaultLocation</span></span>|[<span data-ttu-id="48f3f-143">location</span><span class="sxs-lookup"><span data-stu-id="48f3f-143">location</span></span>](../resources/location.md)|<span data-ttu-id="48f3f-144">Физическое расположение по умолчанию для службы.</span><span class="sxs-lookup"><span data-stu-id="48f3f-144">The default physical location for the service.</span></span>|
|<span data-ttu-id="48f3f-145">defaultPrice</span><span class="sxs-lookup"><span data-stu-id="48f3f-145">defaultPrice</span></span>|<span data-ttu-id="48f3f-146">Double</span><span class="sxs-lookup"><span data-stu-id="48f3f-146">Double</span></span>|<span data-ttu-id="48f3f-147">Денежные Цена по умолчанию для службы.</span><span class="sxs-lookup"><span data-stu-id="48f3f-147">The default monetary price for the service.</span></span>|
|<span data-ttu-id="48f3f-148">defaultPriceType</span><span class="sxs-lookup"><span data-stu-id="48f3f-148">defaultPriceType</span></span>|<span data-ttu-id="48f3f-149">строка</span><span class="sxs-lookup"><span data-stu-id="48f3f-149">string</span></span>|<span data-ttu-id="48f3f-150">По умолчанию способ службу оценивается.</span><span class="sxs-lookup"><span data-stu-id="48f3f-150">The default way the service is charged.</span></span> <span data-ttu-id="48f3f-151">Возможные значения: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="48f3f-151">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="48f3f-152">defaultReminders</span><span class="sxs-lookup"><span data-stu-id="48f3f-152">defaultReminders</span></span>|<span data-ttu-id="48f3f-153">[bookingReminder](../resources/bookingreminder.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="48f3f-153">[bookingReminder](../resources/bookingreminder.md) collection</span></span>|<span data-ttu-id="48f3f-154">Значение по умолчанию набора оповещения о встрече этой службы.</span><span class="sxs-lookup"><span data-stu-id="48f3f-154">The default set of reminders for an appointment of this service.</span></span> <span data-ttu-id="48f3f-155">Значение этого свойства доступна только при чтении этой **bookingService** по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="48f3f-155">The value of this property is available only when reading this **bookingService** by its ID.</span></span>|
|<span data-ttu-id="48f3f-156">описание</span><span class="sxs-lookup"><span data-stu-id="48f3f-156">description</span></span>|<span data-ttu-id="48f3f-157">String</span><span class="sxs-lookup"><span data-stu-id="48f3f-157">String</span></span>|<span data-ttu-id="48f3f-158">Текстовое описание для службы.</span><span class="sxs-lookup"><span data-stu-id="48f3f-158">A text description for the service.</span></span>|
|<span data-ttu-id="48f3f-159">displayName</span><span class="sxs-lookup"><span data-stu-id="48f3f-159">displayName</span></span>|<span data-ttu-id="48f3f-160">String</span><span class="sxs-lookup"><span data-stu-id="48f3f-160">String</span></span>|<span data-ttu-id="48f3f-161">Имя службы.</span><span class="sxs-lookup"><span data-stu-id="48f3f-161">A service name.</span></span>|
|<span data-ttu-id="48f3f-162">emailAddress</span><span class="sxs-lookup"><span data-stu-id="48f3f-162">emailAddress</span></span>|<span data-ttu-id="48f3f-163">String</span><span class="sxs-lookup"><span data-stu-id="48f3f-163">String</span></span>|<span data-ttu-id="48f3f-164">Адрес электронной почты</span><span class="sxs-lookup"><span data-stu-id="48f3f-164">An email address</span></span>|
|<span data-ttu-id="48f3f-165">id</span><span class="sxs-lookup"><span data-stu-id="48f3f-165">id</span></span>|<span data-ttu-id="48f3f-166">String</span><span class="sxs-lookup"><span data-stu-id="48f3f-166">String</span></span>| <span data-ttu-id="48f3f-167">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="48f3f-167">Read-only.</span></span>|
|<span data-ttu-id="48f3f-168">isHiddenFromCustomers</span><span class="sxs-lookup"><span data-stu-id="48f3f-168">isHiddenFromCustomers</span></span>|<span data-ttu-id="48f3f-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="48f3f-169">Boolean</span></span>|<span data-ttu-id="48f3f-170">Значение true означает, что эта служба недоступна для клиентов для резервирования.</span><span class="sxs-lookup"><span data-stu-id="48f3f-170">True means this service is not available to customers for booking.</span></span>|
|<span data-ttu-id="48f3f-171">notes</span><span class="sxs-lookup"><span data-stu-id="48f3f-171">notes</span></span>|<span data-ttu-id="48f3f-172">String</span><span class="sxs-lookup"><span data-stu-id="48f3f-172">String</span></span>|<span data-ttu-id="48f3f-173">Дополнительные сведения об этой службы.</span><span class="sxs-lookup"><span data-stu-id="48f3f-173">Additional information about this service.</span></span>|
|<span data-ttu-id="48f3f-174">postBuffer</span><span class="sxs-lookup"><span data-stu-id="48f3f-174">postBuffer</span></span>|<span data-ttu-id="48f3f-175">Продолжительность</span><span class="sxs-lookup"><span data-stu-id="48f3f-175">Duration</span></span>|<span data-ttu-id="48f3f-176">Заканчивается время буфер после встречи для этой службы и перед следующим встречи клиента можно заранее.</span><span class="sxs-lookup"><span data-stu-id="48f3f-176">The time to buffer after an appointment for this service ends, and before the next customer appointment can be booked.</span></span>|
|<span data-ttu-id="48f3f-177">пребуфер</span><span class="sxs-lookup"><span data-stu-id="48f3f-177">preBuffer</span></span>|<span data-ttu-id="48f3f-178">Продолжительность</span><span class="sxs-lookup"><span data-stu-id="48f3f-178">Duration</span></span>|<span data-ttu-id="48f3f-179">Время для буфера до начала встречи для этой службы.</span><span class="sxs-lookup"><span data-stu-id="48f3f-179">The time to buffer before an appointment for this service can start.</span></span>|
|<span data-ttu-id="48f3f-180">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="48f3f-180">schedulingPolicy</span></span>|[<span data-ttu-id="48f3f-181">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="48f3f-181">bookingSchedulingPolicy</span></span>](../resources/bookingschedulingpolicy.md)|<span data-ttu-id="48f3f-182">Набор политик, определяющие порядок встреч для этого типа службы следует создания и управления.</span><span class="sxs-lookup"><span data-stu-id="48f3f-182">The set of policies that determine how appointments for this type of service should be created and managed.</span></span>|
|<span data-ttu-id="48f3f-183">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="48f3f-183">staffMemberIds</span></span>|<span data-ttu-id="48f3f-184">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="48f3f-184">String collection</span></span>|<span data-ttu-id="48f3f-185">Представляет эти [Сотрудники](../resources/bookingstaffmember.md) , предоставляющих этой службы.</span><span class="sxs-lookup"><span data-stu-id="48f3f-185">Represents those [staff members](../resources/bookingstaffmember.md) who provide this service.</span></span> |

## <a name="response"></a><span data-ttu-id="48f3f-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="48f3f-186">Response</span></span>
<span data-ttu-id="48f3f-p108">При успешном выполнении этот метод возвращает код отклика `204 No content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="48f3f-p108">If successful, this method returns a `204 No content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="48f3f-189">Пример</span><span class="sxs-lookup"><span data-stu-id="48f3f-189">Example</span></span>
##### <a name="request"></a><span data-ttu-id="48f3f-190">Запрос</span><span class="sxs-lookup"><span data-stu-id="48f3f-190">Request</span></span>
<span data-ttu-id="48f3f-191">В следующем примере обновляются длительность указанной службы.</span><span class="sxs-lookup"><span data-stu-id="48f3f-191">The following example updates the duration of the specified service.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_bookingservice"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.bookingService",
    "defaultDuration":"PT30M"
}
```
##### <a name="response"></a><span data-ttu-id="48f3f-192">Отклик</span><span class="sxs-lookup"><span data-stu-id="48f3f-192">Response</span></span>
<span data-ttu-id="48f3f-193">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="48f3f-193">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update bookingservice",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
