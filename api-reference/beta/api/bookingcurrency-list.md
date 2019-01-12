---
title: Список bookingCurrencies
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: e08385c887b1da6972caab83da068b0e537586db
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941522"
---
# <a name="list-bookingcurrencies"></a><span data-ttu-id="6359b-104">Список bookingCurrencies</span><span class="sxs-lookup"><span data-stu-id="6359b-104">List bookingCurrencies</span></span>

 > <span data-ttu-id="6359b-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6359b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6359b-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6359b-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="6359b-107">Получите список объектов [bookingCurrency](../resources/bookingcurrency.md) , доступные для резервирования Microsoft business.</span><span class="sxs-lookup"><span data-stu-id="6359b-107">Get a list of [bookingCurrency](../resources/bookingcurrency.md) objects available to a Microsoft Bookings business.</span></span>
## <a name="permissions"></a><span data-ttu-id="6359b-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6359b-108">Permissions</span></span>
<span data-ttu-id="6359b-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6359b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6359b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6359b-111">Permission type</span></span>      | <span data-ttu-id="6359b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6359b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6359b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6359b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="6359b-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="6359b-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="6359b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6359b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6359b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6359b-116">Not supported.</span></span>   |
|<span data-ttu-id="6359b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6359b-117">Application</span></span> | <span data-ttu-id="6359b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6359b-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="6359b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6359b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingCurrencies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6359b-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6359b-120">Optional query parameters</span></span>
<span data-ttu-id="6359b-121">Этот метод поддерживает [Параметры запроса OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) , которые помогут при настройке клиентов ответа, включая $count, $filter, $select, $skip и $top.</span><span class="sxs-lookup"><span data-stu-id="6359b-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response, including $count, $filter, $select, $skip, and $top.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6359b-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6359b-122">Request headers</span></span>
| <span data-ttu-id="6359b-123">Имя</span><span class="sxs-lookup"><span data-stu-id="6359b-123">Name</span></span>      |<span data-ttu-id="6359b-124">Описание</span><span class="sxs-lookup"><span data-stu-id="6359b-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6359b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="6359b-125">Authorization</span></span>  | <span data-ttu-id="6359b-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="6359b-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="6359b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6359b-127">Request body</span></span>
<span data-ttu-id="6359b-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6359b-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="6359b-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="6359b-129">Response</span></span>
<span data-ttu-id="6359b-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [bookingCurrency](../resources/bookingcurrency.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6359b-130">If successful, this method returns a `200 OK` response code and collection of [bookingCurrency](../resources/bookingcurrency.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6359b-131">Пример</span><span class="sxs-lookup"><span data-stu-id="6359b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6359b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="6359b-132">Request</span></span>
<span data-ttu-id="6359b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6359b-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingcurrencies"
}-->
```http
GET https://graph.microsoft.com/beta/bookingCurrencies
```
##### <a name="response"></a><span data-ttu-id="6359b-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="6359b-134">Response</span></span>
<span data-ttu-id="6359b-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6359b-135">The following is an example of the response.</span></span> <span data-ttu-id="6359b-136">Примечание: Для краткости усекается объект ответа, показано ниже.</span><span class="sxs-lookup"><span data-stu-id="6359b-136">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="6359b-137">Все поддерживаемые валют и свойства будут возвращены из фактический вызов.</span><span class="sxs-lookup"><span data-stu-id="6359b-137">All of the supported currencies and properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List bookingCurrencies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
