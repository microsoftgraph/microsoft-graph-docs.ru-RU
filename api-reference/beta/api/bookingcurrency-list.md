---
title: Список БукингкурренЦиес
description: Получение списка объектов Букингкурренци, доступных для корпоративных книг Майкрософт.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: eb0b9a2e2d122083905c79be7cf540853340d40a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48960547"
---
# <a name="list-bookingcurrencies"></a><span data-ttu-id="99cee-103">Список БукингкурренЦиес</span><span class="sxs-lookup"><span data-stu-id="99cee-103">List bookingCurrencies</span></span>

<span data-ttu-id="99cee-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99cee-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99cee-105">Получение списка объектов [букингкурренци](../resources/bookingcurrency.md) , доступных для корпоративных книг Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="99cee-105">Get a list of [bookingCurrency](../resources/bookingcurrency.md) objects available to a Microsoft Bookings business.</span></span>
## <a name="permissions"></a><span data-ttu-id="99cee-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="99cee-106">Permissions</span></span>
<span data-ttu-id="99cee-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99cee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99cee-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="99cee-109">Permission type</span></span>      | <span data-ttu-id="99cee-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="99cee-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99cee-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="99cee-111">Delegated (work or school account)</span></span> | <span data-ttu-id="99cee-112">Резервирования. Read. ALL, Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="99cee-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="99cee-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="99cee-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99cee-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99cee-114">Not supported.</span></span>   |
|<span data-ttu-id="99cee-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="99cee-115">Application</span></span> | <span data-ttu-id="99cee-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99cee-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="99cee-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="99cee-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingCurrencies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="99cee-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="99cee-118">Optional query parameters</span></span>
<span data-ttu-id="99cee-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа, в том числе $count, $filter, $select, $skip и $Top.</span><span class="sxs-lookup"><span data-stu-id="99cee-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response, including $count, $filter, $select, $skip, and $top.</span></span>

## <a name="request-headers"></a><span data-ttu-id="99cee-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="99cee-120">Request headers</span></span>
| <span data-ttu-id="99cee-121">Имя</span><span class="sxs-lookup"><span data-stu-id="99cee-121">Name</span></span>      |<span data-ttu-id="99cee-122">Описание</span><span class="sxs-lookup"><span data-stu-id="99cee-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="99cee-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="99cee-123">Authorization</span></span>  | <span data-ttu-id="99cee-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="99cee-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="99cee-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="99cee-125">Request body</span></span>
<span data-ttu-id="99cee-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="99cee-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="99cee-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="99cee-127">Response</span></span>
<span data-ttu-id="99cee-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [букингкурренци](../resources/bookingcurrency.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="99cee-128">If successful, this method returns a `200 OK` response code and collection of [bookingCurrency](../resources/bookingcurrency.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="99cee-129">Пример</span><span class="sxs-lookup"><span data-stu-id="99cee-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="99cee-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="99cee-130">Request</span></span>
<span data-ttu-id="99cee-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="99cee-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="99cee-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="99cee-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingcurrencies"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingCurrencies
```
# <a name="c"></a>[<span data-ttu-id="99cee-133">C#</span><span class="sxs-lookup"><span data-stu-id="99cee-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingcurrencies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="99cee-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="99cee-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingcurrencies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="99cee-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="99cee-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingcurrencies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="99cee-136">Java</span><span class="sxs-lookup"><span data-stu-id="99cee-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bookingcurrencies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="99cee-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="99cee-137">Response</span></span>
<span data-ttu-id="99cee-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="99cee-138">The following is an example of the response.</span></span> <span data-ttu-id="99cee-139">Note: объект Response, показанный здесь, усекается для краткости.</span><span class="sxs-lookup"><span data-stu-id="99cee-139">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="99cee-140">Все поддерживаемые валюты и свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="99cee-140">All of the supported currencies and properties will be returned from an actual call.</span></span>
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
