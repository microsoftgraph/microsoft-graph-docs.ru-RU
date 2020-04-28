---
title: Обновление букингбусинесс
description: Обновление свойств объекта Букингбусинесс.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: b820d65a50b2a07bd1c3e95936bc6ee304f20d96
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43376606"
---
# <a name="update-bookingbusiness"></a><span data-ttu-id="1f0a6-103">Обновление букингбусинесс</span><span class="sxs-lookup"><span data-stu-id="1f0a6-103">Update bookingbusiness</span></span>

<span data-ttu-id="1f0a6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f0a6-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f0a6-105">Обновление свойств объекта [букингбусинесс](../resources/bookingbusiness.md) .</span><span class="sxs-lookup"><span data-stu-id="1f0a6-105">Update the properties of a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1f0a6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1f0a6-106">Permissions</span></span>
<span data-ttu-id="1f0a6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f0a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f0a6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1f0a6-109">Permission type</span></span>      | <span data-ttu-id="1f0a6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1f0a6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f0a6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1f0a6-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="1f0a6-112">Резервирования. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="1f0a6-112">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="1f0a6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1f0a6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f0a6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f0a6-114">Not supported.</span></span>   |
|<span data-ttu-id="1f0a6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1f0a6-115">Application</span></span> | <span data-ttu-id="1f0a6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f0a6-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="1f0a6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1f0a6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="1f0a6-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1f0a6-118">Optional request headers</span></span>
| <span data-ttu-id="1f0a6-119">Имя</span><span class="sxs-lookup"><span data-stu-id="1f0a6-119">Name</span></span>       | <span data-ttu-id="1f0a6-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1f0a6-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="1f0a6-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1f0a6-121">Authorization</span></span>  | <span data-ttu-id="1f0a6-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="1f0a6-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f0a6-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1f0a6-123">Request body</span></span>
<span data-ttu-id="1f0a6-p102">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="1f0a6-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1f0a6-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="1f0a6-127">Property</span></span>     | <span data-ttu-id="1f0a6-128">Тип</span><span class="sxs-lookup"><span data-stu-id="1f0a6-128">Type</span></span>   |<span data-ttu-id="1f0a6-129">Описание</span><span class="sxs-lookup"><span data-stu-id="1f0a6-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1f0a6-130">address</span><span class="sxs-lookup"><span data-stu-id="1f0a6-130">address</span></span>|[<span data-ttu-id="1f0a6-131">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="1f0a6-131">physicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="1f0a6-132">Адрес в почтовом ящике организации.</span><span class="sxs-lookup"><span data-stu-id="1f0a6-132">The street address of the business.</span></span>|
|<span data-ttu-id="1f0a6-133">businessHours</span><span class="sxs-lookup"><span data-stu-id="1f0a6-133">businessHours</span></span>|<span data-ttu-id="1f0a6-134">Коллекция [букингворкхаурс](../resources/bookingworkhours.md)</span><span class="sxs-lookup"><span data-stu-id="1f0a6-134">[bookingWorkHours](../resources/bookingworkhours.md) collection</span></span>|<span data-ttu-id="1f0a6-135">Количество часов работы для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="1f0a6-135">The hours of operation for the business.</span></span>|
|<span data-ttu-id="1f0a6-136">бусинесстипе</span><span class="sxs-lookup"><span data-stu-id="1f0a6-136">businessType</span></span>|<span data-ttu-id="1f0a6-137">String</span><span class="sxs-lookup"><span data-stu-id="1f0a6-137">String</span></span>|<span data-ttu-id="1f0a6-138">Тип бизнеса.</span><span class="sxs-lookup"><span data-stu-id="1f0a6-138">The type of business.</span></span>|
|<span data-ttu-id="1f0a6-139">дефаулткурренциисо</span><span class="sxs-lookup"><span data-stu-id="1f0a6-139">defaultCurrencyIso</span></span>|<span data-ttu-id="1f0a6-140">String</span><span class="sxs-lookup"><span data-stu-id="1f0a6-140">String</span></span>|<span data-ttu-id="1f0a6-141">Код валюты, в которой работает предприятие, в Microsoft Books.</span><span class="sxs-lookup"><span data-stu-id="1f0a6-141">The code for the currency that the business operates in on Microsoft Bookings.</span></span>|
|<span data-ttu-id="1f0a6-142">displayName</span><span class="sxs-lookup"><span data-stu-id="1f0a6-142">displayName</span></span>|<span data-ttu-id="1f0a6-143">Строка</span><span class="sxs-lookup"><span data-stu-id="1f0a6-143">String</span></span>|<span data-ttu-id="1f0a6-144">Название организации, которая взаимодействует с клиентами.</span><span class="sxs-lookup"><span data-stu-id="1f0a6-144">A name for the business that interfaces with customers.</span></span>|
|<span data-ttu-id="1f0a6-145">email</span><span class="sxs-lookup"><span data-stu-id="1f0a6-145">email</span></span>|<span data-ttu-id="1f0a6-146">String</span><span class="sxs-lookup"><span data-stu-id="1f0a6-146">String</span></span>|<span data-ttu-id="1f0a6-147">Адрес электронной почты для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="1f0a6-147">The email address for the business.</span></span>|
|<span data-ttu-id="1f0a6-148">phone</span><span class="sxs-lookup"><span data-stu-id="1f0a6-148">phone</span></span>|<span data-ttu-id="1f0a6-149">String</span><span class="sxs-lookup"><span data-stu-id="1f0a6-149">String</span></span>|<span data-ttu-id="1f0a6-150">Номер телефона для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="1f0a6-150">The telephone number for the business.</span></span>|
|<span data-ttu-id="1f0a6-151">счедулингполици</span><span class="sxs-lookup"><span data-stu-id="1f0a6-151">schedulingPolicy</span></span>|[<span data-ttu-id="1f0a6-152">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="1f0a6-152">bookingSchedulingPolicy</span></span>](../resources/bookingschedulingpolicy.md)|<span data-ttu-id="1f0a6-153">Указывает, как можно создавать резервирования для этого бизнеса.</span><span class="sxs-lookup"><span data-stu-id="1f0a6-153">Specifies how bookings can be created for this business.</span></span>|
|<span data-ttu-id="1f0a6-154">вебситеурл</span><span class="sxs-lookup"><span data-stu-id="1f0a6-154">webSiteUrl</span></span>|<span data-ttu-id="1f0a6-155">String</span><span class="sxs-lookup"><span data-stu-id="1f0a6-155">String</span></span>|<span data-ttu-id="1f0a6-156">URL-адрес веб-сайта компании.</span><span class="sxs-lookup"><span data-stu-id="1f0a6-156">The URL of the business web site.</span></span>|

## <a name="response"></a><span data-ttu-id="1f0a6-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f0a6-157">Response</span></span>
<span data-ttu-id="1f0a6-p103">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1f0a6-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1f0a6-160">Пример</span><span class="sxs-lookup"><span data-stu-id="1f0a6-160">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1f0a6-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f0a6-161">Request</span></span>
<span data-ttu-id="1f0a6-162">В следующем примере показано, как обновить адрес электронной почты и политику планирования, чтобы изменить период резервирования по умолчанию для бизнеса на час, а затем выполнить резервное резервирование в течение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="1f0a6-162">The following example updates the business email address and scheduling policy, to change the business default booking time slot to an hour, and advance booking up to 30 days.</span></span>

# <a name="http"></a>[<span data-ttu-id="1f0a6-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="1f0a6-163">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="1f0a6-164">C#</span><span class="sxs-lookup"><span data-stu-id="1f0a6-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-bookingbusiness-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1f0a6-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1f0a6-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-bookingbusiness-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1f0a6-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1f0a6-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-bookingbusiness-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1f0a6-167">Ответ</span><span class="sxs-lookup"><span data-stu-id="1f0a6-167">Response</span></span>
<span data-ttu-id="1f0a6-168">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1f0a6-168">The following is an example of the response.</span></span> <span data-ttu-id="1f0a6-169">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="1f0a6-169">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="1f0a6-170">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1f0a6-170">All of the properties will be returned from an actual call.</span></span>
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
