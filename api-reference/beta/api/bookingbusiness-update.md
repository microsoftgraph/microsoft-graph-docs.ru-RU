---
title: Обновление букингбусинесс
description: Обновление свойств объекта Букингбусинесс.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: a9713231b8d0556ff27ee872039a40f1eadcc0cd
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865451"
---
# <a name="update-bookingbusiness"></a><span data-ttu-id="da576-103">Обновление букингбусинесс</span><span class="sxs-lookup"><span data-stu-id="da576-103">Update bookingbusiness</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da576-104">Обновление свойств объекта [букингбусинесс](../resources/bookingbusiness.md) .</span><span class="sxs-lookup"><span data-stu-id="da576-104">Update the properties of a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="da576-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="da576-105">Permissions</span></span>
<span data-ttu-id="da576-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da576-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da576-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="da576-108">Permission type</span></span>      | <span data-ttu-id="da576-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="da576-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da576-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="da576-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="da576-111">Резервирования. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="da576-111">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="da576-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="da576-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da576-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da576-113">Not supported.</span></span>   |
|<span data-ttu-id="da576-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="da576-114">Application</span></span> | <span data-ttu-id="da576-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da576-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="da576-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="da576-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/<id>
```
## <a name="optional-request-headers"></a><span data-ttu-id="da576-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="da576-117">Optional request headers</span></span>
| <span data-ttu-id="da576-118">Имя</span><span class="sxs-lookup"><span data-stu-id="da576-118">Name</span></span>       | <span data-ttu-id="da576-119">Описание</span><span class="sxs-lookup"><span data-stu-id="da576-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="da576-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="da576-120">Authorization</span></span>  | <span data-ttu-id="da576-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="da576-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="da576-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="da576-122">Request body</span></span>
<span data-ttu-id="da576-p102">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="da576-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="da576-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="da576-126">Property</span></span>     | <span data-ttu-id="da576-127">Тип</span><span class="sxs-lookup"><span data-stu-id="da576-127">Type</span></span>   |<span data-ttu-id="da576-128">Описание</span><span class="sxs-lookup"><span data-stu-id="da576-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="da576-129">address</span><span class="sxs-lookup"><span data-stu-id="da576-129">address</span></span>|[<span data-ttu-id="da576-130">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="da576-130">physicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="da576-131">Адрес в почтовом ящике организации.</span><span class="sxs-lookup"><span data-stu-id="da576-131">The street address of the business.</span></span>|
|<span data-ttu-id="da576-132">businessHours</span><span class="sxs-lookup"><span data-stu-id="da576-132">businessHours</span></span>|<span data-ttu-id="da576-133">Коллекция [букингворкхаурс](../resources/bookingworkhours.md)</span><span class="sxs-lookup"><span data-stu-id="da576-133">[bookingWorkHours](../resources/bookingworkhours.md) collection</span></span>|<span data-ttu-id="da576-134">Количество часов работы для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="da576-134">The hours of operation for the business.</span></span>|
|<span data-ttu-id="da576-135">Бусинесстипе</span><span class="sxs-lookup"><span data-stu-id="da576-135">businessType</span></span>|<span data-ttu-id="da576-136">String</span><span class="sxs-lookup"><span data-stu-id="da576-136">String</span></span>|<span data-ttu-id="da576-137">Тип бизнеса.</span><span class="sxs-lookup"><span data-stu-id="da576-137">The type of business.</span></span>|
|<span data-ttu-id="da576-138">Дефаулткурренциисо</span><span class="sxs-lookup"><span data-stu-id="da576-138">defaultCurrencyIso</span></span>|<span data-ttu-id="da576-139">String</span><span class="sxs-lookup"><span data-stu-id="da576-139">String</span></span>|<span data-ttu-id="da576-140">Код валюты, в которой работает предприятие, в Microsoft Books.</span><span class="sxs-lookup"><span data-stu-id="da576-140">The code for the currency that the business operates in on Microsoft Bookings.</span></span>|
|<span data-ttu-id="da576-141">displayName</span><span class="sxs-lookup"><span data-stu-id="da576-141">displayName</span></span>|<span data-ttu-id="da576-142">Строка</span><span class="sxs-lookup"><span data-stu-id="da576-142">String</span></span>|<span data-ttu-id="da576-143">Название организации, которая взаимодействует с клиентами.</span><span class="sxs-lookup"><span data-stu-id="da576-143">A name for the business that interfaces with customers.</span></span>|
|<span data-ttu-id="da576-144">email</span><span class="sxs-lookup"><span data-stu-id="da576-144">email</span></span>|<span data-ttu-id="da576-145">String</span><span class="sxs-lookup"><span data-stu-id="da576-145">String</span></span>|<span data-ttu-id="da576-146">Адрес электронной почты для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="da576-146">The email address for the business.</span></span>|
|<span data-ttu-id="da576-147">phone</span><span class="sxs-lookup"><span data-stu-id="da576-147">phone</span></span>|<span data-ttu-id="da576-148">String</span><span class="sxs-lookup"><span data-stu-id="da576-148">String</span></span>|<span data-ttu-id="da576-149">Номер телефона для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="da576-149">The telephone number for the business.</span></span>|
|<span data-ttu-id="da576-150">Счедулингполици</span><span class="sxs-lookup"><span data-stu-id="da576-150">schedulingPolicy</span></span>|[<span data-ttu-id="da576-151">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="da576-151">bookingSchedulingPolicy</span></span>](../resources/bookingschedulingpolicy.md)|<span data-ttu-id="da576-152">Указывает, как можно создавать резервирования для этого бизнеса.</span><span class="sxs-lookup"><span data-stu-id="da576-152">Specifies how bookings can be created for this business.</span></span>|
|<span data-ttu-id="da576-153">Вебситеурл</span><span class="sxs-lookup"><span data-stu-id="da576-153">webSiteUrl</span></span>|<span data-ttu-id="da576-154">String</span><span class="sxs-lookup"><span data-stu-id="da576-154">String</span></span>|<span data-ttu-id="da576-155">URL-адрес веб-сайта компании.</span><span class="sxs-lookup"><span data-stu-id="da576-155">The URL of the business web site.</span></span>|

## <a name="response"></a><span data-ttu-id="da576-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="da576-156">Response</span></span>
<span data-ttu-id="da576-p103">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="da576-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="da576-159">Пример</span><span class="sxs-lookup"><span data-stu-id="da576-159">Example</span></span>
##### <a name="request"></a><span data-ttu-id="da576-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="da576-160">Request</span></span>
<span data-ttu-id="da576-161">В следующем примере показано, как обновить адрес электронной почты и политику планирования, чтобы изменить период резервирования по умолчанию для бизнеса на час, а затем выполнить резервное резервирование в течение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="da576-161">The following example updates the business email address and scheduling policy, to change the business default booking time slot to an hour, and advance booking up to 30 days.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="da576-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="da576-162">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="da576-163">C#</span><span class="sxs-lookup"><span data-stu-id="da576-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-bookingbusiness-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="da576-164">Javascript</span><span class="sxs-lookup"><span data-stu-id="da576-164">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-bookingbusiness-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="da576-165">Цель — C</span><span class="sxs-lookup"><span data-stu-id="da576-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-bookingbusiness-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="da576-166">Java</span><span class="sxs-lookup"><span data-stu-id="da576-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-bookingbusiness-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="da576-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="da576-167">Response</span></span>
<span data-ttu-id="da576-168">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="da576-168">The following is an example of the response.</span></span> <span data-ttu-id="da576-169">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="da576-169">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="da576-170">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="da576-170">All of the properties will be returned from an actual call.</span></span>
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
