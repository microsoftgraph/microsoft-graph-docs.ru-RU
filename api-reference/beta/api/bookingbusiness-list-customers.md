---
title: Список клиентов
description: Получите список объектов bookingCustomer.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 9eff7f998ad5bf5f1c623e2a699c7c1be3636b8a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047905"
---
# <a name="list-customers"></a><span data-ttu-id="d3b2e-103">Список клиентов</span><span class="sxs-lookup"><span data-stu-id="d3b2e-103">List customers</span></span>

<span data-ttu-id="d3b2e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3b2e-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3b2e-105">Получите список объектов [bookingCustomer.](../resources/bookingcustomer.md)</span><span class="sxs-lookup"><span data-stu-id="d3b2e-105">Get a list of [bookingCustomer](../resources/bookingcustomer.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="d3b2e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d3b2e-106">Permissions</span></span>
<span data-ttu-id="d3b2e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3b2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3b2e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d3b2e-109">Permission type</span></span>      | <span data-ttu-id="d3b2e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d3b2e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d3b2e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d3b2e-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="d3b2e-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="d3b2e-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="d3b2e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d3b2e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3b2e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3b2e-114">Not supported.</span></span>   |
|<span data-ttu-id="d3b2e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d3b2e-115">Application</span></span> | <span data-ttu-id="d3b2e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3b2e-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="d3b2e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d3b2e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/customers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d3b2e-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d3b2e-118">Optional query parameters</span></span>
<span data-ttu-id="d3b2e-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d3b2e-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d3b2e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d3b2e-120">Request headers</span></span>
| <span data-ttu-id="d3b2e-121">Имя</span><span class="sxs-lookup"><span data-stu-id="d3b2e-121">Name</span></span>      |<span data-ttu-id="d3b2e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d3b2e-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d3b2e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d3b2e-123">Authorization</span></span>  | <span data-ttu-id="d3b2e-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="d3b2e-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3b2e-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d3b2e-125">Request body</span></span>
<span data-ttu-id="d3b2e-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d3b2e-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d3b2e-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3b2e-127">Response</span></span>
<span data-ttu-id="d3b2e-128">В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` [объектов bookingCustomer](../resources/bookingcustomer.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d3b2e-128">If successful, this method returns a `200 OK` response code and collection of [bookingCustomer](../resources/bookingcustomer.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d3b2e-129">Пример</span><span class="sxs-lookup"><span data-stu-id="d3b2e-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d3b2e-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="d3b2e-130">Request</span></span>
<span data-ttu-id="d3b2e-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d3b2e-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d3b2e-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="d3b2e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_customers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers
```
# <a name="c"></a>[<span data-ttu-id="d3b2e-133">C#</span><span class="sxs-lookup"><span data-stu-id="d3b2e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-customers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d3b2e-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d3b2e-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-customers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d3b2e-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d3b2e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-customers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d3b2e-136">Java</span><span class="sxs-lookup"><span data-stu-id="d3b2e-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-customers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d3b2e-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3b2e-137">Response</span></span>
<span data-ttu-id="d3b2e-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d3b2e-138">The following is an example of the response.</span></span> <span data-ttu-id="d3b2e-139">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d3b2e-139">Note: The response object shown here might be shortened for readability.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List customers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
