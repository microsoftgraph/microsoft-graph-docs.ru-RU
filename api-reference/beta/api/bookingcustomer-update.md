---
title: Обновление bookingcustomer
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: a22568347e887a9c0ddfc000123e3413d544c7fc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990516"
---
# <a name="update-bookingcustomer"></a><span data-ttu-id="b9f85-104">Обновление bookingcustomer</span><span class="sxs-lookup"><span data-stu-id="b9f85-104">Update bookingcustomer</span></span>

 > <span data-ttu-id="b9f85-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b9f85-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b9f85-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9f85-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="b9f85-107">Обновление свойства объекта [bookingCustomer](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="b9f85-107">Update the properties of a [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b9f85-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b9f85-108">Permissions</span></span>
<span data-ttu-id="b9f85-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9f85-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9f85-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b9f85-111">Permission type</span></span>      | <span data-ttu-id="b9f85-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b9f85-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9f85-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b9f85-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b9f85-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="b9f85-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="b9f85-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b9f85-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9f85-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9f85-116">Not supported.</span></span>   |
|<span data-ttu-id="b9f85-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b9f85-117">Application</span></span> | <span data-ttu-id="b9f85-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9f85-118">Not supported.</span></span>  |  

## <a name="http-request"></a><span data-ttu-id="b9f85-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b9f85-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/customers/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="b9f85-120">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b9f85-120">Optional request headers</span></span>
| <span data-ttu-id="b9f85-121">Имя</span><span class="sxs-lookup"><span data-stu-id="b9f85-121">Name</span></span>       | <span data-ttu-id="b9f85-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b9f85-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="b9f85-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9f85-123">Authorization</span></span>  | <span data-ttu-id="b9f85-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="b9f85-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9f85-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b9f85-125">Request body</span></span>
<span data-ttu-id="b9f85-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="b9f85-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b9f85-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b9f85-129">Property</span></span>     | <span data-ttu-id="b9f85-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b9f85-130">Type</span></span>   |<span data-ttu-id="b9f85-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b9f85-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b9f85-132">displayName</span><span class="sxs-lookup"><span data-stu-id="b9f85-132">displayName</span></span>|<span data-ttu-id="b9f85-133">String</span><span class="sxs-lookup"><span data-stu-id="b9f85-133">String</span></span>|<span data-ttu-id="b9f85-134">Имя клиента.</span><span class="sxs-lookup"><span data-stu-id="b9f85-134">The name of the customer.</span></span>|
|<span data-ttu-id="b9f85-135">emailAddress</span><span class="sxs-lookup"><span data-stu-id="b9f85-135">emailAddress</span></span>|<span data-ttu-id="b9f85-136">String</span><span class="sxs-lookup"><span data-stu-id="b9f85-136">String</span></span>|<span data-ttu-id="b9f85-137">SMTP-адрес клиента.</span><span class="sxs-lookup"><span data-stu-id="b9f85-137">The SMTP address of the customer.</span></span>|

## <a name="response"></a><span data-ttu-id="b9f85-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="b9f85-138">Response</span></span>
<span data-ttu-id="b9f85-139">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [bookingCustomer](../resources/bookingcustomer.md) объект в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b9f85-139">If successful, this method returns a `200 OK` response code and updated [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b9f85-140">Пример</span><span class="sxs-lookup"><span data-stu-id="b9f85-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b9f85-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="b9f85-141">Request</span></span>
<span data-ttu-id="b9f85-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b9f85-142">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_bookingcustomer"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers/8bb19078-0f45-4efb-b2c5-da78b860f73a
Content-type: application/json

{
    "displayName": "Adele",
    "emailAddress": "adele@relecloud.com"
}
```
##### <a name="response"></a><span data-ttu-id="b9f85-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="b9f85-143">Response</span></span>
<span data-ttu-id="b9f85-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b9f85-144">The following is an example of the response.</span></span> <span data-ttu-id="b9f85-145">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="b9f85-145">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b9f85-146">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b9f85-146">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCustomer"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/customers/$entity",
    "id": "8bb19078-0f45-4efb-b2c5-da78b860f73a",
    "displayName": "Adele",
    "emailAddress": "adele@relecloud.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update bookingcustomer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
