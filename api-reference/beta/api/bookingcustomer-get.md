---
title: Получение Букингкустомер
description: Получение свойств и связей объекта Букингкустомер.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: b7285d6df368e48ac232265c99d5338254f981b6
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/07/2020
ms.locfileid: "48372189"
---
# <a name="get-bookingcustomer"></a><span data-ttu-id="db2a4-103">Получение Букингкустомер</span><span class="sxs-lookup"><span data-stu-id="db2a4-103">Get bookingCustomer</span></span>

<span data-ttu-id="db2a4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db2a4-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db2a4-105">Получение свойств и связей объекта [букингкустомер](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="db2a4-105">Get the properties and relationships of a [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="db2a4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="db2a4-106">Permissions</span></span>
<span data-ttu-id="db2a4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db2a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db2a4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="db2a4-109">Permission type</span></span>      | <span data-ttu-id="db2a4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="db2a4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db2a4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="db2a4-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="db2a4-112">Резервирования. Read. ALL, Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="db2a4-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="db2a4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="db2a4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db2a4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db2a4-114">Not supported.</span></span>   |
|<span data-ttu-id="db2a4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="db2a4-115">Application</span></span> | <span data-ttu-id="db2a4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db2a4-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="db2a4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="db2a4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/customers/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="db2a4-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="db2a4-118">Optional query parameters</span></span>
<span data-ttu-id="db2a4-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="db2a4-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="db2a4-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="db2a4-120">Request headers</span></span>
| <span data-ttu-id="db2a4-121">Имя</span><span class="sxs-lookup"><span data-stu-id="db2a4-121">Name</span></span>      |<span data-ttu-id="db2a4-122">Описание</span><span class="sxs-lookup"><span data-stu-id="db2a4-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="db2a4-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="db2a4-123">Authorization</span></span>  | <span data-ttu-id="db2a4-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="db2a4-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="db2a4-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="db2a4-125">Request body</span></span>
<span data-ttu-id="db2a4-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="db2a4-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="db2a4-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="db2a4-127">Response</span></span>
<span data-ttu-id="db2a4-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [букингкустомер](../resources/bookingcustomer.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="db2a4-128">If successful, this method returns a `200 OK` response code and [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="db2a4-129">Пример</span><span class="sxs-lookup"><span data-stu-id="db2a4-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="db2a4-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="db2a4-130">Request</span></span>
<span data-ttu-id="db2a4-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="db2a4-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="db2a4-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="db2a4-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingcustomer"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers/8bb19078-0f45-4efb-b2c5-da78b860f73a
```
# <a name="c"></a>[<span data-ttu-id="db2a4-133">C#</span><span class="sxs-lookup"><span data-stu-id="db2a4-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingcustomer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="db2a4-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db2a4-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingcustomer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="db2a4-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db2a4-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingcustomer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="db2a4-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="db2a4-136">Response</span></span>
<span data-ttu-id="db2a4-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="db2a4-137">The following is an example of the response.</span></span> <span data-ttu-id="db2a4-138">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="db2a4-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="db2a4-139">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="db2a4-139">All of the properties will be returned from an actual call.</span></span>
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
