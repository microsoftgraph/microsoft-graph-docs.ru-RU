---
title: Список bookingBusinesses
description: Получите коллекцию объектов bookingbusiness, которые были созданы для клиента.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 8018b8ac7f9d2e5f74e4233dbc36c2a6faa2d9a8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523157"
---
# <a name="list-bookingbusinesses"></a><span data-ttu-id="e5c3a-103">Список bookingBusinesses</span><span class="sxs-lookup"><span data-stu-id="e5c3a-103">List bookingBusinesses</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5c3a-104">Получите коллекцию объектов [bookingbusiness](../resources/bookingbusiness.md) , которые были созданы для клиента.</span><span class="sxs-lookup"><span data-stu-id="e5c3a-104">Get a collection of [bookingbusiness](../resources/bookingbusiness.md) objects that has been created for the tenant.</span></span>

<span data-ttu-id="e5c3a-105">Эта операция возвращает **идентификатор** и **отображаемое имя** каждого business резервирования в коллекции.</span><span class="sxs-lookup"><span data-stu-id="e5c3a-105">This operation returns only the **id** and **displayName** of each Bookings business in the collection.</span></span> <span data-ttu-id="e5c3a-106">По соображениям производительности он не возвращает другие свойства.</span><span class="sxs-lookup"><span data-stu-id="e5c3a-106">For performance considerations, it does not return other properties.</span></span> <span data-ttu-id="e5c3a-107">Другие свойства business резервирования можно получить, указав его **идентификатор** в операции [GET](bookingbusiness-get.md) .</span><span class="sxs-lookup"><span data-stu-id="e5c3a-107">You can get the other properties of a Bookings business by specifying its **id** in a [GET](bookingbusiness-get.md) operation.</span></span>

<span data-ttu-id="e5c3a-108">Также можно запрашивать для резервирования бизнеса путем указания строки в `query` параметр совпадение между бизнеса клиента строк.</span><span class="sxs-lookup"><span data-stu-id="e5c3a-108">You can also query for Bookings businesses by specifying a string in a `query` parameter to do substring matching among the businesses of a tenant.</span></span> <span data-ttu-id="e5c3a-109">См. [пример](#request-2) ниже.</span><span class="sxs-lookup"><span data-stu-id="e5c3a-109">See an [example](#request-2) below.</span></span>


## <a name="permissions"></a><span data-ttu-id="e5c3a-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e5c3a-110">Permissions</span></span>
<span data-ttu-id="e5c3a-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5c3a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5c3a-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5c3a-113">Permission type</span></span>      | <span data-ttu-id="e5c3a-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5c3a-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5c3a-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5c3a-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="e5c3a-116">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="e5c3a-116">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="e5c3a-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5c3a-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5c3a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5c3a-118">Not supported.</span></span>   |
|<span data-ttu-id="e5c3a-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e5c3a-119">Application</span></span> | <span data-ttu-id="e5c3a-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5c3a-120">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="e5c3a-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5c3a-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e5c3a-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e5c3a-122">Optional query parameters</span></span>
<span data-ttu-id="e5c3a-123">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e5c3a-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="e5c3a-124">Этот метод также поддерживает `query` параметр, который принимает значение типа string.</span><span class="sxs-lookup"><span data-stu-id="e5c3a-124">This method also supports the `query` parameter which accepts a string value.</span></span> <span data-ttu-id="e5c3a-125">Этот параметр ограничивает результаты GET для предприятий, которые соответствуют указанной строке.</span><span class="sxs-lookup"><span data-stu-id="e5c3a-125">This parameter limits the GET results to businesses that match the specified string.</span></span> <span data-ttu-id="e5c3a-126">Можно приведенном ниже [примере](#request-2) .</span><span class="sxs-lookup"><span data-stu-id="e5c3a-126">You can see an [example](#request-2) below.</span></span>


## <a name="request-headers"></a><span data-ttu-id="e5c3a-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e5c3a-127">Request headers</span></span>
| <span data-ttu-id="e5c3a-128">Имя</span><span class="sxs-lookup"><span data-stu-id="e5c3a-128">Name</span></span>      |<span data-ttu-id="e5c3a-129">Описание</span><span class="sxs-lookup"><span data-stu-id="e5c3a-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e5c3a-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5c3a-130">Authorization</span></span>  | <span data-ttu-id="e5c3a-131">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="e5c3a-131">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5c3a-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e5c3a-132">Request body</span></span>
<span data-ttu-id="e5c3a-133">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e5c3a-133">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e5c3a-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="e5c3a-134">Response</span></span>
<span data-ttu-id="e5c3a-135">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [bookingBusiness](../resources/bookingbusiness.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e5c3a-135">If successful, this method returns a `200 OK` response code and collection of [bookingBusiness](../resources/bookingbusiness.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e5c3a-136">Пример</span><span class="sxs-lookup"><span data-stu-id="e5c3a-136">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="e5c3a-137">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="e5c3a-137">Request 1</span></span>
<span data-ttu-id="e5c3a-138">В следующем примере получается предприятий резервирования в клиент.</span><span class="sxs-lookup"><span data-stu-id="e5c3a-138">The following example gets the Bookings businesses in a tenant.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingbusinesses"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses
```
##### <a name="response-1"></a><span data-ttu-id="e5c3a-139">Ответ 1</span><span class="sxs-lookup"><span data-stu-id="e5c3a-139">Response 1</span></span>
<span data-ttu-id="e5c3a-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e5c3a-140">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingBusiness",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#bookingBusinesses",
    "value":[
        {
            "id":"Contosolunchdelivery@M365B489948.onmicrosoft.com",
            "displayName":"Contoso lunch delivery",
        },
        {
            "id":"Fabrikam@M365B489948.onmicrosoft.com",
            "displayName":"Fabrikam",
        }
    ]
}
```


##### <a name="request-2"></a><span data-ttu-id="e5c3a-141">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="e5c3a-141">Request 2</span></span>
<span data-ttu-id="e5c3a-142">Следующий пример демонстрирует использование `query` параметр для получения совпадающих предприятий резервирования в клиента.</span><span class="sxs-lookup"><span data-stu-id="e5c3a-142">The following example shows how to use the `query` parameter to get one or more matching Bookings businesses in the tenant.</span></span>
<!-- {
  "blockType": "request",
  "name": "query_bookingbusinesses"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses?query=Adventure
```
##### <a name="response-2"></a><span data-ttu-id="e5c3a-143">Ответ 2</span><span class="sxs-lookup"><span data-stu-id="e5c3a-143">Response 2</span></span>
<span data-ttu-id="e5c3a-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e5c3a-144">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingBusiness",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#bookingBusinesses",
    "value":[
        {
            "id":"AdventureWorksCycles@M365B960066.onmicrosoft.com",
            "displayName":"Adventure Works Cycles",
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List bookingBusinesses",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingbusiness-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
