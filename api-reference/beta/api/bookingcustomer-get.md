---
title: Get bookingCustomer
description: Получите свойства и связи объекта bookingCustomer.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 77e2a1a44a973581524dd652a33f7e9a449512a4
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047828"
---
# <a name="get-bookingcustomer"></a><span data-ttu-id="31419-103">Get bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="31419-103">Get bookingCustomer</span></span>

<span data-ttu-id="31419-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31419-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31419-105">Получите свойства и связи объекта [bookingCustomer.](../resources/bookingcustomer.md)</span><span class="sxs-lookup"><span data-stu-id="31419-105">Get the properties and relationships of a [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="31419-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="31419-106">Permissions</span></span>
<span data-ttu-id="31419-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31419-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31419-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="31419-109">Permission type</span></span>      | <span data-ttu-id="31419-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="31419-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="31419-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="31419-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="31419-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="31419-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="31419-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="31419-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31419-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31419-114">Not supported.</span></span>   |
|<span data-ttu-id="31419-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="31419-115">Application</span></span> | <span data-ttu-id="31419-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31419-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="31419-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="31419-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/customers/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="31419-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="31419-118">Optional query parameters</span></span>
<span data-ttu-id="31419-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="31419-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="31419-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="31419-120">Request headers</span></span>
| <span data-ttu-id="31419-121">Имя</span><span class="sxs-lookup"><span data-stu-id="31419-121">Name</span></span>      |<span data-ttu-id="31419-122">Описание</span><span class="sxs-lookup"><span data-stu-id="31419-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="31419-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="31419-123">Authorization</span></span>  | <span data-ttu-id="31419-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="31419-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="31419-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="31419-125">Request body</span></span>
<span data-ttu-id="31419-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="31419-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="31419-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="31419-127">Response</span></span>
<span data-ttu-id="31419-128">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект bookingCustomer](../resources/bookingcustomer.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="31419-128">If successful, this method returns a `200 OK` response code and [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="31419-129">Пример</span><span class="sxs-lookup"><span data-stu-id="31419-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="31419-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="31419-130">Request</span></span>
<span data-ttu-id="31419-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="31419-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="31419-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="31419-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingcustomer"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers/8bb19078-0f45-4efb-b2c5-da78b860f73a
```
# <a name="c"></a>[<span data-ttu-id="31419-133">C#</span><span class="sxs-lookup"><span data-stu-id="31419-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingcustomer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="31419-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="31419-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingcustomer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="31419-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="31419-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingcustomer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="31419-136">Java</span><span class="sxs-lookup"><span data-stu-id="31419-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bookingcustomer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="31419-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="31419-137">Response</span></span>
<span data-ttu-id="31419-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="31419-138">The following is an example of the response.</span></span> <span data-ttu-id="31419-139">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="31419-139">Note: The response object shown here might be shortened for readability.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get bookingCustomer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
