---
title: Обновление bookingbusiness
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: 53115469821bc39c05c4e7a262e5f9fc15b376ce
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824999"
---
# <a name="update-bookingbusiness"></a><span data-ttu-id="6da63-104">Обновление bookingbusiness</span><span class="sxs-lookup"><span data-stu-id="6da63-104">Update bookingbusiness</span></span>

 > <span data-ttu-id="6da63-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6da63-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6da63-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6da63-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="6da63-107">Обновление свойства объекта [bookingBusiness](../resources/bookingbusiness.md) .</span><span class="sxs-lookup"><span data-stu-id="6da63-107">Update the properties of a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="6da63-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6da63-108">Permissions</span></span>
<span data-ttu-id="6da63-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6da63-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6da63-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6da63-111">Permission type</span></span>      | <span data-ttu-id="6da63-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6da63-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6da63-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6da63-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="6da63-114">Bookings.ReadWrite.All Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="6da63-114">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="6da63-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6da63-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6da63-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6da63-116">Not supported.</span></span>   |
|<span data-ttu-id="6da63-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6da63-117">Application</span></span> | <span data-ttu-id="6da63-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6da63-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="6da63-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6da63-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/<id>
```
## <a name="optional-request-headers"></a><span data-ttu-id="6da63-120">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6da63-120">Optional request headers</span></span>
| <span data-ttu-id="6da63-121">Имя</span><span class="sxs-lookup"><span data-stu-id="6da63-121">Name</span></span>       | <span data-ttu-id="6da63-122">Описание</span><span class="sxs-lookup"><span data-stu-id="6da63-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="6da63-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6da63-123">Authorization</span></span>  | <span data-ttu-id="6da63-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="6da63-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="6da63-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6da63-125">Request body</span></span>
<span data-ttu-id="6da63-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="6da63-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6da63-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="6da63-129">Property</span></span>     | <span data-ttu-id="6da63-130">Тип</span><span class="sxs-lookup"><span data-stu-id="6da63-130">Type</span></span>   |<span data-ttu-id="6da63-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6da63-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6da63-132">address</span><span class="sxs-lookup"><span data-stu-id="6da63-132">address</span></span>|[<span data-ttu-id="6da63-133">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="6da63-133">physicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="6da63-134">Почтовый адрес организации.</span><span class="sxs-lookup"><span data-stu-id="6da63-134">The street address of the business.</span></span>|
|<span data-ttu-id="6da63-135">businessHours</span><span class="sxs-lookup"><span data-stu-id="6da63-135">businessHours</span></span>|<span data-ttu-id="6da63-136">[bookingWorkHours](../resources/bookingworkhours.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="6da63-136">[bookingWorkHours](../resources/bookingworkhours.md) collection</span></span>|<span data-ttu-id="6da63-137">Часы работы для предприятий.</span><span class="sxs-lookup"><span data-stu-id="6da63-137">The hours of operation for the business.</span></span>|
|<span data-ttu-id="6da63-138">businessType</span><span class="sxs-lookup"><span data-stu-id="6da63-138">businessType</span></span>|<span data-ttu-id="6da63-139">Строка</span><span class="sxs-lookup"><span data-stu-id="6da63-139">String</span></span>|<span data-ttu-id="6da63-140">Тип бизнеса.</span><span class="sxs-lookup"><span data-stu-id="6da63-140">The type of business.</span></span>|
|<span data-ttu-id="6da63-141">defaultCurrencyIso</span><span class="sxs-lookup"><span data-stu-id="6da63-141">defaultCurrencyIso</span></span>|<span data-ttu-id="6da63-142">Строка</span><span class="sxs-lookup"><span data-stu-id="6da63-142">String</span></span>|<span data-ttu-id="6da63-143">Код для валюты, предприятию работает в Microsoft резервирования.</span><span class="sxs-lookup"><span data-stu-id="6da63-143">The code for the currency that the business operates in on Microsoft Bookings.</span></span>|
|<span data-ttu-id="6da63-144">displayName</span><span class="sxs-lookup"><span data-stu-id="6da63-144">displayName</span></span>|<span data-ttu-id="6da63-145">Строка</span><span class="sxs-lookup"><span data-stu-id="6da63-145">String</span></span>|<span data-ttu-id="6da63-146">Имя для бизнеса, связанный с клиентами.</span><span class="sxs-lookup"><span data-stu-id="6da63-146">A name for the business that interfaces with customers.</span></span>|
|<span data-ttu-id="6da63-147">email</span><span class="sxs-lookup"><span data-stu-id="6da63-147">email</span></span>|<span data-ttu-id="6da63-148">String</span><span class="sxs-lookup"><span data-stu-id="6da63-148">String</span></span>|<span data-ttu-id="6da63-149">Адрес электронной почты для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="6da63-149">The email address for the business.</span></span>|
|<span data-ttu-id="6da63-150">phone</span><span class="sxs-lookup"><span data-stu-id="6da63-150">phone</span></span>|<span data-ttu-id="6da63-151">String</span><span class="sxs-lookup"><span data-stu-id="6da63-151">String</span></span>|<span data-ttu-id="6da63-152">Номер телефона для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="6da63-152">The telephone number for the business.</span></span>|
|<span data-ttu-id="6da63-153">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="6da63-153">schedulingPolicy</span></span>|[<span data-ttu-id="6da63-154">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="6da63-154">bookingSchedulingPolicy</span></span>](../resources/bookingschedulingpolicy.md)|<span data-ttu-id="6da63-155">Указывает, как можно создать резервирования для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="6da63-155">Specifies how bookings can be created for this business.</span></span>|
|<span data-ttu-id="6da63-156">webSiteUrl</span><span class="sxs-lookup"><span data-stu-id="6da63-156">webSiteUrl</span></span>|<span data-ttu-id="6da63-157">Строка</span><span class="sxs-lookup"><span data-stu-id="6da63-157">String</span></span>|<span data-ttu-id="6da63-158">URL-адрес веб-сайта бизнеса.</span><span class="sxs-lookup"><span data-stu-id="6da63-158">The URL of the business web site.</span></span>|

## <a name="response"></a><span data-ttu-id="6da63-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="6da63-159">Response</span></span>
<span data-ttu-id="6da63-p105">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6da63-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6da63-162">Пример</span><span class="sxs-lookup"><span data-stu-id="6da63-162">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6da63-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="6da63-163">Request</span></span>
<span data-ttu-id="6da63-164">В следующем примере обновляются рабочий адрес электронной почты и планирования политики, чтобы изменить промежуток времени резервирования по умолчанию business часа и переход резервирования до 30 дней.</span><span class="sxs-lookup"><span data-stu-id="6da63-164">The following example updates the business email address and scheduling policy, to change the business default booking time slot to an hour, and advance booking up to 30 days.</span></span>
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
##### <a name="response"></a><span data-ttu-id="6da63-165">Ответ</span><span class="sxs-lookup"><span data-stu-id="6da63-165">Response</span></span>
<span data-ttu-id="6da63-166">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6da63-166">The following is an example of the response.</span></span> <span data-ttu-id="6da63-167">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="6da63-167">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="6da63-168">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6da63-168">All of the properties will be returned from an actual call.</span></span>
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
