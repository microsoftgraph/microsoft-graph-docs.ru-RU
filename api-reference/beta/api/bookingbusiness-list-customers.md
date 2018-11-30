---
title: Список клиентов
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
ms.openlocfilehash: a46e8dcc39b69e8391829c176eb01d075d23fccf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076694"
---
# <a name="list-customers"></a><span data-ttu-id="86ccb-104">Список клиентов</span><span class="sxs-lookup"><span data-stu-id="86ccb-104">List customers</span></span>

 > <span data-ttu-id="86ccb-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="86ccb-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="86ccb-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86ccb-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="86ccb-107">Получите список объектов [bookingCustomer](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="86ccb-107">Get a list of [bookingCustomer](../resources/bookingcustomer.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="86ccb-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="86ccb-108">Permissions</span></span>
<span data-ttu-id="86ccb-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86ccb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86ccb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="86ccb-111">Permission type</span></span>      | <span data-ttu-id="86ccb-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="86ccb-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="86ccb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="86ccb-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="86ccb-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="86ccb-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="86ccb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="86ccb-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86ccb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86ccb-116">Not supported.</span></span>   |
|<span data-ttu-id="86ccb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="86ccb-117">Application</span></span> | <span data-ttu-id="86ccb-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86ccb-118">Not supported.</span></span>  |  

## <a name="http-request"></a><span data-ttu-id="86ccb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="86ccb-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/customers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="86ccb-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="86ccb-120">Optional query parameters</span></span>
<span data-ttu-id="86ccb-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="86ccb-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="86ccb-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="86ccb-122">Request headers</span></span>
| <span data-ttu-id="86ccb-123">Имя</span><span class="sxs-lookup"><span data-stu-id="86ccb-123">Name</span></span>      |<span data-ttu-id="86ccb-124">Описание</span><span class="sxs-lookup"><span data-stu-id="86ccb-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="86ccb-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="86ccb-125">Authorization</span></span>  | <span data-ttu-id="86ccb-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="86ccb-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="86ccb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="86ccb-127">Request body</span></span>
<span data-ttu-id="86ccb-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="86ccb-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="86ccb-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="86ccb-129">Response</span></span>
<span data-ttu-id="86ccb-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [bookingCustomer](../resources/bookingcustomer.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="86ccb-130">If successful, this method returns a `200 OK` response code and collection of [bookingCustomer](../resources/bookingcustomer.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="86ccb-131">Пример</span><span class="sxs-lookup"><span data-stu-id="86ccb-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="86ccb-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="86ccb-132">Request</span></span>
<span data-ttu-id="86ccb-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="86ccb-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_customers"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers
```
##### <a name="response"></a><span data-ttu-id="86ccb-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="86ccb-134">Response</span></span>
<span data-ttu-id="86ccb-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="86ccb-135">The following is an example of the response.</span></span> <span data-ttu-id="86ccb-136">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="86ccb-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="86ccb-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="86ccb-137">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCustomer",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/customers",
    "value": [
        {
            "id": "80b5ddda-1e3b-4c9d-abe2-d606cc075e2e",
            "displayName": "Adele Vance",
            "emailAddress": "adelev@proseware.com"
        },
        {
            "id": "8bb19078-0f45-4efb-b2c5-da78b860f73a",
            "displayName": "Adele Vance",
            "emailAddress": "adelev@proseware.com"
        },
        {
            "id": "829e3cb5-3d4d-4319-a8de-1953aedaa166",
            "displayName": "Bob Kelly",
            "emailAddress": "bobk@tailspintoys.com"
        },
        {
            "id": "7ed53fa5-9ef2-4f2f-975b-27447440bc09",
            "displayName": "Jordan Miller",
            "emailAddress": "jordanm@contoso.com"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List customers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->