---
title: Перечисление клиентов
description: Получение списка объектов Букингкустомер.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 413e0da2bfff04c89c157ad6aea7b13e0f1348ae
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865725"
---
# <a name="list-customers"></a><span data-ttu-id="79ede-103">Перечисление клиентов</span><span class="sxs-lookup"><span data-stu-id="79ede-103">List customers</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79ede-104">Получение списка объектов [букингкустомер](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="79ede-104">Get a list of [bookingCustomer](../resources/bookingcustomer.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="79ede-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="79ede-105">Permissions</span></span>
<span data-ttu-id="79ede-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79ede-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79ede-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79ede-108">Permission type</span></span>      | <span data-ttu-id="79ede-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="79ede-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="79ede-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79ede-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="79ede-111">Резервирования. Read. ALL, Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="79ede-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="79ede-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79ede-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79ede-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79ede-113">Not supported.</span></span>   |
|<span data-ttu-id="79ede-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="79ede-114">Application</span></span> | <span data-ttu-id="79ede-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79ede-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="79ede-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79ede-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/customers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="79ede-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="79ede-117">Optional query parameters</span></span>
<span data-ttu-id="79ede-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="79ede-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="79ede-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="79ede-119">Request headers</span></span>
| <span data-ttu-id="79ede-120">Имя</span><span class="sxs-lookup"><span data-stu-id="79ede-120">Name</span></span>      |<span data-ttu-id="79ede-121">Описание</span><span class="sxs-lookup"><span data-stu-id="79ede-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="79ede-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="79ede-122">Authorization</span></span>  | <span data-ttu-id="79ede-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="79ede-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="79ede-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="79ede-124">Request body</span></span>
<span data-ttu-id="79ede-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="79ede-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="79ede-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="79ede-126">Response</span></span>
<span data-ttu-id="79ede-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [букингкустомер](../resources/bookingcustomer.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="79ede-127">If successful, this method returns a `200 OK` response code and collection of [bookingCustomer](../resources/bookingcustomer.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="79ede-128">Пример</span><span class="sxs-lookup"><span data-stu-id="79ede-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="79ede-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="79ede-129">Request</span></span>
<span data-ttu-id="79ede-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="79ede-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="79ede-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="79ede-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_customers"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="79ede-132">C#</span><span class="sxs-lookup"><span data-stu-id="79ede-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-customers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="79ede-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="79ede-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-customers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="79ede-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="79ede-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-customers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="79ede-135">Java</span><span class="sxs-lookup"><span data-stu-id="79ede-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-customers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="79ede-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="79ede-136">Response</span></span>
<span data-ttu-id="79ede-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="79ede-137">The following is an example of the response.</span></span> <span data-ttu-id="79ede-138">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="79ede-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="79ede-139">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="79ede-139">All of the properties will be returned from an actual call.</span></span>
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
