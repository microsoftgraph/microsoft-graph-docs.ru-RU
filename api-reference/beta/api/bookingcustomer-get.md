---
title: Получение bookingCustomer
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: 4c17b1d80b6f105c35554012313736fee46b0b36
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818713"
---
# <a name="get-bookingcustomer"></a><span data-ttu-id="91360-104">Получение bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="91360-104">Get bookingCustomer</span></span>

 > <span data-ttu-id="91360-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="91360-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="91360-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91360-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="91360-107">Получите свойства и связи объекта [bookingCustomer](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="91360-107">Get the properties and relationships of a [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="91360-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="91360-108">Permissions</span></span>
<span data-ttu-id="91360-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91360-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91360-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="91360-111">Permission type</span></span>      | <span data-ttu-id="91360-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="91360-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91360-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="91360-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="91360-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="91360-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="91360-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="91360-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91360-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91360-116">Not supported.</span></span>   |
|<span data-ttu-id="91360-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="91360-117">Application</span></span> | <span data-ttu-id="91360-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91360-118">Not supported.</span></span>  |  

## <a name="http-request"></a><span data-ttu-id="91360-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="91360-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/customers/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="91360-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="91360-120">Optional query parameters</span></span>
<span data-ttu-id="91360-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="91360-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="91360-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="91360-122">Request headers</span></span>
| <span data-ttu-id="91360-123">Имя</span><span class="sxs-lookup"><span data-stu-id="91360-123">Name</span></span>      |<span data-ttu-id="91360-124">Описание</span><span class="sxs-lookup"><span data-stu-id="91360-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="91360-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="91360-125">Authorization</span></span>  | <span data-ttu-id="91360-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="91360-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="91360-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="91360-127">Request body</span></span>
<span data-ttu-id="91360-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="91360-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="91360-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="91360-129">Response</span></span>
<span data-ttu-id="91360-130">Успешно завершена, этот метод возвращает `200 OK` объект [bookingCustomer](../resources/bookingcustomer.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="91360-130">If successful, this method returns a `200 OK` response code and [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="91360-131">Пример</span><span class="sxs-lookup"><span data-stu-id="91360-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="91360-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="91360-132">Request</span></span>
<span data-ttu-id="91360-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="91360-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingcustomer"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers/8bb19078-0f45-4efb-b2c5-da78b860f73a
```
##### <a name="response"></a><span data-ttu-id="91360-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="91360-134">Response</span></span>
<span data-ttu-id="91360-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="91360-135">The following is an example of the response.</span></span> <span data-ttu-id="91360-136">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="91360-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="91360-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="91360-137">All of the properties will be returned from an actual call.</span></span>
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
    "displayName": "Adele Vance",
    "emailAddress": "adelev@proseware.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get bookingCustomer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
