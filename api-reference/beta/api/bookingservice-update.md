---
title: Обновление букингсервице
description: Обновление свойств объекта Букингсервице в указанном букингбусинесс.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 9e8eec740df193662c10a5ff9557fa3dafa30753
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48960376"
---
# <a name="update-bookingservice"></a><span data-ttu-id="60b1d-103">Обновление букингсервице</span><span class="sxs-lookup"><span data-stu-id="60b1d-103">Update bookingservice</span></span>

<span data-ttu-id="60b1d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60b1d-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60b1d-105">Обновление свойств объекта [букингсервице](../resources/bookingservice.md) в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="60b1d-105">Update the properties of a [bookingService](../resources/bookingservice.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>

<span data-ttu-id="60b1d-106">Ниже приведено несколько примеров, которые можно настроить для службы.</span><span class="sxs-lookup"><span data-stu-id="60b1d-106">The following are some examples you can customize for a service:</span></span>
- <span data-ttu-id="60b1d-107">ЦЕНА</span><span class="sxs-lookup"><span data-stu-id="60b1d-107">Price</span></span>
- <span data-ttu-id="60b1d-108">Типичная длительность встречи</span><span class="sxs-lookup"><span data-stu-id="60b1d-108">Typical length of an appointment</span></span>
- <span data-ttu-id="60b1d-109">Reminders</span><span class="sxs-lookup"><span data-stu-id="60b1d-109">Reminders</span></span>
- <span data-ttu-id="60b1d-110">Любой буфер, который должен быть настроен до или окончание срока выполнения службы</span><span class="sxs-lookup"><span data-stu-id="60b1d-110">Any time buffer to set up before or finish up after the service</span></span>
- <span data-ttu-id="60b1d-111">[Планирование](../resources/bookingschedulingpolicy.md) таких параметров политики, как минимальное уведомление о книге или Отмена, а также возможность выбора определенных сотрудников для встречи пользователями.</span><span class="sxs-lookup"><span data-stu-id="60b1d-111">[Scheduling policy](../resources/bookingschedulingpolicy.md) parameters such as minimum notice to book or cancel, and whether customers can select specific staff members for an appointment.</span></span>

## <a name="permissions"></a><span data-ttu-id="60b1d-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="60b1d-112">Permissions</span></span>
<span data-ttu-id="60b1d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60b1d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60b1d-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="60b1d-115">Permission type</span></span>      | <span data-ttu-id="60b1d-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="60b1d-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60b1d-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="60b1d-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="60b1d-118">Резервирования. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="60b1d-118">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="60b1d-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="60b1d-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60b1d-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60b1d-120">Not supported.</span></span>   |
|<span data-ttu-id="60b1d-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="60b1d-121">Application</span></span> | <span data-ttu-id="60b1d-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60b1d-122">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="60b1d-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="60b1d-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/services/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="60b1d-124">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="60b1d-124">Optional request headers</span></span>
| <span data-ttu-id="60b1d-125">Имя</span><span class="sxs-lookup"><span data-stu-id="60b1d-125">Name</span></span>       | <span data-ttu-id="60b1d-126">Описание</span><span class="sxs-lookup"><span data-stu-id="60b1d-126">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="60b1d-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="60b1d-127">Authorization</span></span>  | <span data-ttu-id="60b1d-128">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="60b1d-128">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="60b1d-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="60b1d-129">Request body</span></span>
<span data-ttu-id="60b1d-p102">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="60b1d-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="60b1d-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="60b1d-133">Property</span></span>     | <span data-ttu-id="60b1d-134">Тип</span><span class="sxs-lookup"><span data-stu-id="60b1d-134">Type</span></span>   |<span data-ttu-id="60b1d-135">Описание</span><span class="sxs-lookup"><span data-stu-id="60b1d-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="60b1d-136">дефаултдуратион</span><span class="sxs-lookup"><span data-stu-id="60b1d-136">defaultDuration</span></span>|<span data-ttu-id="60b1d-137">Длительность</span><span class="sxs-lookup"><span data-stu-id="60b1d-137">Duration</span></span>|<span data-ttu-id="60b1d-138">Длина службы по умолчанию, представленная в виде числа дней, часов, минут и секунд.</span><span class="sxs-lookup"><span data-stu-id="60b1d-138">The default length of the service, represented in numbers of days, hours, minutes, and seconds.</span></span> <span data-ttu-id="60b1d-139">Например, P11D23H59M 59.999999999999 S.</span><span class="sxs-lookup"><span data-stu-id="60b1d-139">For example, P11D23H59M59.999999999999S.</span></span> |
|<span data-ttu-id="60b1d-140">defaultLocation</span><span class="sxs-lookup"><span data-stu-id="60b1d-140">defaultLocation</span></span>|[<span data-ttu-id="60b1d-141">location</span><span class="sxs-lookup"><span data-stu-id="60b1d-141">location</span></span>](../resources/location.md)|<span data-ttu-id="60b1d-142">Физическое расположение службы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="60b1d-142">The default physical location for the service.</span></span>|
|<span data-ttu-id="60b1d-143">дефаултприце</span><span class="sxs-lookup"><span data-stu-id="60b1d-143">defaultPrice</span></span>|<span data-ttu-id="60b1d-144">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="60b1d-144">Double</span></span>|<span data-ttu-id="60b1d-145">Денежная Цена по умолчанию для службы.</span><span class="sxs-lookup"><span data-stu-id="60b1d-145">The default monetary price for the service.</span></span>|
|<span data-ttu-id="60b1d-146">дефаултприцетипе</span><span class="sxs-lookup"><span data-stu-id="60b1d-146">defaultPriceType</span></span>|<span data-ttu-id="60b1d-147">string</span><span class="sxs-lookup"><span data-stu-id="60b1d-147">string</span></span>|<span data-ttu-id="60b1d-148">Способ оплаты службы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="60b1d-148">The default way the service is charged.</span></span> <span data-ttu-id="60b1d-149">Возможные значения: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="60b1d-149">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="60b1d-150">дефаултреминдерс</span><span class="sxs-lookup"><span data-stu-id="60b1d-150">defaultReminders</span></span>|<span data-ttu-id="60b1d-151">Коллекция [букингреминдер](../resources/bookingreminder.md)</span><span class="sxs-lookup"><span data-stu-id="60b1d-151">[bookingReminder](../resources/bookingreminder.md) collection</span></span>|<span data-ttu-id="60b1d-152">Набор напоминаний по умолчанию для встречи этой службы.</span><span class="sxs-lookup"><span data-stu-id="60b1d-152">The default set of reminders for an appointment of this service.</span></span> <span data-ttu-id="60b1d-153">Значение этого свойства доступно только при чтении этого **букингсервице** с помощью идентификатора.</span><span class="sxs-lookup"><span data-stu-id="60b1d-153">The value of this property is available only when reading this **bookingService** by its ID.</span></span>|
|<span data-ttu-id="60b1d-154">description</span><span class="sxs-lookup"><span data-stu-id="60b1d-154">description</span></span>|<span data-ttu-id="60b1d-155">String</span><span class="sxs-lookup"><span data-stu-id="60b1d-155">String</span></span>|<span data-ttu-id="60b1d-156">Текстовое описание службы.</span><span class="sxs-lookup"><span data-stu-id="60b1d-156">A text description for the service.</span></span>|
|<span data-ttu-id="60b1d-157">displayName</span><span class="sxs-lookup"><span data-stu-id="60b1d-157">displayName</span></span>|<span data-ttu-id="60b1d-158">String</span><span class="sxs-lookup"><span data-stu-id="60b1d-158">String</span></span>|<span data-ttu-id="60b1d-159">Имя службы.</span><span class="sxs-lookup"><span data-stu-id="60b1d-159">A service name.</span></span>|
|<span data-ttu-id="60b1d-160">emailAddress</span><span class="sxs-lookup"><span data-stu-id="60b1d-160">emailAddress</span></span>|<span data-ttu-id="60b1d-161">String</span><span class="sxs-lookup"><span data-stu-id="60b1d-161">String</span></span>|<span data-ttu-id="60b1d-162">Адрес электронной почты</span><span class="sxs-lookup"><span data-stu-id="60b1d-162">An email address</span></span>|
|<span data-ttu-id="60b1d-163">id</span><span class="sxs-lookup"><span data-stu-id="60b1d-163">id</span></span>|<span data-ttu-id="60b1d-164">String</span><span class="sxs-lookup"><span data-stu-id="60b1d-164">String</span></span>| <span data-ttu-id="60b1d-165">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="60b1d-165">Read-only.</span></span>|
|<span data-ttu-id="60b1d-166">ишидденфромкустомерс</span><span class="sxs-lookup"><span data-stu-id="60b1d-166">isHiddenFromCustomers</span></span>|<span data-ttu-id="60b1d-167">Логический</span><span class="sxs-lookup"><span data-stu-id="60b1d-167">Boolean</span></span>|<span data-ttu-id="60b1d-168">Значение true означает, что эта служба недоступна клиентам для резервирования.</span><span class="sxs-lookup"><span data-stu-id="60b1d-168">True means this service is not available to customers for booking.</span></span>|
|<span data-ttu-id="60b1d-169">notes</span><span class="sxs-lookup"><span data-stu-id="60b1d-169">notes</span></span>|<span data-ttu-id="60b1d-170">String</span><span class="sxs-lookup"><span data-stu-id="60b1d-170">String</span></span>|<span data-ttu-id="60b1d-171">Дополнительные сведения об этой службе.</span><span class="sxs-lookup"><span data-stu-id="60b1d-171">Additional information about this service.</span></span>|
|<span data-ttu-id="60b1d-172">Буфер буфера</span><span class="sxs-lookup"><span data-stu-id="60b1d-172">postBuffer</span></span>|<span data-ttu-id="60b1d-173">Длительность</span><span class="sxs-lookup"><span data-stu-id="60b1d-173">Duration</span></span>|<span data-ttu-id="60b1d-174">Время, в течение которого помещается в буфер после встречи для этой службы и до того, как может быть зарезервирована Следующая встреча покупателя.</span><span class="sxs-lookup"><span data-stu-id="60b1d-174">The time to buffer after an appointment for this service ends, and before the next customer appointment can be booked.</span></span>|
|<span data-ttu-id="60b1d-175">пребуфер</span><span class="sxs-lookup"><span data-stu-id="60b1d-175">preBuffer</span></span>|<span data-ttu-id="60b1d-176">Длительность</span><span class="sxs-lookup"><span data-stu-id="60b1d-176">Duration</span></span>|<span data-ttu-id="60b1d-177">Время, в течение которого будет помещено в буфер, прежде чем можно будет запустить встречу для этой службы.</span><span class="sxs-lookup"><span data-stu-id="60b1d-177">The time to buffer before an appointment for this service can start.</span></span>|
|<span data-ttu-id="60b1d-178">счедулингполици</span><span class="sxs-lookup"><span data-stu-id="60b1d-178">schedulingPolicy</span></span>|[<span data-ttu-id="60b1d-179">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="60b1d-179">bookingSchedulingPolicy</span></span>](../resources/bookingschedulingpolicy.md)|<span data-ttu-id="60b1d-180">Набор политик, определяющих, как должны создаваться встречи для этого типа службы и управлять ими.</span><span class="sxs-lookup"><span data-stu-id="60b1d-180">The set of policies that determine how appointments for this type of service should be created and managed.</span></span>|
|<span data-ttu-id="60b1d-181">стаффмемберидс</span><span class="sxs-lookup"><span data-stu-id="60b1d-181">staffMemberIds</span></span>|<span data-ttu-id="60b1d-182">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="60b1d-182">String collection</span></span>|<span data-ttu-id="60b1d-183">Представляет [сотрудников](../resources/bookingstaffmember.md) , которые предоставляют эту службу.</span><span class="sxs-lookup"><span data-stu-id="60b1d-183">Represents those [staff members](../resources/bookingstaffmember.md) who provide this service.</span></span> |

## <a name="response"></a><span data-ttu-id="60b1d-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="60b1d-184">Response</span></span>
<span data-ttu-id="60b1d-p106">При успешном выполнении этот метод возвращает код отклика `204 No content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="60b1d-p106">If successful, this method returns a `204 No content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="60b1d-187">Пример</span><span class="sxs-lookup"><span data-stu-id="60b1d-187">Example</span></span>
##### <a name="request"></a><span data-ttu-id="60b1d-188">Запрос</span><span class="sxs-lookup"><span data-stu-id="60b1d-188">Request</span></span>
<span data-ttu-id="60b1d-189">В следующем примере обновляется длительность указанной службы.</span><span class="sxs-lookup"><span data-stu-id="60b1d-189">The following example updates the duration of the specified service.</span></span>

# <a name="http"></a>[<span data-ttu-id="60b1d-190">HTTP</span><span class="sxs-lookup"><span data-stu-id="60b1d-190">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="60b1d-191">C#</span><span class="sxs-lookup"><span data-stu-id="60b1d-191">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-bookingservice-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="60b1d-192">JavaScript</span><span class="sxs-lookup"><span data-stu-id="60b1d-192">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-bookingservice-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="60b1d-193">Objective-C</span><span class="sxs-lookup"><span data-stu-id="60b1d-193">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-bookingservice-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="60b1d-194">Java</span><span class="sxs-lookup"><span data-stu-id="60b1d-194">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-bookingservice-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="60b1d-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="60b1d-195">Response</span></span>
<span data-ttu-id="60b1d-196">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="60b1d-196">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update bookingservice",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


