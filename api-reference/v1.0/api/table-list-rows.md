---
title: Список строк
description: Получение списка объектов tableRow.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: abc5e482013adfa30ad92404ad318c1006dc0e2e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52034485"
---
# <a name="list-rows"></a><span data-ttu-id="9278a-103">Перечисление строк</span><span class="sxs-lookup"><span data-stu-id="9278a-103">List rows</span></span>

<span data-ttu-id="9278a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9278a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9278a-105">Получение списка объектов tablerow.</span><span class="sxs-lookup"><span data-stu-id="9278a-105">Retrieve a list of tablerow objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="9278a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9278a-106">Permissions</span></span>
<span data-ttu-id="9278a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9278a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9278a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9278a-109">Permission type</span></span>      | <span data-ttu-id="9278a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9278a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9278a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9278a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9278a-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9278a-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9278a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9278a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9278a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9278a-114">Not supported.</span></span>    |
|<span data-ttu-id="9278a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9278a-115">Application</span></span> | <span data-ttu-id="9278a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9278a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9278a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9278a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/tables/{id|name}/rows
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/rows
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/rows
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/rows
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9278a-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9278a-118">Optional query parameters</span></span>
<span data-ttu-id="9278a-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9278a-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>  <span data-ttu-id="9278a-120">Для получения надежных результатов применяйте параметры запросов [$top](/graph/query-parameters#top) и [$skip](/graph/query-parameters#skip-parameter) на странице.</span><span class="sxs-lookup"><span data-stu-id="9278a-120">For reliable results, use the [$top](/graph/query-parameters#top) and [$skip](/graph/query-parameters#skip-parameter) query parameters to page through the results.</span></span> <span data-ttu-id="9278a-121">Это поможет избежать проблем с производительностью, связанных с большими результирующими наборами.</span><span class="sxs-lookup"><span data-stu-id="9278a-121">This will help avoid performance problems related to large result sets.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9278a-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9278a-122">Request headers</span></span>
| <span data-ttu-id="9278a-123">Имя</span><span class="sxs-lookup"><span data-stu-id="9278a-123">Name</span></span>      |<span data-ttu-id="9278a-124">Описание</span><span class="sxs-lookup"><span data-stu-id="9278a-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9278a-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9278a-125">Authorization</span></span>  | <span data-ttu-id="9278a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9278a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9278a-128">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9278a-128">Workbook-Session-Id</span></span>  | <span data-ttu-id="9278a-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="9278a-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9278a-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9278a-131">Request body</span></span>
<span data-ttu-id="9278a-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9278a-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9278a-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="9278a-133">Response</span></span>

<span data-ttu-id="9278a-134">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [WorkbookTableRow](../resources/tablerow.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9278a-134">If successful, this method returns a `200 OK` response code and collection of [WorkbookTableRow](../resources/tablerow.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9278a-135">Пример</span><span class="sxs-lookup"><span data-stu-id="9278a-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9278a-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="9278a-136">Request</span></span>
<span data-ttu-id="9278a-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9278a-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9278a-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="9278a-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_table_rows"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5&$skip=5
```
# <a name="c"></a>[<span data-ttu-id="9278a-139">C#</span><span class="sxs-lookup"><span data-stu-id="9278a-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-table-rows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9278a-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9278a-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-table-rows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9278a-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9278a-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-table-rows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9278a-142">Java</span><span class="sxs-lookup"><span data-stu-id="9278a-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-table-rows-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9278a-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="9278a-143">Response</span></span>
<span data-ttu-id="9278a-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9278a-144">Here is an example of the response.</span></span> <span data-ttu-id="9278a-145">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9278a-145">Note: The response object shown here might be shortened for readability.</span></span>
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
> <span data-ttu-id="9278a-146">**Примечание:** Используйте [параметры $top](/graph/query-parameters#top) [и $skip](/graph/query-parameters#skip-parameter) запроса для страницы через большое количество строк.</span><span class="sxs-lookup"><span data-stu-id="9278a-146">**Note:** Use the [$top](/graph/query-parameters#top) and [$skip](/graph/query-parameters#skip-parameter) query parameters to page through large numbers of rows.</span></span>

<span data-ttu-id="9278a-147">Пример:</span><span class="sxs-lookup"><span data-stu-id="9278a-147">Example:</span></span> 

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
