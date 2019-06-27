---
title: Обновление букингбусинесс
description: Обновление свойств объекта Букингбусинесс.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 25d1f592590b4afafe4358f591115b05ff273903
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35257941"
---
# <a name="update-bookingbusiness"></a><span data-ttu-id="46d51-103">Обновление букингбусинесс</span><span class="sxs-lookup"><span data-stu-id="46d51-103">Update bookingbusiness</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46d51-104">Обновление свойств объекта [букингбусинесс](../resources/bookingbusiness.md) .</span><span class="sxs-lookup"><span data-stu-id="46d51-104">Update the properties of a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="46d51-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="46d51-105">Permissions</span></span>
<span data-ttu-id="46d51-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46d51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46d51-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="46d51-108">Permission type</span></span>      | <span data-ttu-id="46d51-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="46d51-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="46d51-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="46d51-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="46d51-111">Резервирования. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="46d51-111">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="46d51-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="46d51-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46d51-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46d51-113">Not supported.</span></span>   |
|<span data-ttu-id="46d51-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="46d51-114">Application</span></span> | <span data-ttu-id="46d51-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46d51-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="46d51-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="46d51-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/<id>
```
## <a name="optional-request-headers"></a><span data-ttu-id="46d51-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="46d51-117">Optional request headers</span></span>
| <span data-ttu-id="46d51-118">Имя</span><span class="sxs-lookup"><span data-stu-id="46d51-118">Name</span></span>       | <span data-ttu-id="46d51-119">Описание</span><span class="sxs-lookup"><span data-stu-id="46d51-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="46d51-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="46d51-120">Authorization</span></span>  | <span data-ttu-id="46d51-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="46d51-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="46d51-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="46d51-122">Request body</span></span>
<span data-ttu-id="46d51-p102">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="46d51-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="46d51-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="46d51-126">Property</span></span>     | <span data-ttu-id="46d51-127">Тип</span><span class="sxs-lookup"><span data-stu-id="46d51-127">Type</span></span>   |<span data-ttu-id="46d51-128">Описание</span><span class="sxs-lookup"><span data-stu-id="46d51-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="46d51-129">address</span><span class="sxs-lookup"><span data-stu-id="46d51-129">address</span></span>|[<span data-ttu-id="46d51-130">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="46d51-130">physicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="46d51-131">Адрес в почтовом ящике организации.</span><span class="sxs-lookup"><span data-stu-id="46d51-131">The street address of the business.</span></span>|
|<span data-ttu-id="46d51-132">businessHours</span><span class="sxs-lookup"><span data-stu-id="46d51-132">businessHours</span></span>|<span data-ttu-id="46d51-133">Коллекция [букингворкхаурс](../resources/bookingworkhours.md)</span><span class="sxs-lookup"><span data-stu-id="46d51-133">[bookingWorkHours](../resources/bookingworkhours.md) collection</span></span>|<span data-ttu-id="46d51-134">Количество часов работы для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="46d51-134">The hours of operation for the business.</span></span>|
|<span data-ttu-id="46d51-135">Бусинесстипе</span><span class="sxs-lookup"><span data-stu-id="46d51-135">businessType</span></span>|<span data-ttu-id="46d51-136">String</span><span class="sxs-lookup"><span data-stu-id="46d51-136">String</span></span>|<span data-ttu-id="46d51-137">Тип бизнеса.</span><span class="sxs-lookup"><span data-stu-id="46d51-137">The type of business.</span></span>|
|<span data-ttu-id="46d51-138">Дефаулткурренциисо</span><span class="sxs-lookup"><span data-stu-id="46d51-138">defaultCurrencyIso</span></span>|<span data-ttu-id="46d51-139">String</span><span class="sxs-lookup"><span data-stu-id="46d51-139">String</span></span>|<span data-ttu-id="46d51-140">Код валюты, в которой работает предприятие, в Microsoft Books.</span><span class="sxs-lookup"><span data-stu-id="46d51-140">The code for the currency that the business operates in on Microsoft Bookings.</span></span>|
|<span data-ttu-id="46d51-141">displayName</span><span class="sxs-lookup"><span data-stu-id="46d51-141">displayName</span></span>|<span data-ttu-id="46d51-142">Строка</span><span class="sxs-lookup"><span data-stu-id="46d51-142">String</span></span>|<span data-ttu-id="46d51-143">Название организации, которая взаимодействует с клиентами.</span><span class="sxs-lookup"><span data-stu-id="46d51-143">A name for the business that interfaces with customers.</span></span>|
|<span data-ttu-id="46d51-144">email</span><span class="sxs-lookup"><span data-stu-id="46d51-144">email</span></span>|<span data-ttu-id="46d51-145">String</span><span class="sxs-lookup"><span data-stu-id="46d51-145">String</span></span>|<span data-ttu-id="46d51-146">Адрес электронной почты для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="46d51-146">The email address for the business.</span></span>|
|<span data-ttu-id="46d51-147">phone</span><span class="sxs-lookup"><span data-stu-id="46d51-147">phone</span></span>|<span data-ttu-id="46d51-148">String</span><span class="sxs-lookup"><span data-stu-id="46d51-148">String</span></span>|<span data-ttu-id="46d51-149">Номер телефона для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="46d51-149">The telephone number for the business.</span></span>|
|<span data-ttu-id="46d51-150">Счедулингполици</span><span class="sxs-lookup"><span data-stu-id="46d51-150">schedulingPolicy</span></span>|[<span data-ttu-id="46d51-151">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="46d51-151">bookingSchedulingPolicy</span></span>](../resources/bookingschedulingpolicy.md)|<span data-ttu-id="46d51-152">Указывает, как можно создавать резервирования для этого бизнеса.</span><span class="sxs-lookup"><span data-stu-id="46d51-152">Specifies how bookings can be created for this business.</span></span>|
|<span data-ttu-id="46d51-153">Вебситеурл</span><span class="sxs-lookup"><span data-stu-id="46d51-153">webSiteUrl</span></span>|<span data-ttu-id="46d51-154">String</span><span class="sxs-lookup"><span data-stu-id="46d51-154">String</span></span>|<span data-ttu-id="46d51-155">URL-адрес веб-сайта компании.</span><span class="sxs-lookup"><span data-stu-id="46d51-155">The URL of the business web site.</span></span>|

## <a name="response"></a><span data-ttu-id="46d51-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="46d51-156">Response</span></span>
<span data-ttu-id="46d51-p103">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="46d51-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="46d51-159">Пример</span><span class="sxs-lookup"><span data-stu-id="46d51-159">Example</span></span>
##### <a name="request"></a><span data-ttu-id="46d51-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="46d51-160">Request</span></span>
<span data-ttu-id="46d51-161">В следующем примере показано, как обновить адрес электронной почты и политику планирования, чтобы изменить период резервирования по умолчанию для бизнеса на час, а затем выполнить резервное резервирование в течение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="46d51-161">The following example updates the business email address and scheduling policy, to change the business default booking time slot to an hour, and advance booking up to 30 days.</span></span>
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
##### <a name="response"></a><span data-ttu-id="46d51-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="46d51-162">Response</span></span>
<span data-ttu-id="46d51-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="46d51-163">The following is an example of the response.</span></span> <span data-ttu-id="46d51-164">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="46d51-164">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="46d51-165">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="46d51-165">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="46d51-166">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="46d51-166">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="46d51-167">C#</span><span class="sxs-lookup"><span data-stu-id="46d51-167">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_bookingbusiness-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="46d51-168">Javascript</span><span class="sxs-lookup"><span data-stu-id="46d51-168">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_bookingbusiness-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="46d51-169">Цель — C</span><span class="sxs-lookup"><span data-stu-id="46d51-169">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_bookingbusiness-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/bookingbusiness-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/bookingbusiness-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingbusiness-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
