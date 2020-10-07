---
title: Список строк
description: Получение списка объектов tableRow.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: aa3087e98ca50d440c19f1a329b6fa6c57a05156
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/07/2020
ms.locfileid: "48372703"
---
# <a name="list-rows"></a><span data-ttu-id="96471-103">Перечисление строк</span><span class="sxs-lookup"><span data-stu-id="96471-103">List rows</span></span>

<span data-ttu-id="96471-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96471-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96471-105">Получение списка объектов tablerow.</span><span class="sxs-lookup"><span data-stu-id="96471-105">Retrieve a list of tablerow objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="96471-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="96471-106">Permissions</span></span>
<span data-ttu-id="96471-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96471-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96471-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="96471-109">Permission type</span></span>      | <span data-ttu-id="96471-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="96471-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96471-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="96471-111">Delegated (work or school account)</span></span> | <span data-ttu-id="96471-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96471-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="96471-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="96471-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96471-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96471-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="96471-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="96471-115">Application</span></span> | <span data-ttu-id="96471-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96471-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="96471-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="96471-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/rows
GET /workbook/worksheets/{id|name}/tables/{id|name}/rows
```
## <a name="optional-query-parameters"></a><span data-ttu-id="96471-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="96471-118">Optional query parameters</span></span>
<span data-ttu-id="96471-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="96471-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span> <span data-ttu-id="96471-120">Для получения надежных результатов применяйте параметры запросов [$top](/graph/query-parameters#top) и [$skip](/graph/query-parameters#skip-parameter) на странице.</span><span class="sxs-lookup"><span data-stu-id="96471-120">For reliable results, use the [$top](/graph/query-parameters#top) and [$skip](/graph/query-parameters#skip-parameter) query parameters to page through the results.</span></span> <span data-ttu-id="96471-121">Это поможет избежать проблем с производительностью, связанных с большими результирующими наборами.</span><span class="sxs-lookup"><span data-stu-id="96471-121">This will help avoid performance problems related to large result sets.</span></span>

## <a name="request-headers"></a><span data-ttu-id="96471-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="96471-122">Request headers</span></span>
| <span data-ttu-id="96471-123">Имя</span><span class="sxs-lookup"><span data-stu-id="96471-123">Name</span></span>      |<span data-ttu-id="96471-124">Описание</span><span class="sxs-lookup"><span data-stu-id="96471-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="96471-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="96471-125">Authorization</span></span>  | <span data-ttu-id="96471-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="96471-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="96471-128">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="96471-128">Workbook-Session-Id</span></span>  | <span data-ttu-id="96471-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="96471-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="96471-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="96471-131">Request body</span></span>
<span data-ttu-id="96471-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="96471-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96471-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="96471-133">Response</span></span>

<span data-ttu-id="96471-134">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [воркбуктаблеров](../resources/workbooktablerow.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="96471-134">If successful, this method returns a `200 OK` response code and collection of [workbookTableRow](../resources/workbooktablerow.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="96471-135">Пример</span><span class="sxs-lookup"><span data-stu-id="96471-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="96471-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="96471-136">Request</span></span>
<span data-ttu-id="96471-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="96471-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="96471-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="96471-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_table_rows"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5&$skip=5
```
# <a name="c"></a>[<span data-ttu-id="96471-139">C#</span><span class="sxs-lookup"><span data-stu-id="96471-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-table-rows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="96471-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96471-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-table-rows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="96471-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="96471-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-table-rows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="96471-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="96471-142">Response</span></span>
<span data-ttu-id="96471-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="96471-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

> <span data-ttu-id="96471-146">**Примечание:** Используйте параметры запроса [$Top](/graph/query-parameters#top) и [$Skip](/graph/query-parameters#skip-parameter) для постраничного выполнения большого количества строк.</span><span class="sxs-lookup"><span data-stu-id="96471-146">**Note:** Use the [$top](/graph/query-parameters#top) and [$skip](/graph/query-parameters#skip-parameter) query parameters to page through large numbers of rows.</span></span>

<span data-ttu-id="96471-147">Пример:</span><span class="sxs-lookup"><span data-stu-id="96471-147">Example:</span></span> 

`https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5`
`https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5&$skip=5`

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List rows",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
