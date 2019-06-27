---
title: Список Букингбусинессес
description: Получение коллекции объектов букингбусинесс, созданных для клиента.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: ef7581d9e87cdc2e367fe557fbc9a15b018c78c6
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258109"
---
# <a name="list-bookingbusinesses"></a><span data-ttu-id="d02e3-103">Список Букингбусинессес</span><span class="sxs-lookup"><span data-stu-id="d02e3-103">List bookingBusinesses</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d02e3-104">Получение коллекции объектов [букингбусинесс](../resources/bookingbusiness.md) , созданных для клиента.</span><span class="sxs-lookup"><span data-stu-id="d02e3-104">Get a collection of [bookingbusiness](../resources/bookingbusiness.md) objects that has been created for the tenant.</span></span>

<span data-ttu-id="d02e3-105">Эта операция возвращает только **идентификаторы** и **DisplayName** для каждой из бизнесных книг в коллекции.</span><span class="sxs-lookup"><span data-stu-id="d02e3-105">This operation returns only the **id** and **displayName** of each Bookings business in the collection.</span></span> <span data-ttu-id="d02e3-106">В целях повышения производительности он не возвращает другие свойства.</span><span class="sxs-lookup"><span data-stu-id="d02e3-106">For performance considerations, it does not return other properties.</span></span> <span data-ttu-id="d02e3-107">Вы можете получить другие свойства бизнеса учета, указав его **идентификатор** в операции [Get](bookingbusiness-get.md) .</span><span class="sxs-lookup"><span data-stu-id="d02e3-107">You can get the other properties of a Bookings business by specifying its **id** in a [GET](bookingbusiness-get.md) operation.</span></span>

<span data-ttu-id="d02e3-108">Вы также можете запрашивать резервирование для предприятий, указывая строку в `query` параметре, чтобы выполнять согласование подстроки между предприятиями клиента.</span><span class="sxs-lookup"><span data-stu-id="d02e3-108">You can also query for Bookings businesses by specifying a string in a `query` parameter to do substring matching among the businesses of a tenant.</span></span> <span data-ttu-id="d02e3-109">См. [пример](#request-2) ниже.</span><span class="sxs-lookup"><span data-stu-id="d02e3-109">See an [example](#request-2) below.</span></span>


## <a name="permissions"></a><span data-ttu-id="d02e3-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d02e3-110">Permissions</span></span>
<span data-ttu-id="d02e3-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d02e3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d02e3-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d02e3-113">Permission type</span></span>      | <span data-ttu-id="d02e3-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d02e3-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d02e3-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d02e3-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="d02e3-116">Резервирования. Read. ALL, Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="d02e3-116">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="d02e3-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d02e3-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d02e3-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d02e3-118">Not supported.</span></span>   |
|<span data-ttu-id="d02e3-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d02e3-119">Application</span></span> | <span data-ttu-id="d02e3-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d02e3-120">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="d02e3-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d02e3-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d02e3-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d02e3-122">Optional query parameters</span></span>
<span data-ttu-id="d02e3-123">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d02e3-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="d02e3-124">Этот метод также поддерживает `query` параметр, который принимает строковое значение.</span><span class="sxs-lookup"><span data-stu-id="d02e3-124">This method also supports the `query` parameter which accepts a string value.</span></span> <span data-ttu-id="d02e3-125">Этот параметр позволяет ограничить результаты получения для предприятий, которые совпадают с указанной строкой.</span><span class="sxs-lookup"><span data-stu-id="d02e3-125">This parameter limits the GET results to businesses that match the specified string.</span></span> <span data-ttu-id="d02e3-126">Вы можете увидеть [Пример](#request-2) ниже.</span><span class="sxs-lookup"><span data-stu-id="d02e3-126">You can see an [example](#request-2) below.</span></span>


## <a name="request-headers"></a><span data-ttu-id="d02e3-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d02e3-127">Request headers</span></span>
| <span data-ttu-id="d02e3-128">Имя</span><span class="sxs-lookup"><span data-stu-id="d02e3-128">Name</span></span>      |<span data-ttu-id="d02e3-129">Описание</span><span class="sxs-lookup"><span data-stu-id="d02e3-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d02e3-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d02e3-130">Authorization</span></span>  | <span data-ttu-id="d02e3-131">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="d02e3-131">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="d02e3-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d02e3-132">Request body</span></span>
<span data-ttu-id="d02e3-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d02e3-133">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d02e3-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d02e3-134">Response</span></span>
<span data-ttu-id="d02e3-135">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [букингбусинесс](../resources/bookingbusiness.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d02e3-135">If successful, this method returns a `200 OK` response code and collection of [bookingBusiness](../resources/bookingbusiness.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d02e3-136">Пример</span><span class="sxs-lookup"><span data-stu-id="d02e3-136">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="d02e3-137">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="d02e3-137">Request 1</span></span>
<span data-ttu-id="d02e3-138">В приведенном ниже примере показано, как получить резервирование предприятия в клиенте.</span><span class="sxs-lookup"><span data-stu-id="d02e3-138">The following example gets the Bookings businesses in a tenant.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingbusinesses"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses
```
##### <a name="response-1"></a><span data-ttu-id="d02e3-139">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="d02e3-139">Response 1</span></span>
<span data-ttu-id="d02e3-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d02e3-140">The following is an example of the response.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d02e3-141">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="d02e3-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d02e3-142">C#</span><span class="sxs-lookup"><span data-stu-id="d02e3-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_bookingbusinesses-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d02e3-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="d02e3-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_bookingbusinesses-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d02e3-144">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d02e3-144">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_bookingbusinesses-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


##### <a name="request-2"></a><span data-ttu-id="d02e3-145">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="d02e3-145">Request 2</span></span>
<span data-ttu-id="d02e3-146">В приведенном ниже примере показано, как `query` использовать этот параметр для получения одного или нескольких подходящих подходящих корпоративных подходящих подходящих подходящих подходящих корпоративных сотрудников.</span><span class="sxs-lookup"><span data-stu-id="d02e3-146">The following example shows how to use the `query` parameter to get one or more matching Bookings businesses in the tenant.</span></span>
<!-- {
  "blockType": "request",
  "name": "query_bookingbusinesses"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses?query=Adventure
```
##### <a name="response-2"></a><span data-ttu-id="d02e3-147">Ответ 2</span><span class="sxs-lookup"><span data-stu-id="d02e3-147">Response 2</span></span>
<span data-ttu-id="d02e3-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d02e3-148">The following is an example of the response.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d02e3-149">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="d02e3-149">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d02e3-150">C#</span><span class="sxs-lookup"><span data-stu-id="d02e3-150">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/query_bookingbusinesses-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d02e3-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="d02e3-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/query_bookingbusinesses-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d02e3-152">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d02e3-152">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/query_bookingbusinesses-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/bookingbusiness-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/bookingbusiness-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingbusiness-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/bookingbusiness-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingbusiness-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
