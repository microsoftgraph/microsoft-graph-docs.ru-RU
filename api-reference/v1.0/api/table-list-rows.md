---
title: Список строк
description: Получение списка объектов tableRow.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 3aaa30559b3213a2879aa02ad2aaa8bb79dbee09
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36727707"
---
# <a name="list-rows"></a><span data-ttu-id="f77d2-103">Список строк</span><span class="sxs-lookup"><span data-stu-id="f77d2-103">List rows</span></span>

<span data-ttu-id="f77d2-104">Получение списка объектов tablerow.</span><span class="sxs-lookup"><span data-stu-id="f77d2-104">Retrieve a list of tablerow objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="f77d2-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f77d2-105">Permissions</span></span>
<span data-ttu-id="f77d2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f77d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f77d2-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f77d2-108">Permission type</span></span>      | <span data-ttu-id="f77d2-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f77d2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f77d2-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f77d2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f77d2-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f77d2-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f77d2-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f77d2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f77d2-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f77d2-113">Not supported.</span></span>    |
|<span data-ttu-id="f77d2-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f77d2-114">Application</span></span> | <span data-ttu-id="f77d2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f77d2-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f77d2-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f77d2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/rows
GET /workbook/worksheets/{id|name}/tables/{id|name}/rows
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f77d2-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f77d2-117">Optional query parameters</span></span>
<span data-ttu-id="f77d2-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f77d2-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>  <span data-ttu-id="f77d2-119">Для получения надежных результатов применяйте параметры запросов [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) и [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) на странице.</span><span class="sxs-lookup"><span data-stu-id="f77d2-119">For reliable results, use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through the results.</span></span> <span data-ttu-id="f77d2-120">Это поможет избежать проблем с производительностью, связанных с большими результирующими наборами.</span><span class="sxs-lookup"><span data-stu-id="f77d2-120">This will help avoid performance problems related to large result sets.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f77d2-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f77d2-121">Request headers</span></span>
| <span data-ttu-id="f77d2-122">Имя</span><span class="sxs-lookup"><span data-stu-id="f77d2-122">Name</span></span>      |<span data-ttu-id="f77d2-123">Описание</span><span class="sxs-lookup"><span data-stu-id="f77d2-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f77d2-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f77d2-124">Authorization</span></span>  | <span data-ttu-id="f77d2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f77d2-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f77d2-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f77d2-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="f77d2-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="f77d2-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f77d2-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f77d2-130">Request body</span></span>
<span data-ttu-id="f77d2-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f77d2-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f77d2-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="f77d2-132">Response</span></span>

<span data-ttu-id="f77d2-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [воркбуктаблеров](../resources/tablerow.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f77d2-133">If successful, this method returns a `200 OK` response code and collection of [WorkbookTableRow](../resources/tablerow.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f77d2-134">Пример</span><span class="sxs-lookup"><span data-stu-id="f77d2-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f77d2-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="f77d2-135">Request</span></span>
<span data-ttu-id="f77d2-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f77d2-136">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f77d2-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="f77d2-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_table_rows"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5&$skip=5
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f77d2-138">C#</span><span class="sxs-lookup"><span data-stu-id="f77d2-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-table-rows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f77d2-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f77d2-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-table-rows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f77d2-140">Цель — C</span><span class="sxs-lookup"><span data-stu-id="f77d2-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-table-rows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f77d2-141">Java</span><span class="sxs-lookup"><span data-stu-id="f77d2-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-table-rows-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f77d2-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="f77d2-142">Response</span></span>
<span data-ttu-id="f77d2-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f77d2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableRow",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 82

{
  "value": [
    {
      "index": 99,
      "values": "values-value"
    }
  ]
}
```
> <span data-ttu-id="f77d2-146">**Примечание:** Используйте параметры запроса [$Top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) и [$Skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) для постраничного выполнения большого количества строк.</span><span class="sxs-lookup"><span data-stu-id="f77d2-146">**Note:** Use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through large numbers of rows.</span></span>

<span data-ttu-id="f77d2-147">Пример.</span><span class="sxs-lookup"><span data-stu-id="f77d2-147">Example:</span></span> 

`https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5`
`https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5&$skip=5`


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List rows",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
