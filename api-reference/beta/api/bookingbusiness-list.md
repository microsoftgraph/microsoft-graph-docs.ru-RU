---
title: Список bookingBusinesses
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 51b8e049b45542de9940168c994bed8fbd273b60
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951455"
---
# <a name="list-bookingbusinesses"></a><span data-ttu-id="b807d-104">Список bookingBusinesses</span><span class="sxs-lookup"><span data-stu-id="b807d-104">List bookingBusinesses</span></span>

 > <span data-ttu-id="b807d-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b807d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b807d-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b807d-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="b807d-107">Получите коллекцию объектов [bookingbusiness](../resources/bookingbusiness.md) , которые были созданы для клиента.</span><span class="sxs-lookup"><span data-stu-id="b807d-107">Get a collection of [bookingbusiness](../resources/bookingbusiness.md) objects that has been created for the tenant.</span></span> 

<span data-ttu-id="b807d-108">Эта операция возвращает **идентификатор** и **отображаемое имя** каждого business резервирования в коллекции.</span><span class="sxs-lookup"><span data-stu-id="b807d-108">This operation returns only the **id** and **displayName** of each Bookings business in the collection.</span></span> <span data-ttu-id="b807d-109">По соображениям производительности он не возвращает другие свойства.</span><span class="sxs-lookup"><span data-stu-id="b807d-109">For performance considerations, it does not return other properties.</span></span> <span data-ttu-id="b807d-110">Другие свойства business резервирования можно получить, указав его **идентификатор** в операции [GET](bookingbusiness-get.md) .</span><span class="sxs-lookup"><span data-stu-id="b807d-110">You can get the other properties of a Bookings business by specifying its **id** in a [GET](bookingbusiness-get.md) operation.</span></span>

<span data-ttu-id="b807d-111">Также можно запрашивать для резервирования бизнеса путем указания строки в `query` параметр совпадение между бизнеса клиента строк.</span><span class="sxs-lookup"><span data-stu-id="b807d-111">You can also query for Bookings businesses by specifying a string in a `query` parameter to do substring matching among the businesses of a tenant.</span></span> <span data-ttu-id="b807d-112">В приведенном ниже [примере](#request-2) .</span><span class="sxs-lookup"><span data-stu-id="b807d-112">See an [example](#request-2) below.</span></span>


## <a name="permissions"></a><span data-ttu-id="b807d-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b807d-113">Permissions</span></span>
<span data-ttu-id="b807d-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b807d-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b807d-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b807d-116">Permission type</span></span>      | <span data-ttu-id="b807d-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b807d-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b807d-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b807d-118">Delegated (work or school account)</span></span> |  <span data-ttu-id="b807d-119">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="b807d-119">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="b807d-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b807d-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b807d-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b807d-121">Not supported.</span></span>   |
|<span data-ttu-id="b807d-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b807d-122">Application</span></span> | <span data-ttu-id="b807d-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b807d-123">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="b807d-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b807d-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b807d-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b807d-125">Optional query parameters</span></span>
<span data-ttu-id="b807d-126">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b807d-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="b807d-127">Этот метод также поддерживает `query` параметр, который принимает значение типа string.</span><span class="sxs-lookup"><span data-stu-id="b807d-127">This method also supports the `query` parameter which accepts a string value.</span></span> <span data-ttu-id="b807d-128">Этот параметр ограничивает результаты GET для предприятий, которые соответствуют указанной строке.</span><span class="sxs-lookup"><span data-stu-id="b807d-128">This parameter limits the GET results to businesses that match the specified string.</span></span> <span data-ttu-id="b807d-129">Можно приведенном ниже [примере](#request-2) .</span><span class="sxs-lookup"><span data-stu-id="b807d-129">You can see an [example](#request-2) below.</span></span>


## <a name="request-headers"></a><span data-ttu-id="b807d-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b807d-130">Request headers</span></span>
| <span data-ttu-id="b807d-131">Имя</span><span class="sxs-lookup"><span data-stu-id="b807d-131">Name</span></span>      |<span data-ttu-id="b807d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b807d-132">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b807d-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="b807d-133">Authorization</span></span>  | <span data-ttu-id="b807d-134">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="b807d-134">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="b807d-135">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b807d-135">Request body</span></span>
<span data-ttu-id="b807d-136">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b807d-136">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b807d-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="b807d-137">Response</span></span>
<span data-ttu-id="b807d-138">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [bookingBusiness](../resources/bookingbusiness.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b807d-138">If successful, this method returns a `200 OK` response code and collection of [bookingBusiness](../resources/bookingbusiness.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b807d-139">Пример</span><span class="sxs-lookup"><span data-stu-id="b807d-139">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="b807d-140">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="b807d-140">Request 1</span></span>
<span data-ttu-id="b807d-141">В следующем примере получается предприятий резервирования в клиент.</span><span class="sxs-lookup"><span data-stu-id="b807d-141">The following example gets the Bookings businesses in a tenant.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingbusinesses"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses
```
##### <a name="response-1"></a><span data-ttu-id="b807d-142">Ответ 1</span><span class="sxs-lookup"><span data-stu-id="b807d-142">Response 1</span></span>
<span data-ttu-id="b807d-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b807d-143">The following is an example of the response.</span></span>
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


##### <a name="request-2"></a><span data-ttu-id="b807d-144">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="b807d-144">Request 2</span></span>
<span data-ttu-id="b807d-145">Следующий пример демонстрирует использование `query` параметр для получения совпадающих предприятий резервирования в клиента.</span><span class="sxs-lookup"><span data-stu-id="b807d-145">The following example shows how to use the `query` parameter to get one or more matching Bookings businesses in the tenant.</span></span>
<!-- {
  "blockType": "request",
  "name": "query_bookingbusinesses"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses?query=Adventure
```
##### <a name="response-2"></a><span data-ttu-id="b807d-146">Ответ 2</span><span class="sxs-lookup"><span data-stu-id="b807d-146">Response 2</span></span>
<span data-ttu-id="b807d-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b807d-147">The following is an example of the response.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List bookingBusinesses",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
