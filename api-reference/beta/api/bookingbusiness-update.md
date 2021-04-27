---
title: Обновление bookingbusiness
description: Обновление свойств объекта bookingBusiness.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 767d4b3a355c74f6941bd9d9d20579e1c0dcda23
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047849"
---
# <a name="update-bookingbusiness"></a><span data-ttu-id="c0a04-103">Обновление bookingbusiness</span><span class="sxs-lookup"><span data-stu-id="c0a04-103">Update bookingbusiness</span></span>

<span data-ttu-id="c0a04-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0a04-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0a04-105">Обновление свойств объекта [bookingBusiness.](../resources/bookingbusiness.md)</span><span class="sxs-lookup"><span data-stu-id="c0a04-105">Update the properties of a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c0a04-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c0a04-106">Permissions</span></span>
<span data-ttu-id="c0a04-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0a04-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0a04-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c0a04-109">Permission type</span></span>      | <span data-ttu-id="c0a04-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c0a04-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0a04-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c0a04-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="c0a04-112">Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="c0a04-112">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="c0a04-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c0a04-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0a04-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0a04-114">Not supported.</span></span>   |
|<span data-ttu-id="c0a04-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c0a04-115">Application</span></span> | <span data-ttu-id="c0a04-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0a04-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="c0a04-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c0a04-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="c0a04-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c0a04-118">Optional request headers</span></span>
| <span data-ttu-id="c0a04-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c0a04-119">Name</span></span>       | <span data-ttu-id="c0a04-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c0a04-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c0a04-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c0a04-121">Authorization</span></span>  | <span data-ttu-id="c0a04-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c0a04-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0a04-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c0a04-123">Request body</span></span>
<span data-ttu-id="c0a04-p102">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="c0a04-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c0a04-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="c0a04-127">Property</span></span>     | <span data-ttu-id="c0a04-128">Тип</span><span class="sxs-lookup"><span data-stu-id="c0a04-128">Type</span></span>   |<span data-ttu-id="c0a04-129">Описание</span><span class="sxs-lookup"><span data-stu-id="c0a04-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c0a04-130">address</span><span class="sxs-lookup"><span data-stu-id="c0a04-130">address</span></span>|[<span data-ttu-id="c0a04-131">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="c0a04-131">physicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="c0a04-132">Адрес улицы бизнеса.</span><span class="sxs-lookup"><span data-stu-id="c0a04-132">The street address of the business.</span></span>|
|<span data-ttu-id="c0a04-133">businessHours</span><span class="sxs-lookup"><span data-stu-id="c0a04-133">businessHours</span></span>|<span data-ttu-id="c0a04-134">[коллекция bookingWorkHours](../resources/bookingworkhours.md)</span><span class="sxs-lookup"><span data-stu-id="c0a04-134">[bookingWorkHours](../resources/bookingworkhours.md) collection</span></span>|<span data-ttu-id="c0a04-135">Часы работы для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="c0a04-135">The hours of operation for the business.</span></span>|
|<span data-ttu-id="c0a04-136">businessType</span><span class="sxs-lookup"><span data-stu-id="c0a04-136">businessType</span></span>|<span data-ttu-id="c0a04-137">String</span><span class="sxs-lookup"><span data-stu-id="c0a04-137">String</span></span>|<span data-ttu-id="c0a04-138">Тип бизнеса.</span><span class="sxs-lookup"><span data-stu-id="c0a04-138">The type of business.</span></span>|
|<span data-ttu-id="c0a04-139">defaultCurrencyIso</span><span class="sxs-lookup"><span data-stu-id="c0a04-139">defaultCurrencyIso</span></span>|<span data-ttu-id="c0a04-140">String</span><span class="sxs-lookup"><span data-stu-id="c0a04-140">String</span></span>|<span data-ttu-id="c0a04-141">Код валюты, в которую бизнес работает в Microsoft Bookings.</span><span class="sxs-lookup"><span data-stu-id="c0a04-141">The code for the currency that the business operates in on Microsoft Bookings.</span></span>|
|<span data-ttu-id="c0a04-142">displayName</span><span class="sxs-lookup"><span data-stu-id="c0a04-142">displayName</span></span>|<span data-ttu-id="c0a04-143">String</span><span class="sxs-lookup"><span data-stu-id="c0a04-143">String</span></span>|<span data-ttu-id="c0a04-144">Имя для бизнеса, который взаимодействует с клиентами.</span><span class="sxs-lookup"><span data-stu-id="c0a04-144">A name for the business that interfaces with customers.</span></span>|
|<span data-ttu-id="c0a04-145">email</span><span class="sxs-lookup"><span data-stu-id="c0a04-145">email</span></span>|<span data-ttu-id="c0a04-146">String</span><span class="sxs-lookup"><span data-stu-id="c0a04-146">String</span></span>|<span data-ttu-id="c0a04-147">Адрес электронной почты для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="c0a04-147">The email address for the business.</span></span>|
|<span data-ttu-id="c0a04-148">phone</span><span class="sxs-lookup"><span data-stu-id="c0a04-148">phone</span></span>|<span data-ttu-id="c0a04-149">String</span><span class="sxs-lookup"><span data-stu-id="c0a04-149">String</span></span>|<span data-ttu-id="c0a04-150">Номер телефона для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="c0a04-150">The telephone number for the business.</span></span>|
|<span data-ttu-id="c0a04-151">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="c0a04-151">schedulingPolicy</span></span>|[<span data-ttu-id="c0a04-152">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="c0a04-152">bookingSchedulingPolicy</span></span>](../resources/bookingschedulingpolicy.md)|<span data-ttu-id="c0a04-153">Указывает, как можно создавать заказы для этого бизнеса.</span><span class="sxs-lookup"><span data-stu-id="c0a04-153">Specifies how bookings can be created for this business.</span></span>|
|<span data-ttu-id="c0a04-154">webSiteUrl</span><span class="sxs-lookup"><span data-stu-id="c0a04-154">webSiteUrl</span></span>|<span data-ttu-id="c0a04-155">String</span><span class="sxs-lookup"><span data-stu-id="c0a04-155">String</span></span>|<span data-ttu-id="c0a04-156">URL-адрес веб-сайта бизнеса.</span><span class="sxs-lookup"><span data-stu-id="c0a04-156">The URL of the business web site.</span></span>|

## <a name="response"></a><span data-ttu-id="c0a04-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0a04-157">Response</span></span>
<span data-ttu-id="c0a04-p103">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c0a04-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c0a04-160">Пример</span><span class="sxs-lookup"><span data-stu-id="c0a04-160">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c0a04-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="c0a04-161">Request</span></span>
<span data-ttu-id="c0a04-162">В следующем примере обновляется бизнес-адрес электронной почты и политика планирования, чтобы изменить интервал времени бронирования по умолчанию для бизнеса на час, а также предварительное бронирование до 30 дней.</span><span class="sxs-lookup"><span data-stu-id="c0a04-162">The following example updates the business email address and scheduling policy, to change the business default booking time slot to an hour, and advance booking up to 30 days.</span></span>

# <a name="http"></a>[<span data-ttu-id="c0a04-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="c0a04-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_bookingbusiness"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/fabrikam@M365B489948.onmicrosoft.com
Content-type: application/json

{
  "email": "admin@fabrikam.com",
  "schedulingPolicy": {
      "timeSlotInterval": "PT60M",
      "minimumLeadTime": "P1D",
      "maximumAdvance": "P30D",
      "sendConfirmationsToOwner": true,
      "allowStaffSelection": true
  }
}
```
# <a name="c"></a>[<span data-ttu-id="c0a04-164">C#</span><span class="sxs-lookup"><span data-stu-id="c0a04-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-bookingbusiness-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c0a04-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c0a04-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-bookingbusiness-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c0a04-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c0a04-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-bookingbusiness-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c0a04-167">Java</span><span class="sxs-lookup"><span data-stu-id="c0a04-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-bookingbusiness-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c0a04-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0a04-168">Response</span></span>
<span data-ttu-id="c0a04-169">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c0a04-169">The following is an example of the response.</span></span> <span data-ttu-id="c0a04-170">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c0a04-170">Note: The response object shown here might be shortened for readability.</span></span>
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
  "description": "Update bookingbusiness",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


