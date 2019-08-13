---
title: Список БукингкурренЦиес
description: Получение списка объектов Букингкурренци, доступных для корпоративных книг Майкрософт.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: ae3c358644156ce700f59b410ed83ae7ca283b44
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36318168"
---
# <a name="list-bookingcurrencies"></a><span data-ttu-id="0ead4-103">Список БукингкурренЦиес</span><span class="sxs-lookup"><span data-stu-id="0ead4-103">List bookingCurrencies</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ead4-104">Получение списка объектов [букингкурренци](../resources/bookingcurrency.md) , доступных для корпоративных книг Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="0ead4-104">Get a list of [bookingCurrency](../resources/bookingcurrency.md) objects available to a Microsoft Bookings business.</span></span>
## <a name="permissions"></a><span data-ttu-id="0ead4-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0ead4-105">Permissions</span></span>
<span data-ttu-id="0ead4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ead4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ead4-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ead4-108">Permission type</span></span>      | <span data-ttu-id="0ead4-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ead4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ead4-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ead4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0ead4-111">Резервирования. Read. ALL, Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="0ead4-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="0ead4-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ead4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ead4-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ead4-113">Not supported.</span></span>   |
|<span data-ttu-id="0ead4-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0ead4-114">Application</span></span> | <span data-ttu-id="0ead4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ead4-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="0ead4-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ead4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingCurrencies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0ead4-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0ead4-117">Optional query parameters</span></span>
<span data-ttu-id="0ead4-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа, в том числе $count, $filter, $select, $skip и $Top.</span><span class="sxs-lookup"><span data-stu-id="0ead4-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response, including $count, $filter, $select, $skip, and $top.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0ead4-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0ead4-119">Request headers</span></span>
| <span data-ttu-id="0ead4-120">Имя</span><span class="sxs-lookup"><span data-stu-id="0ead4-120">Name</span></span>      |<span data-ttu-id="0ead4-121">Описание</span><span class="sxs-lookup"><span data-stu-id="0ead4-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0ead4-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0ead4-122">Authorization</span></span>  | <span data-ttu-id="0ead4-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="0ead4-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ead4-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0ead4-124">Request body</span></span>
<span data-ttu-id="0ead4-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0ead4-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="0ead4-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ead4-126">Response</span></span>
<span data-ttu-id="0ead4-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [букингкурренци](../resources/bookingcurrency.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0ead4-127">If successful, this method returns a `200 OK` response code and collection of [bookingCurrency](../resources/bookingcurrency.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0ead4-128">Пример</span><span class="sxs-lookup"><span data-stu-id="0ead4-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0ead4-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ead4-129">Request</span></span>
<span data-ttu-id="0ead4-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0ead4-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0ead4-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="0ead4-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingcurrencies"
}-->
```http
GET https://graph.microsoft.com/beta/bookingCurrencies
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0ead4-132">C#</span><span class="sxs-lookup"><span data-stu-id="0ead4-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingcurrencies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0ead4-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0ead4-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingcurrencies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0ead4-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="0ead4-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingcurrencies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0ead4-135">Java</span><span class="sxs-lookup"><span data-stu-id="0ead4-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bookingcurrencies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0ead4-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ead4-136">Response</span></span>
<span data-ttu-id="0ead4-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0ead4-137">The following is an example of the response.</span></span> <span data-ttu-id="0ead4-138">Note: объект Response, показанный здесь, усекается для краткости.</span><span class="sxs-lookup"><span data-stu-id="0ead4-138">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="0ead4-139">Все поддерживаемые валюты и свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0ead4-139">All of the supported currencies and properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCurrency",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#bookingCurrencies",
    "value":[
        {
            "id":"AED",
            "symbol":"د.إ.‏"
        },
        {
            "id":"AFN",
            "symbol":"؋"
        },
        {
            "id":"ALL",
            "symbol":"Lekë"
        },
        {
            "id":"AMD",
            "symbol":"֏"
        },
        {
            "id":"USD",
            "symbol":"$"
        },
        {
            "id":"YER",
            "symbol":"ر.ي.‏"
        },
        {
            "id":"ZAR",
            "symbol":"R"
        },
        {
            "id":"ZMW",
            "symbol":"K"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List bookingCurrencies",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
