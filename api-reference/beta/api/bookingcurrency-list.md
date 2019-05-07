---
title: Список БукингкурренЦиес
description: Получение списка объектов Букингкурренци, доступных для корпоративных книг Майкрософт.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: d33f5980d41620487be95f6d2b30175b2238bb38
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636081"
---
# <a name="list-bookingcurrencies"></a><span data-ttu-id="c6152-103">Список БукингкурренЦиес</span><span class="sxs-lookup"><span data-stu-id="c6152-103">List bookingCurrencies</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6152-104">Получение списка объектов [букингкурренци](../resources/bookingcurrency.md) , доступных для корпоративных книг Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="c6152-104">Get a list of [bookingCurrency](../resources/bookingcurrency.md) objects available to a Microsoft Bookings business.</span></span>
## <a name="permissions"></a><span data-ttu-id="c6152-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c6152-105">Permissions</span></span>
<span data-ttu-id="c6152-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6152-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6152-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c6152-108">Permission type</span></span>      | <span data-ttu-id="c6152-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c6152-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6152-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c6152-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c6152-111">Резервирования. Read. ALL, Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="c6152-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="c6152-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c6152-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6152-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6152-113">Not supported.</span></span>   |
|<span data-ttu-id="c6152-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c6152-114">Application</span></span> | <span data-ttu-id="c6152-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6152-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="c6152-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c6152-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingCurrencies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c6152-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c6152-117">Optional query parameters</span></span>
<span data-ttu-id="c6152-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа, в том числе $count, $filter, $select, $skip и $Top.</span><span class="sxs-lookup"><span data-stu-id="c6152-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response, including $count, $filter, $select, $skip, and $top.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c6152-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c6152-119">Request headers</span></span>
| <span data-ttu-id="c6152-120">Имя</span><span class="sxs-lookup"><span data-stu-id="c6152-120">Name</span></span>      |<span data-ttu-id="c6152-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c6152-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c6152-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c6152-122">Authorization</span></span>  | <span data-ttu-id="c6152-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c6152-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6152-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c6152-124">Request body</span></span>
<span data-ttu-id="c6152-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c6152-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c6152-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="c6152-126">Response</span></span>
<span data-ttu-id="c6152-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [букингкурренци](../resources/bookingcurrency.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c6152-127">If successful, this method returns a `200 OK` response code and collection of [bookingCurrency](../resources/bookingcurrency.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c6152-128">Пример</span><span class="sxs-lookup"><span data-stu-id="c6152-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c6152-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="c6152-129">Request</span></span>
<span data-ttu-id="c6152-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c6152-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingcurrencies"
}-->
```http
GET https://graph.microsoft.com/beta/bookingCurrencies
```
##### <a name="response"></a><span data-ttu-id="c6152-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6152-131">Response</span></span>
<span data-ttu-id="c6152-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c6152-132">The following is an example of the response.</span></span> <span data-ttu-id="c6152-133">Note: объект Response, показанный здесь, усекается для краткости.</span><span class="sxs-lookup"><span data-stu-id="c6152-133">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="c6152-134">Все поддерживаемые валюты и свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c6152-134">All of the supported currencies and properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c6152-135">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="c6152-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c6152-136">Языках</span><span class="sxs-lookup"><span data-stu-id="c6152-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_bookingcurrencies-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c6152-137">Язык</span><span class="sxs-lookup"><span data-stu-id="c6152-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_bookingcurrencies-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/bookingcurrency-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingcurrency-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
