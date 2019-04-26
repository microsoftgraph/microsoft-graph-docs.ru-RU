---
title: Список Букингбусинессес
description: Получение коллекции объектов букингбусинесс, созданных для клиента.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 3836584a5968afb1d077546838c58836b1623166
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322595"
---
# <a name="list-bookingbusinesses"></a><span data-ttu-id="d66f7-103">Список Букингбусинессес</span><span class="sxs-lookup"><span data-stu-id="d66f7-103">List bookingBusinesses</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d66f7-104">Получение коллекции объектов [букингбусинесс](../resources/bookingbusiness.md) , созданных для клиента.</span><span class="sxs-lookup"><span data-stu-id="d66f7-104">Get a collection of [bookingbusiness](../resources/bookingbusiness.md) objects that has been created for the tenant.</span></span>

<span data-ttu-id="d66f7-105">Эта операция возвращает только **идентификаторы** и **DisplayName** для каждой из бизнесных книг в коллекции.</span><span class="sxs-lookup"><span data-stu-id="d66f7-105">This operation returns only the **id** and **displayName** of each Bookings business in the collection.</span></span> <span data-ttu-id="d66f7-106">В целях повышения производительности он не возвращает другие свойства.</span><span class="sxs-lookup"><span data-stu-id="d66f7-106">For performance considerations, it does not return other properties.</span></span> <span data-ttu-id="d66f7-107">Вы можете получить другие свойства бизнеса учета, указав его **идентификатор** в операции [Get](bookingbusiness-get.md) .</span><span class="sxs-lookup"><span data-stu-id="d66f7-107">You can get the other properties of a Bookings business by specifying its **id** in a [GET](bookingbusiness-get.md) operation.</span></span>

<span data-ttu-id="d66f7-108">Вы также можете запрашивать резервирование для предприятий, указывая строку в `query` параметре, чтобы выполнять согласование подстроки между предприятиями клиента.</span><span class="sxs-lookup"><span data-stu-id="d66f7-108">You can also query for Bookings businesses by specifying a string in a `query` parameter to do substring matching among the businesses of a tenant.</span></span> <span data-ttu-id="d66f7-109">См. [пример](#request-2) ниже.</span><span class="sxs-lookup"><span data-stu-id="d66f7-109">See an [example](#request-2) below.</span></span>


## <a name="permissions"></a><span data-ttu-id="d66f7-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d66f7-110">Permissions</span></span>
<span data-ttu-id="d66f7-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d66f7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d66f7-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d66f7-113">Permission type</span></span>      | <span data-ttu-id="d66f7-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d66f7-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d66f7-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d66f7-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="d66f7-116">Резервирования. Read. ALL, Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="d66f7-116">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="d66f7-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d66f7-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d66f7-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d66f7-118">Not supported.</span></span>   |
|<span data-ttu-id="d66f7-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d66f7-119">Application</span></span> | <span data-ttu-id="d66f7-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d66f7-120">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="d66f7-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d66f7-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d66f7-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d66f7-122">Optional query parameters</span></span>
<span data-ttu-id="d66f7-123">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d66f7-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="d66f7-124">Этот метод также поддерживает `query` параметр, который принимает строковое значение.</span><span class="sxs-lookup"><span data-stu-id="d66f7-124">This method also supports the `query` parameter which accepts a string value.</span></span> <span data-ttu-id="d66f7-125">Этот параметр позволяет ограничить результаты получения для предприятий, которые совпадают с указанной строкой.</span><span class="sxs-lookup"><span data-stu-id="d66f7-125">This parameter limits the GET results to businesses that match the specified string.</span></span> <span data-ttu-id="d66f7-126">Вы можете увидеть [Пример](#request-2) ниже.</span><span class="sxs-lookup"><span data-stu-id="d66f7-126">You can see an [example](#request-2) below.</span></span>


## <a name="request-headers"></a><span data-ttu-id="d66f7-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d66f7-127">Request headers</span></span>
| <span data-ttu-id="d66f7-128">Имя</span><span class="sxs-lookup"><span data-stu-id="d66f7-128">Name</span></span>      |<span data-ttu-id="d66f7-129">Описание</span><span class="sxs-lookup"><span data-stu-id="d66f7-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d66f7-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d66f7-130">Authorization</span></span>  | <span data-ttu-id="d66f7-131">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="d66f7-131">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="d66f7-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d66f7-132">Request body</span></span>
<span data-ttu-id="d66f7-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d66f7-133">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d66f7-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d66f7-134">Response</span></span>
<span data-ttu-id="d66f7-135">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [букингбусинесс](../resources/bookingbusiness.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d66f7-135">If successful, this method returns a `200 OK` response code and collection of [bookingBusiness](../resources/bookingbusiness.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d66f7-136">Пример</span><span class="sxs-lookup"><span data-stu-id="d66f7-136">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="d66f7-137">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="d66f7-137">Request 1</span></span>
<span data-ttu-id="d66f7-138">В приведенном ниже примере показано, как получить резервирование предприятия в клиенте.</span><span class="sxs-lookup"><span data-stu-id="d66f7-138">The following example gets the Bookings businesses in a tenant.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingbusinesses"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses
```
##### <a name="response-1"></a><span data-ttu-id="d66f7-139">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="d66f7-139">Response 1</span></span>
<span data-ttu-id="d66f7-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d66f7-140">The following is an example of the response.</span></span>
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


##### <a name="request-2"></a><span data-ttu-id="d66f7-141">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="d66f7-141">Request 2</span></span>
<span data-ttu-id="d66f7-142">В приведенном ниже примере показано, как `query` использовать этот параметр для получения одного или нескольких подходящих подходящих корпоративных подходящих подходящих подходящих подходящих корпоративных сотрудников.</span><span class="sxs-lookup"><span data-stu-id="d66f7-142">The following example shows how to use the `query` parameter to get one or more matching Bookings businesses in the tenant.</span></span>
<!-- {
  "blockType": "request",
  "name": "query_bookingbusinesses"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses?query=Adventure
```
##### <a name="response-2"></a><span data-ttu-id="d66f7-143">Ответ 2</span><span class="sxs-lookup"><span data-stu-id="d66f7-143">Response 2</span></span>
<span data-ttu-id="d66f7-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d66f7-144">The following is an example of the response.</span></span>
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
  "suppressions": []
}
-->
