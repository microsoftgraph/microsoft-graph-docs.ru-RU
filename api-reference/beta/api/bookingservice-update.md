---
title: Обновление bookingservice
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: 6eee5949d5d8cee23821d726563b4687febd77a7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838922"
---
# <a name="update-bookingservice"></a><span data-ttu-id="d79f4-104">Обновление bookingservice</span><span class="sxs-lookup"><span data-stu-id="d79f4-104">Update bookingservice</span></span>

 > <span data-ttu-id="d79f4-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d79f4-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d79f4-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d79f4-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="d79f4-107">Обновление свойства объекта [bookingService](../resources/bookingservice.md) в указанном [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="d79f4-107">Update the properties of a [bookingService](../resources/bookingservice.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>

<span data-ttu-id="d79f4-108">Ниже приведены некоторые примеры, которые можно настроить для службы:</span><span class="sxs-lookup"><span data-stu-id="d79f4-108">The following are some examples you can customize for a service:</span></span>
- <span data-ttu-id="d79f4-109">Price</span><span class="sxs-lookup"><span data-stu-id="d79f4-109">Price</span></span>
- <span data-ttu-id="d79f4-110">Типичная длина встречи</span><span class="sxs-lookup"><span data-stu-id="d79f4-110">Typical length of an appointment</span></span>
- <span data-ttu-id="d79f4-111">Reminders</span><span class="sxs-lookup"><span data-stu-id="d79f4-111">Reminders</span></span>
- <span data-ttu-id="d79f4-112">Любой буфер времени для настройки перед или завершить после службы</span><span class="sxs-lookup"><span data-stu-id="d79f4-112">Any time buffer to set up before or finish up after the service</span></span>
- <span data-ttu-id="d79f4-113">[Планирование политики](../resources/bookingschedulingpolicy.md) параметров, таких как минимальные уведомление о книги или отменить, и ли клиенты могут выбрать элементы определенного персонала для встречи.</span><span class="sxs-lookup"><span data-stu-id="d79f4-113">[Scheduling policy](../resources/bookingschedulingpolicy.md) parameters such as minimum notice to book or cancel, and whether customers can select specific staff members for an appointment.</span></span>

## <a name="permissions"></a><span data-ttu-id="d79f4-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d79f4-114">Permissions</span></span>
<span data-ttu-id="d79f4-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d79f4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d79f4-117">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d79f4-117">Permission type</span></span>      | <span data-ttu-id="d79f4-118">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d79f4-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d79f4-119">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d79f4-119">Delegated (work or school account)</span></span> |  <span data-ttu-id="d79f4-120">Bookings.ReadWrite.All Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="d79f4-120">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="d79f4-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d79f4-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d79f4-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d79f4-122">Not supported.</span></span>   |
|<span data-ttu-id="d79f4-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d79f4-123">Application</span></span> | <span data-ttu-id="d79f4-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d79f4-124">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="d79f4-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d79f4-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/services/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="d79f4-126">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d79f4-126">Optional request headers</span></span>
| <span data-ttu-id="d79f4-127">Имя</span><span class="sxs-lookup"><span data-stu-id="d79f4-127">Name</span></span>       | <span data-ttu-id="d79f4-128">Описание</span><span class="sxs-lookup"><span data-stu-id="d79f4-128">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d79f4-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="d79f4-129">Authorization</span></span>  | <span data-ttu-id="d79f4-130">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="d79f4-130">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="d79f4-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d79f4-131">Request body</span></span>
<span data-ttu-id="d79f4-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="d79f4-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d79f4-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="d79f4-135">Property</span></span>     | <span data-ttu-id="d79f4-136">Тип</span><span class="sxs-lookup"><span data-stu-id="d79f4-136">Type</span></span>   |<span data-ttu-id="d79f4-137">Описание</span><span class="sxs-lookup"><span data-stu-id="d79f4-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d79f4-138">defaultDuration</span><span class="sxs-lookup"><span data-stu-id="d79f4-138">defaultDuration</span></span>|<span data-ttu-id="d79f4-139">Продолжительность</span><span class="sxs-lookup"><span data-stu-id="d79f4-139">Duration</span></span>|<span data-ttu-id="d79f4-140">Длина по умолчанию службы, представленный в числа дней, часов, минут и секунд.</span><span class="sxs-lookup"><span data-stu-id="d79f4-140">The default length of the service, represented in numbers of days, hours, minutes, and seconds.</span></span> <span data-ttu-id="d79f4-141">Например P11D23H59M59.999999999999S.</span><span class="sxs-lookup"><span data-stu-id="d79f4-141">For example, P11D23H59M59.999999999999S.</span></span> |
|<span data-ttu-id="d79f4-142">defaultLocation</span><span class="sxs-lookup"><span data-stu-id="d79f4-142">defaultLocation</span></span>|[<span data-ttu-id="d79f4-143">location</span><span class="sxs-lookup"><span data-stu-id="d79f4-143">location</span></span>](../resources/location.md)|<span data-ttu-id="d79f4-144">Физическое расположение по умолчанию для службы.</span><span class="sxs-lookup"><span data-stu-id="d79f4-144">The default physical location for the service.</span></span>|
|<span data-ttu-id="d79f4-145">defaultPrice</span><span class="sxs-lookup"><span data-stu-id="d79f4-145">defaultPrice</span></span>|<span data-ttu-id="d79f4-146">Double</span><span class="sxs-lookup"><span data-stu-id="d79f4-146">Double</span></span>|<span data-ttu-id="d79f4-147">Денежные Цена по умолчанию для службы.</span><span class="sxs-lookup"><span data-stu-id="d79f4-147">The default monetary price for the service.</span></span>|
|<span data-ttu-id="d79f4-148">defaultPriceType</span><span class="sxs-lookup"><span data-stu-id="d79f4-148">defaultPriceType</span></span>|<span data-ttu-id="d79f4-149">string</span><span class="sxs-lookup"><span data-stu-id="d79f4-149">string</span></span>|<span data-ttu-id="d79f4-150">По умолчанию способ службу оценивается.</span><span class="sxs-lookup"><span data-stu-id="d79f4-150">The default way the service is charged.</span></span> <span data-ttu-id="d79f4-151">Возможные значения: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="d79f4-151">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="d79f4-152">defaultReminders</span><span class="sxs-lookup"><span data-stu-id="d79f4-152">defaultReminders</span></span>|<span data-ttu-id="d79f4-153">[bookingReminder](../resources/bookingreminder.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="d79f4-153">[bookingReminder](../resources/bookingreminder.md) collection</span></span>|<span data-ttu-id="d79f4-154">Значение по умолчанию набора оповещения о встрече этой службы.</span><span class="sxs-lookup"><span data-stu-id="d79f4-154">The default set of reminders for an appointment of this service.</span></span> <span data-ttu-id="d79f4-155">Значение этого свойства доступна только при чтении этой **bookingService** по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="d79f4-155">The value of this property is available only when reading this **bookingService** by its ID.</span></span>|
|<span data-ttu-id="d79f4-156">описание</span><span class="sxs-lookup"><span data-stu-id="d79f4-156">description</span></span>|<span data-ttu-id="d79f4-157">Строка</span><span class="sxs-lookup"><span data-stu-id="d79f4-157">String</span></span>|<span data-ttu-id="d79f4-158">Текстовое описание для службы.</span><span class="sxs-lookup"><span data-stu-id="d79f4-158">A text description for the service.</span></span>|
|<span data-ttu-id="d79f4-159">displayName</span><span class="sxs-lookup"><span data-stu-id="d79f4-159">displayName</span></span>|<span data-ttu-id="d79f4-160">Строка</span><span class="sxs-lookup"><span data-stu-id="d79f4-160">String</span></span>|<span data-ttu-id="d79f4-161">Имя службы.</span><span class="sxs-lookup"><span data-stu-id="d79f4-161">A service name.</span></span>|
|<span data-ttu-id="d79f4-162">emailAddress</span><span class="sxs-lookup"><span data-stu-id="d79f4-162">emailAddress</span></span>|<span data-ttu-id="d79f4-163">String</span><span class="sxs-lookup"><span data-stu-id="d79f4-163">String</span></span>|<span data-ttu-id="d79f4-164">Адрес электронной почты</span><span class="sxs-lookup"><span data-stu-id="d79f4-164">An email address</span></span>|
|<span data-ttu-id="d79f4-165">id</span><span class="sxs-lookup"><span data-stu-id="d79f4-165">id</span></span>|<span data-ttu-id="d79f4-166">Строка</span><span class="sxs-lookup"><span data-stu-id="d79f4-166">String</span></span>| <span data-ttu-id="d79f4-167">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d79f4-167">Read-only.</span></span>|
|<span data-ttu-id="d79f4-168">isHiddenFromCustomers</span><span class="sxs-lookup"><span data-stu-id="d79f4-168">isHiddenFromCustomers</span></span>|<span data-ttu-id="d79f4-169">Логический</span><span class="sxs-lookup"><span data-stu-id="d79f4-169">Boolean</span></span>|<span data-ttu-id="d79f4-170">Значение true означает, что эта служба недоступна для клиентов для резервирования.</span><span class="sxs-lookup"><span data-stu-id="d79f4-170">True means this service is not available to customers for booking.</span></span>|
|<span data-ttu-id="d79f4-171">notes</span><span class="sxs-lookup"><span data-stu-id="d79f4-171">notes</span></span>|<span data-ttu-id="d79f4-172">String</span><span class="sxs-lookup"><span data-stu-id="d79f4-172">String</span></span>|<span data-ttu-id="d79f4-173">Дополнительные сведения об этой службы.</span><span class="sxs-lookup"><span data-stu-id="d79f4-173">Additional information about this service.</span></span>|
|<span data-ttu-id="d79f4-174">postBuffer</span><span class="sxs-lookup"><span data-stu-id="d79f4-174">postBuffer</span></span>|<span data-ttu-id="d79f4-175">Продолжительность</span><span class="sxs-lookup"><span data-stu-id="d79f4-175">Duration</span></span>|<span data-ttu-id="d79f4-176">Заканчивается время буфер после встречи для этой службы и перед следующим встречи клиента можно заранее.</span><span class="sxs-lookup"><span data-stu-id="d79f4-176">The time to buffer after an appointment for this service ends, and before the next customer appointment can be booked.</span></span>|
|<span data-ttu-id="d79f4-177">пребуфер</span><span class="sxs-lookup"><span data-stu-id="d79f4-177">preBuffer</span></span>|<span data-ttu-id="d79f4-178">Продолжительность</span><span class="sxs-lookup"><span data-stu-id="d79f4-178">Duration</span></span>|<span data-ttu-id="d79f4-179">Время для буфера до начала встречи для этой службы.</span><span class="sxs-lookup"><span data-stu-id="d79f4-179">The time to buffer before an appointment for this service can start.</span></span>|
|<span data-ttu-id="d79f4-180">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="d79f4-180">schedulingPolicy</span></span>|[<span data-ttu-id="d79f4-181">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="d79f4-181">bookingSchedulingPolicy</span></span>](../resources/bookingschedulingpolicy.md)|<span data-ttu-id="d79f4-182">Набор политик, определяющие порядок встреч для этого типа службы следует создания и управления.</span><span class="sxs-lookup"><span data-stu-id="d79f4-182">The set of policies that determine how appointments for this type of service should be created and managed.</span></span>|
|<span data-ttu-id="d79f4-183">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="d79f4-183">staffMemberIds</span></span>|<span data-ttu-id="d79f4-184">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d79f4-184">String collection</span></span>|<span data-ttu-id="d79f4-185">Представляет эти [Сотрудники](../resources/bookingstaffmember.md) , предоставляющих этой службы.</span><span class="sxs-lookup"><span data-stu-id="d79f4-185">Represents those [staff members](../resources/bookingstaffmember.md) who provide this service.</span></span> |

## <a name="response"></a><span data-ttu-id="d79f4-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="d79f4-186">Response</span></span>
<span data-ttu-id="d79f4-p108">При успешном выполнении этот метод возвращает код отклика `204 No content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d79f4-p108">If successful, this method returns a `204 No content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d79f4-189">Пример</span><span class="sxs-lookup"><span data-stu-id="d79f4-189">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d79f4-190">Запрос</span><span class="sxs-lookup"><span data-stu-id="d79f4-190">Request</span></span>
<span data-ttu-id="d79f4-191">В следующем примере обновляются длительность указанной службы.</span><span class="sxs-lookup"><span data-stu-id="d79f4-191">The following example updates the duration of the specified service.</span></span>
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
##### <a name="response"></a><span data-ttu-id="d79f4-192">Ответ</span><span class="sxs-lookup"><span data-stu-id="d79f4-192">Response</span></span>
<span data-ttu-id="d79f4-193">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d79f4-193">The following is an example of the response.</span></span> 
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
