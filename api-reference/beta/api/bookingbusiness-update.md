---
title: Обновление bookingbusiness
description: Обновление свойства объекта bookingBusiness.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: dba24dafef030ae53fc83fb06d1cc7b99ed71e81
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528804"
---
# <a name="update-bookingbusiness"></a><span data-ttu-id="e7a07-103">Обновление bookingbusiness</span><span class="sxs-lookup"><span data-stu-id="e7a07-103">Update bookingbusiness</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7a07-104">Обновление свойства объекта [bookingBusiness](../resources/bookingbusiness.md) .</span><span class="sxs-lookup"><span data-stu-id="e7a07-104">Update the properties of a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e7a07-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e7a07-105">Permissions</span></span>
<span data-ttu-id="e7a07-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7a07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7a07-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e7a07-108">Permission type</span></span>      | <span data-ttu-id="e7a07-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e7a07-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7a07-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e7a07-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="e7a07-111">Bookings.ReadWrite.All Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="e7a07-111">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="e7a07-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e7a07-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7a07-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7a07-113">Not supported.</span></span>   |
|<span data-ttu-id="e7a07-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e7a07-114">Application</span></span> | <span data-ttu-id="e7a07-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7a07-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="e7a07-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e7a07-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/<id>
```
## <a name="optional-request-headers"></a><span data-ttu-id="e7a07-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e7a07-117">Optional request headers</span></span>
| <span data-ttu-id="e7a07-118">Имя</span><span class="sxs-lookup"><span data-stu-id="e7a07-118">Name</span></span>       | <span data-ttu-id="e7a07-119">Описание</span><span class="sxs-lookup"><span data-stu-id="e7a07-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e7a07-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7a07-120">Authorization</span></span>  | <span data-ttu-id="e7a07-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="e7a07-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7a07-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e7a07-122">Request body</span></span>
<span data-ttu-id="e7a07-p102">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="e7a07-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e7a07-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="e7a07-126">Property</span></span>     | <span data-ttu-id="e7a07-127">Тип</span><span class="sxs-lookup"><span data-stu-id="e7a07-127">Type</span></span>   |<span data-ttu-id="e7a07-128">Описание</span><span class="sxs-lookup"><span data-stu-id="e7a07-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e7a07-129">address</span><span class="sxs-lookup"><span data-stu-id="e7a07-129">address</span></span>|[<span data-ttu-id="e7a07-130">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="e7a07-130">physicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="e7a07-131">Почтовый адрес организации.</span><span class="sxs-lookup"><span data-stu-id="e7a07-131">The street address of the business.</span></span>|
|<span data-ttu-id="e7a07-132">businessHours</span><span class="sxs-lookup"><span data-stu-id="e7a07-132">businessHours</span></span>|<span data-ttu-id="e7a07-133">[bookingWorkHours](../resources/bookingworkhours.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="e7a07-133">[bookingWorkHours](../resources/bookingworkhours.md) collection</span></span>|<span data-ttu-id="e7a07-134">Часы работы для предприятий.</span><span class="sxs-lookup"><span data-stu-id="e7a07-134">The hours of operation for the business.</span></span>|
|<span data-ttu-id="e7a07-135">businessType</span><span class="sxs-lookup"><span data-stu-id="e7a07-135">businessType</span></span>|<span data-ttu-id="e7a07-136">String</span><span class="sxs-lookup"><span data-stu-id="e7a07-136">String</span></span>|<span data-ttu-id="e7a07-137">Тип бизнеса.</span><span class="sxs-lookup"><span data-stu-id="e7a07-137">The type of business.</span></span>|
|<span data-ttu-id="e7a07-138">defaultCurrencyIso</span><span class="sxs-lookup"><span data-stu-id="e7a07-138">defaultCurrencyIso</span></span>|<span data-ttu-id="e7a07-139">String</span><span class="sxs-lookup"><span data-stu-id="e7a07-139">String</span></span>|<span data-ttu-id="e7a07-140">Код для валюты, предприятию работает в Microsoft резервирования.</span><span class="sxs-lookup"><span data-stu-id="e7a07-140">The code for the currency that the business operates in on Microsoft Bookings.</span></span>|
|<span data-ttu-id="e7a07-141">displayName</span><span class="sxs-lookup"><span data-stu-id="e7a07-141">displayName</span></span>|<span data-ttu-id="e7a07-142">Строка</span><span class="sxs-lookup"><span data-stu-id="e7a07-142">String</span></span>|<span data-ttu-id="e7a07-143">Имя для бизнеса, связанный с клиентами.</span><span class="sxs-lookup"><span data-stu-id="e7a07-143">A name for the business that interfaces with customers.</span></span>|
|<span data-ttu-id="e7a07-144">email</span><span class="sxs-lookup"><span data-stu-id="e7a07-144">email</span></span>|<span data-ttu-id="e7a07-145">String</span><span class="sxs-lookup"><span data-stu-id="e7a07-145">String</span></span>|<span data-ttu-id="e7a07-146">Адрес электронной почты для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="e7a07-146">The email address for the business.</span></span>|
|<span data-ttu-id="e7a07-147">phone</span><span class="sxs-lookup"><span data-stu-id="e7a07-147">phone</span></span>|<span data-ttu-id="e7a07-148">String</span><span class="sxs-lookup"><span data-stu-id="e7a07-148">String</span></span>|<span data-ttu-id="e7a07-149">Номер телефона для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="e7a07-149">The telephone number for the business.</span></span>|
|<span data-ttu-id="e7a07-150">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="e7a07-150">schedulingPolicy</span></span>|[<span data-ttu-id="e7a07-151">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="e7a07-151">bookingSchedulingPolicy</span></span>](../resources/bookingschedulingpolicy.md)|<span data-ttu-id="e7a07-152">Указывает, как можно создать резервирования для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="e7a07-152">Specifies how bookings can be created for this business.</span></span>|
|<span data-ttu-id="e7a07-153">websiteUrl</span><span class="sxs-lookup"><span data-stu-id="e7a07-153">webSiteUrl</span></span>|<span data-ttu-id="e7a07-154">String</span><span class="sxs-lookup"><span data-stu-id="e7a07-154">String</span></span>|<span data-ttu-id="e7a07-155">URL-адрес веб-сайта бизнеса.</span><span class="sxs-lookup"><span data-stu-id="e7a07-155">The URL of the business web site.</span></span>|

## <a name="response"></a><span data-ttu-id="e7a07-156">Ответ</span><span class="sxs-lookup"><span data-stu-id="e7a07-156">Response</span></span>
<span data-ttu-id="e7a07-p103">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e7a07-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e7a07-159">Пример</span><span class="sxs-lookup"><span data-stu-id="e7a07-159">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e7a07-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="e7a07-160">Request</span></span>
<span data-ttu-id="e7a07-161">В следующем примере обновляются рабочий адрес электронной почты и планирования политики, чтобы изменить промежуток времени резервирования по умолчанию business часа и переход резервирования до 30 дней.</span><span class="sxs-lookup"><span data-stu-id="e7a07-161">The following example updates the business email address and scheduling policy, to change the business default booking time slot to an hour, and advance booking up to 30 days.</span></span>
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
##### <a name="response"></a><span data-ttu-id="e7a07-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="e7a07-162">Response</span></span>
<span data-ttu-id="e7a07-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e7a07-163">The following is an example of the response.</span></span> <span data-ttu-id="e7a07-164">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="e7a07-164">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="e7a07-165">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e7a07-165">All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/bookingbusiness-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
