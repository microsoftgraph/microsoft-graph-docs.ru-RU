---
title: Список БукингкурренЦиес
description: Получение списка объектов Букингкурренци, доступных для корпоративных книг Майкрософт.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: c29ad5780deac5e5e338052c72661f834e483054
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461754"
---
# <a name="list-bookingcurrencies"></a><span data-ttu-id="9e296-103">Список БукингкурренЦиес</span><span class="sxs-lookup"><span data-stu-id="9e296-103">List bookingCurrencies</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e296-104">Получение списка объектов [букингкурренци](../resources/bookingcurrency.md) , доступных для корпоративных книг Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="9e296-104">Get a list of [bookingCurrency](../resources/bookingcurrency.md) objects available to a Microsoft Bookings business.</span></span>
## <a name="permissions"></a><span data-ttu-id="9e296-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9e296-105">Permissions</span></span>
<span data-ttu-id="9e296-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e296-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e296-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9e296-108">Permission type</span></span>      | <span data-ttu-id="9e296-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9e296-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9e296-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9e296-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9e296-111">Резервирования. Read. ALL, Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="9e296-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="9e296-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9e296-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e296-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e296-113">Not supported.</span></span>   |
|<span data-ttu-id="9e296-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9e296-114">Application</span></span> | <span data-ttu-id="9e296-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e296-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="9e296-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9e296-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingCurrencies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9e296-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9e296-117">Optional query parameters</span></span>
<span data-ttu-id="9e296-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа, в том числе $count, $filter, $select, $skip и $Top.</span><span class="sxs-lookup"><span data-stu-id="9e296-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response, including $count, $filter, $select, $skip, and $top.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9e296-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9e296-119">Request headers</span></span>
| <span data-ttu-id="9e296-120">Имя</span><span class="sxs-lookup"><span data-stu-id="9e296-120">Name</span></span>      |<span data-ttu-id="9e296-121">Описание</span><span class="sxs-lookup"><span data-stu-id="9e296-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9e296-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9e296-122">Authorization</span></span>  | <span data-ttu-id="9e296-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="9e296-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e296-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9e296-124">Request body</span></span>
<span data-ttu-id="9e296-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9e296-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="9e296-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="9e296-126">Response</span></span>
<span data-ttu-id="9e296-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [букингкурренци](../resources/bookingcurrency.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9e296-127">If successful, this method returns a `200 OK` response code and collection of [bookingCurrency](../resources/bookingcurrency.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9e296-128">Пример</span><span class="sxs-lookup"><span data-stu-id="9e296-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9e296-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="9e296-129">Request</span></span>
<span data-ttu-id="9e296-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9e296-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingcurrencies"
}-->
```http
GET https://graph.microsoft.com/beta/bookingCurrencies
```
##### <a name="response"></a><span data-ttu-id="9e296-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e296-131">Response</span></span>
<span data-ttu-id="9e296-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9e296-132">The following is an example of the response.</span></span> <span data-ttu-id="9e296-133">Note: объект Response, показанный здесь, усекается для краткости.</span><span class="sxs-lookup"><span data-stu-id="9e296-133">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="9e296-134">Все поддерживаемые валюты и свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="9e296-134">All of the supported currencies and properties will be returned from an actual call.</span></span>
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
