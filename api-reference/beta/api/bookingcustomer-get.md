---
title: Получение Букингкустомер
description: Получение свойств и связей объекта Букингкустомер.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 5ba1aede8d6f9a211c8b8827106b9fca9fc8b41d
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36718823"
---
# <a name="get-bookingcustomer"></a><span data-ttu-id="066db-103">Получение Букингкустомер</span><span class="sxs-lookup"><span data-stu-id="066db-103">Get bookingCustomer</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="066db-104">Получение свойств и связей объекта [букингкустомер](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="066db-104">Get the properties and relationships of a [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="066db-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="066db-105">Permissions</span></span>
<span data-ttu-id="066db-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="066db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="066db-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="066db-108">Permission type</span></span>      | <span data-ttu-id="066db-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="066db-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="066db-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="066db-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="066db-111">Резервирования. Read. ALL, Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="066db-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="066db-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="066db-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="066db-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="066db-113">Not supported.</span></span>   |
|<span data-ttu-id="066db-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="066db-114">Application</span></span> | <span data-ttu-id="066db-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="066db-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="066db-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="066db-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/customers/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="066db-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="066db-117">Optional query parameters</span></span>
<span data-ttu-id="066db-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="066db-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="066db-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="066db-119">Request headers</span></span>
| <span data-ttu-id="066db-120">Имя</span><span class="sxs-lookup"><span data-stu-id="066db-120">Name</span></span>      |<span data-ttu-id="066db-121">Описание</span><span class="sxs-lookup"><span data-stu-id="066db-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="066db-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="066db-122">Authorization</span></span>  | <span data-ttu-id="066db-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="066db-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="066db-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="066db-124">Request body</span></span>
<span data-ttu-id="066db-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="066db-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="066db-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="066db-126">Response</span></span>
<span data-ttu-id="066db-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [букингкустомер](../resources/bookingcustomer.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="066db-127">If successful, this method returns a `200 OK` response code and [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="066db-128">Пример</span><span class="sxs-lookup"><span data-stu-id="066db-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="066db-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="066db-129">Request</span></span>
<span data-ttu-id="066db-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="066db-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="066db-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="066db-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingcustomer"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers/8bb19078-0f45-4efb-b2c5-da78b860f73a
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="066db-132">C#</span><span class="sxs-lookup"><span data-stu-id="066db-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingcustomer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="066db-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="066db-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingcustomer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="066db-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="066db-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingcustomer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="066db-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="066db-135">Response</span></span>
<span data-ttu-id="066db-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="066db-136">The following is an example of the response.</span></span> <span data-ttu-id="066db-137">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="066db-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="066db-138">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="066db-138">All of the properties will be returned from an actual call.</span></span>
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
