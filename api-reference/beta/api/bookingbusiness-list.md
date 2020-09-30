---
title: Список Букингбусинессес
description: Получение коллекции объектов букингбусинесс, созданных для клиента.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 2a3e2ad3923e7404b72a5e612c5f776b22a8bbad
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/30/2020
ms.locfileid: "48312738"
---
# <a name="list-bookingbusinesses"></a><span data-ttu-id="fde3a-103">Список Букингбусинессес</span><span class="sxs-lookup"><span data-stu-id="fde3a-103">List bookingBusinesses</span></span>

<span data-ttu-id="fde3a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fde3a-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fde3a-105">Получение коллекции объектов [букингбусинесс](../resources/bookingbusiness.md) , созданных для клиента.</span><span class="sxs-lookup"><span data-stu-id="fde3a-105">Get a collection of [bookingbusiness](../resources/bookingbusiness.md) objects that has been created for the tenant.</span></span>

<span data-ttu-id="fde3a-106">Эта операция возвращает только **идентификаторы** и **DisplayName** для каждой из бизнесных книг в коллекции.</span><span class="sxs-lookup"><span data-stu-id="fde3a-106">This operation returns only the **id** and **displayName** of each Bookings business in the collection.</span></span> <span data-ttu-id="fde3a-107">В целях повышения производительности он не возвращает другие свойства.</span><span class="sxs-lookup"><span data-stu-id="fde3a-107">For performance considerations, it does not return other properties.</span></span> <span data-ttu-id="fde3a-108">Вы можете получить другие свойства бизнеса учета, указав его **идентификатор** в операции [Get](bookingbusiness-get.md) .</span><span class="sxs-lookup"><span data-stu-id="fde3a-108">You can get the other properties of a Bookings business by specifying its **id** in a [GET](bookingbusiness-get.md) operation.</span></span>

<span data-ttu-id="fde3a-109">Вы также можете запрашивать резервирование для предприятий, указывая строку в `query` параметре, чтобы выполнять согласование подстроки между предприятиями клиента.</span><span class="sxs-lookup"><span data-stu-id="fde3a-109">You can also query for Bookings businesses by specifying a string in a `query` parameter to do substring matching among the businesses of a tenant.</span></span> <span data-ttu-id="fde3a-110">См. [пример](#request-2) ниже.</span><span class="sxs-lookup"><span data-stu-id="fde3a-110">See an [example](#request-2) below.</span></span>


## <a name="permissions"></a><span data-ttu-id="fde3a-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fde3a-111">Permissions</span></span>
<span data-ttu-id="fde3a-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fde3a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fde3a-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fde3a-114">Permission type</span></span>      | <span data-ttu-id="fde3a-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fde3a-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fde3a-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fde3a-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="fde3a-117">Резервирования. Read. ALL, Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="fde3a-117">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="fde3a-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fde3a-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fde3a-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fde3a-119">Not supported.</span></span>   |
|<span data-ttu-id="fde3a-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fde3a-120">Application</span></span> | <span data-ttu-id="fde3a-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fde3a-121">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="fde3a-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fde3a-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fde3a-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fde3a-123">Optional query parameters</span></span>
<span data-ttu-id="fde3a-124">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fde3a-124">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="fde3a-125">Этот метод также поддерживает `query` параметр, который принимает строковое значение.</span><span class="sxs-lookup"><span data-stu-id="fde3a-125">This method also supports the `query` parameter which accepts a string value.</span></span> <span data-ttu-id="fde3a-126">Этот параметр позволяет ограничить результаты получения для предприятий, которые совпадают с указанной строкой.</span><span class="sxs-lookup"><span data-stu-id="fde3a-126">This parameter limits the GET results to businesses that match the specified string.</span></span> <span data-ttu-id="fde3a-127">Вы можете увидеть [Пример](#request-2) ниже.</span><span class="sxs-lookup"><span data-stu-id="fde3a-127">You can see an [example](#request-2) below.</span></span>


## <a name="request-headers"></a><span data-ttu-id="fde3a-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fde3a-128">Request headers</span></span>
| <span data-ttu-id="fde3a-129">Имя</span><span class="sxs-lookup"><span data-stu-id="fde3a-129">Name</span></span>      |<span data-ttu-id="fde3a-130">Описание</span><span class="sxs-lookup"><span data-stu-id="fde3a-130">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fde3a-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fde3a-131">Authorization</span></span>  | <span data-ttu-id="fde3a-132">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="fde3a-132">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="fde3a-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fde3a-133">Request body</span></span>
<span data-ttu-id="fde3a-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fde3a-134">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="fde3a-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="fde3a-135">Response</span></span>
<span data-ttu-id="fde3a-136">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [букингбусинесс](../resources/bookingbusiness.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fde3a-136">If successful, this method returns a `200 OK` response code and collection of [bookingBusiness](../resources/bookingbusiness.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fde3a-137">Пример</span><span class="sxs-lookup"><span data-stu-id="fde3a-137">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="fde3a-138">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="fde3a-138">Request 1</span></span>
<span data-ttu-id="fde3a-139">В приведенном ниже примере показано, как получить резервирование предприятия в клиенте.</span><span class="sxs-lookup"><span data-stu-id="fde3a-139">The following example gets the Bookings businesses in a tenant.</span></span>

# <a name="http"></a>[<span data-ttu-id="fde3a-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="fde3a-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingbusinesses"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingBusinesses
```
# <a name="c"></a>[<span data-ttu-id="fde3a-141">C#</span><span class="sxs-lookup"><span data-stu-id="fde3a-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingbusinesses-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fde3a-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fde3a-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingbusinesses-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fde3a-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fde3a-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingbusinesses-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-1"></a><span data-ttu-id="fde3a-144">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="fde3a-144">Response 1</span></span>
<span data-ttu-id="fde3a-145">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="fde3a-145">The following is an example of the response.</span></span>
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


##### <a name="request-2"></a><span data-ttu-id="fde3a-146">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="fde3a-146">Request 2</span></span>
<span data-ttu-id="fde3a-147">В приведенном ниже примере показано, как использовать этот `query` параметр для получения одного или нескольких подходящих подходящих корпоративных подходящих подходящих подходящих подходящих корпоративных сотрудников.</span><span class="sxs-lookup"><span data-stu-id="fde3a-147">The following example shows how to use the `query` parameter to get one or more matching Bookings businesses in the tenant.</span></span>

# <a name="http"></a>[<span data-ttu-id="fde3a-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="fde3a-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "query_bookingbusinesses"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingBusinesses?query=Adventure
```
# <a name="c"></a>[<span data-ttu-id="fde3a-149">C#</span><span class="sxs-lookup"><span data-stu-id="fde3a-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/query-bookingbusinesses-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fde3a-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fde3a-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/query-bookingbusinesses-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fde3a-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fde3a-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/query-bookingbusinesses-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-2"></a><span data-ttu-id="fde3a-152">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="fde3a-152">Response 2</span></span>
<span data-ttu-id="fde3a-153">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="fde3a-153">The following is an example of the response.</span></span>
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
  ]
}
-->