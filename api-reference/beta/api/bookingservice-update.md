---
title: Обновление букингсервице
description: Обновление свойств объекта Букингсервице в указанном букингбусинесс.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 49a775e542dba518d382b6999def6aa5795861a8
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865275"
---
# <a name="update-bookingservice"></a><span data-ttu-id="0ec44-103">Обновление букингсервице</span><span class="sxs-lookup"><span data-stu-id="0ec44-103">Update bookingservice</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ec44-104">Обновление свойств объекта [букингсервице](../resources/bookingservice.md) в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="0ec44-104">Update the properties of a [bookingService](../resources/bookingservice.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>

<span data-ttu-id="0ec44-105">Ниже приведено несколько примеров, которые можно настроить для службы.</span><span class="sxs-lookup"><span data-stu-id="0ec44-105">The following are some examples you can customize for a service:</span></span>
- <span data-ttu-id="0ec44-106">ЦЕНА</span><span class="sxs-lookup"><span data-stu-id="0ec44-106">Price</span></span>
- <span data-ttu-id="0ec44-107">Типичная длительность встречи</span><span class="sxs-lookup"><span data-stu-id="0ec44-107">Typical length of an appointment</span></span>
- <span data-ttu-id="0ec44-108">Reminders</span><span class="sxs-lookup"><span data-stu-id="0ec44-108">Reminders</span></span>
- <span data-ttu-id="0ec44-109">Любой буфер, который должен быть настроен до или окончание срока выполнения службы</span><span class="sxs-lookup"><span data-stu-id="0ec44-109">Any time buffer to set up before or finish up after the service</span></span>
- <span data-ttu-id="0ec44-110">[Планирование](../resources/bookingschedulingpolicy.md) таких параметров политики, как минимальное уведомление о книге или Отмена, а также возможность выбора определенных сотрудников для встречи пользователями.</span><span class="sxs-lookup"><span data-stu-id="0ec44-110">[Scheduling policy](../resources/bookingschedulingpolicy.md) parameters such as minimum notice to book or cancel, and whether customers can select specific staff members for an appointment.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ec44-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0ec44-111">Permissions</span></span>
<span data-ttu-id="0ec44-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ec44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ec44-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ec44-114">Permission type</span></span>      | <span data-ttu-id="0ec44-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ec44-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ec44-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ec44-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="0ec44-117">Резервирования. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="0ec44-117">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="0ec44-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ec44-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ec44-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ec44-119">Not supported.</span></span>   |
|<span data-ttu-id="0ec44-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0ec44-120">Application</span></span> | <span data-ttu-id="0ec44-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ec44-121">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="0ec44-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ec44-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/services/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="0ec44-123">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0ec44-123">Optional request headers</span></span>
| <span data-ttu-id="0ec44-124">Имя</span><span class="sxs-lookup"><span data-stu-id="0ec44-124">Name</span></span>       | <span data-ttu-id="0ec44-125">Описание</span><span class="sxs-lookup"><span data-stu-id="0ec44-125">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0ec44-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0ec44-126">Authorization</span></span>  | <span data-ttu-id="0ec44-127">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="0ec44-127">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ec44-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0ec44-128">Request body</span></span>
<span data-ttu-id="0ec44-p102">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="0ec44-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0ec44-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="0ec44-132">Property</span></span>     | <span data-ttu-id="0ec44-133">Тип</span><span class="sxs-lookup"><span data-stu-id="0ec44-133">Type</span></span>   |<span data-ttu-id="0ec44-134">Описание</span><span class="sxs-lookup"><span data-stu-id="0ec44-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0ec44-135">Дефаултдуратион</span><span class="sxs-lookup"><span data-stu-id="0ec44-135">defaultDuration</span></span>|<span data-ttu-id="0ec44-136">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="0ec44-136">Duration</span></span>|<span data-ttu-id="0ec44-137">Длина службы по умолчанию, представленная в виде числа дней, часов, минут и секунд.</span><span class="sxs-lookup"><span data-stu-id="0ec44-137">The default length of the service, represented in numbers of days, hours, minutes, and seconds.</span></span> <span data-ttu-id="0ec44-138">Например, P11D23H59M 59.999999999999 S.</span><span class="sxs-lookup"><span data-stu-id="0ec44-138">For example, P11D23H59M59.999999999999S.</span></span> |
|<span data-ttu-id="0ec44-139">defaultLocation</span><span class="sxs-lookup"><span data-stu-id="0ec44-139">defaultLocation</span></span>|[<span data-ttu-id="0ec44-140">location</span><span class="sxs-lookup"><span data-stu-id="0ec44-140">location</span></span>](../resources/location.md)|<span data-ttu-id="0ec44-141">Физическое расположение службы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="0ec44-141">The default physical location for the service.</span></span>|
|<span data-ttu-id="0ec44-142">Дефаултприце</span><span class="sxs-lookup"><span data-stu-id="0ec44-142">defaultPrice</span></span>|<span data-ttu-id="0ec44-143">Двойное</span><span class="sxs-lookup"><span data-stu-id="0ec44-143">Double</span></span>|<span data-ttu-id="0ec44-144">Денежная Цена по умолчанию для службы.</span><span class="sxs-lookup"><span data-stu-id="0ec44-144">The default monetary price for the service.</span></span>|
|<span data-ttu-id="0ec44-145">Дефаултприцетипе</span><span class="sxs-lookup"><span data-stu-id="0ec44-145">defaultPriceType</span></span>|<span data-ttu-id="0ec44-146">string</span><span class="sxs-lookup"><span data-stu-id="0ec44-146">string</span></span>|<span data-ttu-id="0ec44-147">Способ оплаты службы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="0ec44-147">The default way the service is charged.</span></span> <span data-ttu-id="0ec44-148">Возможные значения: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="0ec44-148">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="0ec44-149">Дефаултреминдерс</span><span class="sxs-lookup"><span data-stu-id="0ec44-149">defaultReminders</span></span>|<span data-ttu-id="0ec44-150">Коллекция [букингреминдер](../resources/bookingreminder.md)</span><span class="sxs-lookup"><span data-stu-id="0ec44-150">[bookingReminder](../resources/bookingreminder.md) collection</span></span>|<span data-ttu-id="0ec44-151">Набор напоминаний по умолчанию для встречи этой службы.</span><span class="sxs-lookup"><span data-stu-id="0ec44-151">The default set of reminders for an appointment of this service.</span></span> <span data-ttu-id="0ec44-152">Значение этого свойства доступно только при чтении этого **букингсервице** с помощью идентификатора.</span><span class="sxs-lookup"><span data-stu-id="0ec44-152">The value of this property is available only when reading this **bookingService** by its ID.</span></span>|
|<span data-ttu-id="0ec44-153">description</span><span class="sxs-lookup"><span data-stu-id="0ec44-153">description</span></span>|<span data-ttu-id="0ec44-154">String</span><span class="sxs-lookup"><span data-stu-id="0ec44-154">String</span></span>|<span data-ttu-id="0ec44-155">Текстовое описание службы.</span><span class="sxs-lookup"><span data-stu-id="0ec44-155">A text description for the service.</span></span>|
|<span data-ttu-id="0ec44-156">displayName</span><span class="sxs-lookup"><span data-stu-id="0ec44-156">displayName</span></span>|<span data-ttu-id="0ec44-157">Строка</span><span class="sxs-lookup"><span data-stu-id="0ec44-157">String</span></span>|<span data-ttu-id="0ec44-158">Имя службы.</span><span class="sxs-lookup"><span data-stu-id="0ec44-158">A service name.</span></span>|
|<span data-ttu-id="0ec44-159">emailAddress</span><span class="sxs-lookup"><span data-stu-id="0ec44-159">emailAddress</span></span>|<span data-ttu-id="0ec44-160">String</span><span class="sxs-lookup"><span data-stu-id="0ec44-160">String</span></span>|<span data-ttu-id="0ec44-161">Адрес электронной почты</span><span class="sxs-lookup"><span data-stu-id="0ec44-161">An email address</span></span>|
|<span data-ttu-id="0ec44-162">id</span><span class="sxs-lookup"><span data-stu-id="0ec44-162">id</span></span>|<span data-ttu-id="0ec44-163">String</span><span class="sxs-lookup"><span data-stu-id="0ec44-163">String</span></span>| <span data-ttu-id="0ec44-164">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0ec44-164">Read-only.</span></span>|
|<span data-ttu-id="0ec44-165">Ишидденфромкустомерс</span><span class="sxs-lookup"><span data-stu-id="0ec44-165">isHiddenFromCustomers</span></span>|<span data-ttu-id="0ec44-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ec44-166">Boolean</span></span>|<span data-ttu-id="0ec44-167">Значение true означает, что эта служба недоступна клиентам для резервирования.</span><span class="sxs-lookup"><span data-stu-id="0ec44-167">True means this service is not available to customers for booking.</span></span>|
|<span data-ttu-id="0ec44-168">notes</span><span class="sxs-lookup"><span data-stu-id="0ec44-168">notes</span></span>|<span data-ttu-id="0ec44-169">String</span><span class="sxs-lookup"><span data-stu-id="0ec44-169">String</span></span>|<span data-ttu-id="0ec44-170">Дополнительные сведения об этой службе.</span><span class="sxs-lookup"><span data-stu-id="0ec44-170">Additional information about this service.</span></span>|
|<span data-ttu-id="0ec44-171">Буфер буфера</span><span class="sxs-lookup"><span data-stu-id="0ec44-171">postBuffer</span></span>|<span data-ttu-id="0ec44-172">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="0ec44-172">Duration</span></span>|<span data-ttu-id="0ec44-173">Время, в течение которого помещается в буфер после встречи для этой службы и до того, как может быть зарезервирована Следующая встреча покупателя.</span><span class="sxs-lookup"><span data-stu-id="0ec44-173">The time to buffer after an appointment for this service ends, and before the next customer appointment can be booked.</span></span>|
|<span data-ttu-id="0ec44-174">пребуфер</span><span class="sxs-lookup"><span data-stu-id="0ec44-174">preBuffer</span></span>|<span data-ttu-id="0ec44-175">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="0ec44-175">Duration</span></span>|<span data-ttu-id="0ec44-176">Время, в течение которого будет помещено в буфер, прежде чем можно будет запустить встречу для этой службы.</span><span class="sxs-lookup"><span data-stu-id="0ec44-176">The time to buffer before an appointment for this service can start.</span></span>|
|<span data-ttu-id="0ec44-177">Счедулингполици</span><span class="sxs-lookup"><span data-stu-id="0ec44-177">schedulingPolicy</span></span>|[<span data-ttu-id="0ec44-178">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="0ec44-178">bookingSchedulingPolicy</span></span>](../resources/bookingschedulingpolicy.md)|<span data-ttu-id="0ec44-179">Набор политик, определяющих, как должны создаваться встречи для этого типа службы и управлять ими.</span><span class="sxs-lookup"><span data-stu-id="0ec44-179">The set of policies that determine how appointments for this type of service should be created and managed.</span></span>|
|<span data-ttu-id="0ec44-180">Стаффмемберидс</span><span class="sxs-lookup"><span data-stu-id="0ec44-180">staffMemberIds</span></span>|<span data-ttu-id="0ec44-181">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="0ec44-181">String collection</span></span>|<span data-ttu-id="0ec44-182">Представляет [сотрудников](../resources/bookingstaffmember.md) , которые предоставляют эту службу.</span><span class="sxs-lookup"><span data-stu-id="0ec44-182">Represents those [staff members](../resources/bookingstaffmember.md) who provide this service.</span></span> |

## <a name="response"></a><span data-ttu-id="0ec44-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ec44-183">Response</span></span>
<span data-ttu-id="0ec44-p106">При успешном выполнении этот метод возвращает код отклика `204 No content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0ec44-p106">If successful, this method returns a `204 No content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0ec44-186">Пример</span><span class="sxs-lookup"><span data-stu-id="0ec44-186">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0ec44-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ec44-187">Request</span></span>
<span data-ttu-id="0ec44-188">В следующем примере обновляется длительность указанной службы.</span><span class="sxs-lookup"><span data-stu-id="0ec44-188">The following example updates the duration of the specified service.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0ec44-189">HTTP</span><span class="sxs-lookup"><span data-stu-id="0ec44-189">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="0ec44-190">C#</span><span class="sxs-lookup"><span data-stu-id="0ec44-190">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-bookingservice-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0ec44-191">Javascript</span><span class="sxs-lookup"><span data-stu-id="0ec44-191">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-bookingservice-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0ec44-192">Цель — C</span><span class="sxs-lookup"><span data-stu-id="0ec44-192">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-bookingservice-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0ec44-193">Java</span><span class="sxs-lookup"><span data-stu-id="0ec44-193">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-bookingservice-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0ec44-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ec44-194">Response</span></span>
<span data-ttu-id="0ec44-195">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0ec44-195">The following is an example of the response.</span></span>
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
