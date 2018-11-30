---
title: Обновление bookingbusiness
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
ms.openlocfilehash: c0d92e0ddf792e28cb488cf466a1462272086c8f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076708"
---
# <a name="update-bookingbusiness"></a><span data-ttu-id="530d3-104">Обновление bookingbusiness</span><span class="sxs-lookup"><span data-stu-id="530d3-104">Update bookingbusiness</span></span>

 > <span data-ttu-id="530d3-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="530d3-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="530d3-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="530d3-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="530d3-107">Обновление свойства объекта [bookingBusiness](../resources/bookingbusiness.md) .</span><span class="sxs-lookup"><span data-stu-id="530d3-107">Update the properties of a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="530d3-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="530d3-108">Permissions</span></span>
<span data-ttu-id="530d3-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="530d3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="530d3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="530d3-111">Permission type</span></span>      | <span data-ttu-id="530d3-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="530d3-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="530d3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="530d3-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="530d3-114">Bookings.ReadWrite.All Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="530d3-114">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="530d3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="530d3-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="530d3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="530d3-116">Not supported.</span></span>   |
|<span data-ttu-id="530d3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="530d3-117">Application</span></span> | <span data-ttu-id="530d3-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="530d3-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="530d3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="530d3-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/<id>
```
## <a name="optional-request-headers"></a><span data-ttu-id="530d3-120">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="530d3-120">Optional request headers</span></span>
| <span data-ttu-id="530d3-121">Имя</span><span class="sxs-lookup"><span data-stu-id="530d3-121">Name</span></span>       | <span data-ttu-id="530d3-122">Описание</span><span class="sxs-lookup"><span data-stu-id="530d3-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="530d3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="530d3-123">Authorization</span></span>  | <span data-ttu-id="530d3-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="530d3-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="530d3-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="530d3-125">Request body</span></span>
<span data-ttu-id="530d3-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="530d3-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="530d3-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="530d3-129">Property</span></span>     | <span data-ttu-id="530d3-130">Тип</span><span class="sxs-lookup"><span data-stu-id="530d3-130">Type</span></span>   |<span data-ttu-id="530d3-131">Описание</span><span class="sxs-lookup"><span data-stu-id="530d3-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="530d3-132">address</span><span class="sxs-lookup"><span data-stu-id="530d3-132">address</span></span>|[<span data-ttu-id="530d3-133">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="530d3-133">physicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="530d3-134">Почтовый адрес организации.</span><span class="sxs-lookup"><span data-stu-id="530d3-134">The street address of the business.</span></span>|
|<span data-ttu-id="530d3-135">businessHours</span><span class="sxs-lookup"><span data-stu-id="530d3-135">businessHours</span></span>|<span data-ttu-id="530d3-136">[bookingWorkHours](../resources/bookingworkhours.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="530d3-136">[bookingWorkHours](../resources/bookingworkhours.md) collection</span></span>|<span data-ttu-id="530d3-137">Часы работы для предприятий.</span><span class="sxs-lookup"><span data-stu-id="530d3-137">The hours of operation for the business.</span></span>|
|<span data-ttu-id="530d3-138">businessType</span><span class="sxs-lookup"><span data-stu-id="530d3-138">businessType</span></span>|<span data-ttu-id="530d3-139">String</span><span class="sxs-lookup"><span data-stu-id="530d3-139">String</span></span>|<span data-ttu-id="530d3-140">Тип бизнеса.</span><span class="sxs-lookup"><span data-stu-id="530d3-140">The type of business.</span></span>|
|<span data-ttu-id="530d3-141">defaultCurrencyIso</span><span class="sxs-lookup"><span data-stu-id="530d3-141">defaultCurrencyIso</span></span>|<span data-ttu-id="530d3-142">String</span><span class="sxs-lookup"><span data-stu-id="530d3-142">String</span></span>|<span data-ttu-id="530d3-143">Код для валюты, предприятию работает в Microsoft резервирования.</span><span class="sxs-lookup"><span data-stu-id="530d3-143">The code for the currency that the business operates in on Microsoft Bookings.</span></span>|
|<span data-ttu-id="530d3-144">displayName</span><span class="sxs-lookup"><span data-stu-id="530d3-144">displayName</span></span>|<span data-ttu-id="530d3-145">String</span><span class="sxs-lookup"><span data-stu-id="530d3-145">String</span></span>|<span data-ttu-id="530d3-146">Имя для бизнеса, связанный с клиентами.</span><span class="sxs-lookup"><span data-stu-id="530d3-146">A name for the business that interfaces with customers.</span></span>|
|<span data-ttu-id="530d3-147">email</span><span class="sxs-lookup"><span data-stu-id="530d3-147">email</span></span>|<span data-ttu-id="530d3-148">String</span><span class="sxs-lookup"><span data-stu-id="530d3-148">String</span></span>|<span data-ttu-id="530d3-149">Адрес электронной почты для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="530d3-149">The email address for the business.</span></span>|
|<span data-ttu-id="530d3-150">phone</span><span class="sxs-lookup"><span data-stu-id="530d3-150">phone</span></span>|<span data-ttu-id="530d3-151">String</span><span class="sxs-lookup"><span data-stu-id="530d3-151">String</span></span>|<span data-ttu-id="530d3-152">Номер телефона для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="530d3-152">The telephone number for the business.</span></span>|
|<span data-ttu-id="530d3-153">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="530d3-153">schedulingPolicy</span></span>|[<span data-ttu-id="530d3-154">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="530d3-154">bookingSchedulingPolicy</span></span>](../resources/bookingschedulingpolicy.md)|<span data-ttu-id="530d3-155">Указывает, как можно создать резервирования для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="530d3-155">Specifies how bookings can be created for this business.</span></span>|
|<span data-ttu-id="530d3-156">webSiteUrl</span><span class="sxs-lookup"><span data-stu-id="530d3-156">webSiteUrl</span></span>|<span data-ttu-id="530d3-157">String</span><span class="sxs-lookup"><span data-stu-id="530d3-157">String</span></span>|<span data-ttu-id="530d3-158">URL-адрес веб-сайта бизнеса.</span><span class="sxs-lookup"><span data-stu-id="530d3-158">The URL of the business web site.</span></span>|

## <a name="response"></a><span data-ttu-id="530d3-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="530d3-159">Response</span></span>
<span data-ttu-id="530d3-p105">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="530d3-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="530d3-162">Пример</span><span class="sxs-lookup"><span data-stu-id="530d3-162">Example</span></span>
##### <a name="request"></a><span data-ttu-id="530d3-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="530d3-163">Request</span></span>
<span data-ttu-id="530d3-164">В следующем примере обновляются рабочий адрес электронной почты и планирования политики, чтобы изменить промежуток времени резервирования по умолчанию business часа и переход резервирования до 30 дней.</span><span class="sxs-lookup"><span data-stu-id="530d3-164">The following example updates the business email address and scheduling policy, to change the business default booking time slot to an hour, and advance booking up to 30 days.</span></span>
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
##### <a name="response"></a><span data-ttu-id="530d3-165">Ответ</span><span class="sxs-lookup"><span data-stu-id="530d3-165">Response</span></span>
<span data-ttu-id="530d3-166">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="530d3-166">The following is an example of the response.</span></span> <span data-ttu-id="530d3-167">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="530d3-167">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="530d3-168">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="530d3-168">All of the properties will be returned from an actual call.</span></span>
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
  "description": "Update bookingbusiness",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->