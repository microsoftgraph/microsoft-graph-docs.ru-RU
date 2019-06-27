---
title: Список БукингкурренЦиес
description: Получение списка объектов Букингкурренци, доступных для корпоративных книг Майкрософт.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 23be76f3b2741918d414043a00a5e56017a3dad8
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35257948"
---
# <a name="list-bookingcurrencies"></a><span data-ttu-id="c8624-103">Список БукингкурренЦиес</span><span class="sxs-lookup"><span data-stu-id="c8624-103">List bookingCurrencies</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8624-104">Получение списка объектов [букингкурренци](../resources/bookingcurrency.md) , доступных для корпоративных книг Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="c8624-104">Get a list of [bookingCurrency](../resources/bookingcurrency.md) objects available to a Microsoft Bookings business.</span></span>
## <a name="permissions"></a><span data-ttu-id="c8624-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c8624-105">Permissions</span></span>
<span data-ttu-id="c8624-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8624-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8624-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c8624-108">Permission type</span></span>      | <span data-ttu-id="c8624-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c8624-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c8624-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c8624-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c8624-111">Резервирования. Read. ALL, Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="c8624-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="c8624-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c8624-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8624-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8624-113">Not supported.</span></span>   |
|<span data-ttu-id="c8624-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c8624-114">Application</span></span> | <span data-ttu-id="c8624-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8624-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="c8624-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c8624-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingCurrencies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c8624-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c8624-117">Optional query parameters</span></span>
<span data-ttu-id="c8624-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа, в том числе $count, $filter, $select, $skip и $Top.</span><span class="sxs-lookup"><span data-stu-id="c8624-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response, including $count, $filter, $select, $skip, and $top.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c8624-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c8624-119">Request headers</span></span>
| <span data-ttu-id="c8624-120">Имя</span><span class="sxs-lookup"><span data-stu-id="c8624-120">Name</span></span>      |<span data-ttu-id="c8624-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c8624-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c8624-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c8624-122">Authorization</span></span>  | <span data-ttu-id="c8624-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c8624-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8624-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c8624-124">Request body</span></span>
<span data-ttu-id="c8624-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c8624-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c8624-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="c8624-126">Response</span></span>
<span data-ttu-id="c8624-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [букингкурренци](../resources/bookingcurrency.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c8624-127">If successful, this method returns a `200 OK` response code and collection of [bookingCurrency](../resources/bookingcurrency.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c8624-128">Пример</span><span class="sxs-lookup"><span data-stu-id="c8624-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c8624-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8624-129">Request</span></span>
<span data-ttu-id="c8624-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c8624-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingcurrencies"
}-->
```http
GET https://graph.microsoft.com/beta/bookingCurrencies
```
##### <a name="response"></a><span data-ttu-id="c8624-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8624-131">Response</span></span>
<span data-ttu-id="c8624-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c8624-132">The following is an example of the response.</span></span> <span data-ttu-id="c8624-133">Note: объект Response, показанный здесь, усекается для краткости.</span><span class="sxs-lookup"><span data-stu-id="c8624-133">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="c8624-134">Все поддерживаемые валюты и свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c8624-134">All of the supported currencies and properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c8624-135">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="c8624-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c8624-136">C#</span><span class="sxs-lookup"><span data-stu-id="c8624-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_bookingcurrencies-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c8624-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="c8624-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_bookingcurrencies-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c8624-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c8624-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_bookingcurrencies-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/bookingcurrency-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/bookingcurrency-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingcurrency-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
