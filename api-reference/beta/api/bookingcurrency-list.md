---
title: Список bookingCurrencies
description: Получите список объектов bookingCurrency, доступные для резервирования Microsoft business.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: c29ad5780deac5e5e338052c72661f834e483054
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513223"
---
# <a name="list-bookingcurrencies"></a><span data-ttu-id="ceffe-103">Список bookingCurrencies</span><span class="sxs-lookup"><span data-stu-id="ceffe-103">List bookingCurrencies</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ceffe-104">Получите список объектов [bookingCurrency](../resources/bookingcurrency.md) , доступные для резервирования Microsoft business.</span><span class="sxs-lookup"><span data-stu-id="ceffe-104">Get a list of [bookingCurrency](../resources/bookingcurrency.md) objects available to a Microsoft Bookings business.</span></span>
## <a name="permissions"></a><span data-ttu-id="ceffe-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ceffe-105">Permissions</span></span>
<span data-ttu-id="ceffe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ceffe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ceffe-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ceffe-108">Permission type</span></span>      | <span data-ttu-id="ceffe-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ceffe-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ceffe-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ceffe-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ceffe-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="ceffe-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="ceffe-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ceffe-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ceffe-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ceffe-113">Not supported.</span></span>   |
|<span data-ttu-id="ceffe-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ceffe-114">Application</span></span> | <span data-ttu-id="ceffe-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ceffe-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="ceffe-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ceffe-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingCurrencies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ceffe-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ceffe-117">Optional query parameters</span></span>
<span data-ttu-id="ceffe-118">Этот метод поддерживает [Параметры запроса OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) , которые помогут при настройке клиентов ответа, включая $count, $filter, $select, $skip и $top.</span><span class="sxs-lookup"><span data-stu-id="ceffe-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response, including $count, $filter, $select, $skip, and $top.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ceffe-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ceffe-119">Request headers</span></span>
| <span data-ttu-id="ceffe-120">Имя</span><span class="sxs-lookup"><span data-stu-id="ceffe-120">Name</span></span>      |<span data-ttu-id="ceffe-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ceffe-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ceffe-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ceffe-122">Authorization</span></span>  | <span data-ttu-id="ceffe-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="ceffe-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="ceffe-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ceffe-124">Request body</span></span>
<span data-ttu-id="ceffe-125">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ceffe-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ceffe-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="ceffe-126">Response</span></span>
<span data-ttu-id="ceffe-127">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [bookingCurrency](../resources/bookingcurrency.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ceffe-127">If successful, this method returns a `200 OK` response code and collection of [bookingCurrency](../resources/bookingcurrency.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ceffe-128">Пример</span><span class="sxs-lookup"><span data-stu-id="ceffe-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ceffe-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="ceffe-129">Request</span></span>
<span data-ttu-id="ceffe-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ceffe-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingcurrencies"
}-->
```http
GET https://graph.microsoft.com/beta/bookingCurrencies
```
##### <a name="response"></a><span data-ttu-id="ceffe-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="ceffe-131">Response</span></span>
<span data-ttu-id="ceffe-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ceffe-132">The following is an example of the response.</span></span> <span data-ttu-id="ceffe-133">Примечание: Для краткости усекается объект ответа, показано ниже.</span><span class="sxs-lookup"><span data-stu-id="ceffe-133">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="ceffe-134">Все поддерживаемые валют и свойства будут возвращены из фактический вызов.</span><span class="sxs-lookup"><span data-stu-id="ceffe-134">All of the supported currencies and properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/bookingcurrency-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
