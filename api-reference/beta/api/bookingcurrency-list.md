---
title: Список bookingCurrencies
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
ms.openlocfilehash: 146fc1197a8ef206e78304d81c30878a67eeafad
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074761"
---
# <a name="list-bookingcurrencies"></a><span data-ttu-id="08b88-104">Список bookingCurrencies</span><span class="sxs-lookup"><span data-stu-id="08b88-104">List bookingCurrencies</span></span>

 > <span data-ttu-id="08b88-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="08b88-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="08b88-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08b88-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="08b88-107">Получите список объектов [bookingCurrency](../resources/bookingcurrency.md) , доступные для резервирования Microsoft business.</span><span class="sxs-lookup"><span data-stu-id="08b88-107">Get a list of [bookingCurrency](../resources/bookingcurrency.md) objects available to a Microsoft Bookings business.</span></span>
## <a name="permissions"></a><span data-ttu-id="08b88-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="08b88-108">Permissions</span></span>
<span data-ttu-id="08b88-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08b88-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08b88-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="08b88-111">Permission type</span></span>      | <span data-ttu-id="08b88-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="08b88-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08b88-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08b88-113">Delegated (work or school account)</span></span> | <span data-ttu-id="08b88-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="08b88-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="08b88-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08b88-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08b88-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08b88-116">Not supported.</span></span>   |
|<span data-ttu-id="08b88-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="08b88-117">Application</span></span> | <span data-ttu-id="08b88-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08b88-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="08b88-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08b88-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingCurrencies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="08b88-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="08b88-120">Optional query parameters</span></span>
<span data-ttu-id="08b88-121">Этот метод поддерживает [Параметры запроса OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) , которые помогут при настройке клиентов ответа, включая $count, $filter, $select, $skip и $top.</span><span class="sxs-lookup"><span data-stu-id="08b88-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response, including $count, $filter, $select, $skip, and $top.</span></span>

## <a name="request-headers"></a><span data-ttu-id="08b88-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="08b88-122">Request headers</span></span>
| <span data-ttu-id="08b88-123">Имя</span><span class="sxs-lookup"><span data-stu-id="08b88-123">Name</span></span>      |<span data-ttu-id="08b88-124">Описание</span><span class="sxs-lookup"><span data-stu-id="08b88-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="08b88-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="08b88-125">Authorization</span></span>  | <span data-ttu-id="08b88-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="08b88-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="08b88-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="08b88-127">Request body</span></span>
<span data-ttu-id="08b88-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="08b88-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="08b88-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="08b88-129">Response</span></span>
<span data-ttu-id="08b88-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [bookingCurrency](../resources/bookingcurrency.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="08b88-130">If successful, this method returns a `200 OK` response code and collection of [bookingCurrency](../resources/bookingcurrency.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="08b88-131">Пример</span><span class="sxs-lookup"><span data-stu-id="08b88-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="08b88-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="08b88-132">Request</span></span>
<span data-ttu-id="08b88-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="08b88-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingcurrencies"
}-->
```http
GET https://graph.microsoft.com/beta/bookingCurrencies
```
##### <a name="response"></a><span data-ttu-id="08b88-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="08b88-134">Response</span></span>
<span data-ttu-id="08b88-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="08b88-135">The following is an example of the response.</span></span> <span data-ttu-id="08b88-136">Примечание: Для краткости усекается объект ответа, показано ниже.</span><span class="sxs-lookup"><span data-stu-id="08b88-136">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="08b88-137">Все поддерживаемые валют и свойства будут возвращены из фактический вызов.</span><span class="sxs-lookup"><span data-stu-id="08b88-137">All of the supported currencies and properties will be returned from an actual call.</span></span>
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