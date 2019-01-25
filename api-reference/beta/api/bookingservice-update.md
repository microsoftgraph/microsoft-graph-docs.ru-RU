---
title: Обновление bookingservice
description: Обновление свойства объекта bookingService в указанном bookingbusiness.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 6049fe68eaa45597246bef1c1b11952e3c4a5d42
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519719"
---
# <a name="update-bookingservice"></a><span data-ttu-id="4b425-103">Обновление bookingservice</span><span class="sxs-lookup"><span data-stu-id="4b425-103">Update bookingservice</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b425-104">Обновление свойства объекта [bookingService](../resources/bookingservice.md) в указанном [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="4b425-104">Update the properties of a [bookingService](../resources/bookingservice.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>

<span data-ttu-id="4b425-105">Ниже приведены некоторые примеры, которые можно настроить для службы:</span><span class="sxs-lookup"><span data-stu-id="4b425-105">The following are some examples you can customize for a service:</span></span>
- <span data-ttu-id="4b425-106">Price</span><span class="sxs-lookup"><span data-stu-id="4b425-106">Price</span></span>
- <span data-ttu-id="4b425-107">Типичная длина встречи</span><span class="sxs-lookup"><span data-stu-id="4b425-107">Typical length of an appointment</span></span>
- <span data-ttu-id="4b425-108">Reminders</span><span class="sxs-lookup"><span data-stu-id="4b425-108">Reminders</span></span>
- <span data-ttu-id="4b425-109">Любой буфер времени для настройки перед или завершить после службы</span><span class="sxs-lookup"><span data-stu-id="4b425-109">Any time buffer to set up before or finish up after the service</span></span>
- <span data-ttu-id="4b425-110">[Планирование политики](../resources/bookingschedulingpolicy.md) параметров, таких как минимальные уведомление о книги или отменить, и ли клиенты могут выбрать элементы определенного персонала для встречи.</span><span class="sxs-lookup"><span data-stu-id="4b425-110">[Scheduling policy](../resources/bookingschedulingpolicy.md) parameters such as minimum notice to book or cancel, and whether customers can select specific staff members for an appointment.</span></span>

## <a name="permissions"></a><span data-ttu-id="4b425-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4b425-111">Permissions</span></span>
<span data-ttu-id="4b425-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b425-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b425-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b425-114">Permission type</span></span>      | <span data-ttu-id="4b425-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b425-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b425-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b425-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="4b425-117">Bookings.ReadWrite.All Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="4b425-117">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="4b425-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b425-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b425-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b425-119">Not supported.</span></span>   |
|<span data-ttu-id="4b425-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4b425-120">Application</span></span> | <span data-ttu-id="4b425-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b425-121">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="4b425-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b425-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/services/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="4b425-123">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4b425-123">Optional request headers</span></span>
| <span data-ttu-id="4b425-124">Имя</span><span class="sxs-lookup"><span data-stu-id="4b425-124">Name</span></span>       | <span data-ttu-id="4b425-125">Описание</span><span class="sxs-lookup"><span data-stu-id="4b425-125">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="4b425-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b425-126">Authorization</span></span>  | <span data-ttu-id="4b425-127">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="4b425-127">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b425-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4b425-128">Request body</span></span>
<span data-ttu-id="4b425-p102">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="4b425-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4b425-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b425-132">Property</span></span>     | <span data-ttu-id="4b425-133">Тип</span><span class="sxs-lookup"><span data-stu-id="4b425-133">Type</span></span>   |<span data-ttu-id="4b425-134">Описание</span><span class="sxs-lookup"><span data-stu-id="4b425-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4b425-135">defaultDuration</span><span class="sxs-lookup"><span data-stu-id="4b425-135">defaultDuration</span></span>|<span data-ttu-id="4b425-136">Длительность</span><span class="sxs-lookup"><span data-stu-id="4b425-136">Duration</span></span>|<span data-ttu-id="4b425-137">Длина по умолчанию службы, представленный в числа дней, часов, минут и секунд.</span><span class="sxs-lookup"><span data-stu-id="4b425-137">The default length of the service, represented in numbers of days, hours, minutes, and seconds.</span></span> <span data-ttu-id="4b425-138">Например P11D23H59M59.999999999999S.</span><span class="sxs-lookup"><span data-stu-id="4b425-138">For example, P11D23H59M59.999999999999S.</span></span> |
|<span data-ttu-id="4b425-139">defaultLocation</span><span class="sxs-lookup"><span data-stu-id="4b425-139">defaultLocation</span></span>|[<span data-ttu-id="4b425-140">location</span><span class="sxs-lookup"><span data-stu-id="4b425-140">location</span></span>](../resources/location.md)|<span data-ttu-id="4b425-141">Физическое расположение по умолчанию для службы.</span><span class="sxs-lookup"><span data-stu-id="4b425-141">The default physical location for the service.</span></span>|
|<span data-ttu-id="4b425-142">defaultPrice</span><span class="sxs-lookup"><span data-stu-id="4b425-142">defaultPrice</span></span>|<span data-ttu-id="4b425-143">Double</span><span class="sxs-lookup"><span data-stu-id="4b425-143">Double</span></span>|<span data-ttu-id="4b425-144">Денежные Цена по умолчанию для службы.</span><span class="sxs-lookup"><span data-stu-id="4b425-144">The default monetary price for the service.</span></span>|
|<span data-ttu-id="4b425-145">defaultPriceType</span><span class="sxs-lookup"><span data-stu-id="4b425-145">defaultPriceType</span></span>|<span data-ttu-id="4b425-146">string</span><span class="sxs-lookup"><span data-stu-id="4b425-146">string</span></span>|<span data-ttu-id="4b425-147">По умолчанию способ службу оценивается.</span><span class="sxs-lookup"><span data-stu-id="4b425-147">The default way the service is charged.</span></span> <span data-ttu-id="4b425-148">Возможные значения: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="4b425-148">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="4b425-149">defaultReminders</span><span class="sxs-lookup"><span data-stu-id="4b425-149">defaultReminders</span></span>|<span data-ttu-id="4b425-150">[bookingReminder](../resources/bookingreminder.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="4b425-150">[bookingReminder](../resources/bookingreminder.md) collection</span></span>|<span data-ttu-id="4b425-151">Значение по умолчанию набора оповещения о встрече этой службы.</span><span class="sxs-lookup"><span data-stu-id="4b425-151">The default set of reminders for an appointment of this service.</span></span> <span data-ttu-id="4b425-152">Значение этого свойства доступна только при чтении этой **bookingService** по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="4b425-152">The value of this property is available only when reading this **bookingService** by its ID.</span></span>|
|<span data-ttu-id="4b425-153">description</span><span class="sxs-lookup"><span data-stu-id="4b425-153">description</span></span>|<span data-ttu-id="4b425-154">Строка</span><span class="sxs-lookup"><span data-stu-id="4b425-154">String</span></span>|<span data-ttu-id="4b425-155">Текстовое описание для службы.</span><span class="sxs-lookup"><span data-stu-id="4b425-155">A text description for the service.</span></span>|
|<span data-ttu-id="4b425-156">displayName</span><span class="sxs-lookup"><span data-stu-id="4b425-156">displayName</span></span>|<span data-ttu-id="4b425-157">String</span><span class="sxs-lookup"><span data-stu-id="4b425-157">String</span></span>|<span data-ttu-id="4b425-158">Имя службы.</span><span class="sxs-lookup"><span data-stu-id="4b425-158">A service name.</span></span>|
|<span data-ttu-id="4b425-159">emailAddress</span><span class="sxs-lookup"><span data-stu-id="4b425-159">emailAddress</span></span>|<span data-ttu-id="4b425-160">String</span><span class="sxs-lookup"><span data-stu-id="4b425-160">String</span></span>|<span data-ttu-id="4b425-161">Адрес электронной почты</span><span class="sxs-lookup"><span data-stu-id="4b425-161">An email address</span></span>|
|<span data-ttu-id="4b425-162">id</span><span class="sxs-lookup"><span data-stu-id="4b425-162">id</span></span>|<span data-ttu-id="4b425-163">String</span><span class="sxs-lookup"><span data-stu-id="4b425-163">String</span></span>| <span data-ttu-id="4b425-164">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4b425-164">Read-only.</span></span>|
|<span data-ttu-id="4b425-165">isHiddenFromCustomers</span><span class="sxs-lookup"><span data-stu-id="4b425-165">isHiddenFromCustomers</span></span>|<span data-ttu-id="4b425-166">Логическое</span><span class="sxs-lookup"><span data-stu-id="4b425-166">Boolean</span></span>|<span data-ttu-id="4b425-167">Значение true означает, что эта служба недоступна для клиентов для резервирования.</span><span class="sxs-lookup"><span data-stu-id="4b425-167">True means this service is not available to customers for booking.</span></span>|
|<span data-ttu-id="4b425-168">notes</span><span class="sxs-lookup"><span data-stu-id="4b425-168">notes</span></span>|<span data-ttu-id="4b425-169">String</span><span class="sxs-lookup"><span data-stu-id="4b425-169">String</span></span>|<span data-ttu-id="4b425-170">Дополнительные сведения об этой службы.</span><span class="sxs-lookup"><span data-stu-id="4b425-170">Additional information about this service.</span></span>|
|<span data-ttu-id="4b425-171">postBuffer</span><span class="sxs-lookup"><span data-stu-id="4b425-171">postBuffer</span></span>|<span data-ttu-id="4b425-172">Длительность</span><span class="sxs-lookup"><span data-stu-id="4b425-172">Duration</span></span>|<span data-ttu-id="4b425-173">Заканчивается время буфер после встречи для этой службы и перед следующим встречи клиента можно заранее.</span><span class="sxs-lookup"><span data-stu-id="4b425-173">The time to buffer after an appointment for this service ends, and before the next customer appointment can be booked.</span></span>|
|<span data-ttu-id="4b425-174">пребуфер</span><span class="sxs-lookup"><span data-stu-id="4b425-174">preBuffer</span></span>|<span data-ttu-id="4b425-175">Длительность</span><span class="sxs-lookup"><span data-stu-id="4b425-175">Duration</span></span>|<span data-ttu-id="4b425-176">Время для буфера до начала встречи для этой службы.</span><span class="sxs-lookup"><span data-stu-id="4b425-176">The time to buffer before an appointment for this service can start.</span></span>|
|<span data-ttu-id="4b425-177">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="4b425-177">schedulingPolicy</span></span>|[<span data-ttu-id="4b425-178">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="4b425-178">bookingSchedulingPolicy</span></span>](../resources/bookingschedulingpolicy.md)|<span data-ttu-id="4b425-179">Набор политик, определяющие порядок встреч для этого типа службы следует создания и управления.</span><span class="sxs-lookup"><span data-stu-id="4b425-179">The set of policies that determine how appointments for this type of service should be created and managed.</span></span>|
|<span data-ttu-id="4b425-180">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="4b425-180">staffMemberIds</span></span>|<span data-ttu-id="4b425-181">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4b425-181">String collection</span></span>|<span data-ttu-id="4b425-182">Представляет эти [Сотрудники](../resources/bookingstaffmember.md) , предоставляющих этой службы.</span><span class="sxs-lookup"><span data-stu-id="4b425-182">Represents those [staff members](../resources/bookingstaffmember.md) who provide this service.</span></span> |

## <a name="response"></a><span data-ttu-id="4b425-183">Ответ</span><span class="sxs-lookup"><span data-stu-id="4b425-183">Response</span></span>
<span data-ttu-id="4b425-p106">При успешном выполнении этот метод возвращает код отклика `204 No content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4b425-p106">If successful, this method returns a `204 No content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4b425-186">Пример</span><span class="sxs-lookup"><span data-stu-id="4b425-186">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4b425-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b425-187">Request</span></span>
<span data-ttu-id="4b425-188">В следующем примере обновляются длительность указанной службы.</span><span class="sxs-lookup"><span data-stu-id="4b425-188">The following example updates the duration of the specified service.</span></span>
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
##### <a name="response"></a><span data-ttu-id="4b425-189">Ответ</span><span class="sxs-lookup"><span data-stu-id="4b425-189">Response</span></span>
<span data-ttu-id="4b425-190">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4b425-190">The following is an example of the response.</span></span>
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
    "Error: /api-reference/beta/api/bookingservice-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
