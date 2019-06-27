---
title: Список столбцов
description: Получение списка объектов tablecolumn.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: bd1da20b9b67168f4d1d93950927b9f11cf82635
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35279130"
---
# <a name="list-columns"></a><span data-ttu-id="ff891-103">Список столбцов</span><span class="sxs-lookup"><span data-stu-id="ff891-103">List columns</span></span>

<span data-ttu-id="ff891-104">Получение списка объектов tablecolumn.</span><span class="sxs-lookup"><span data-stu-id="ff891-104">Retrieve a list of tablecolumn objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="ff891-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ff891-105">Permissions</span></span>
<span data-ttu-id="ff891-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff891-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff891-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ff891-108">Permission type</span></span>      | <span data-ttu-id="ff891-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ff891-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ff891-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ff891-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ff891-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ff891-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ff891-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ff891-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff891-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff891-113">Not supported.</span></span>    |
|<span data-ttu-id="ff891-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ff891-114">Application</span></span> | <span data-ttu-id="ff891-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff891-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff891-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ff891-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/columns
GET /workbook/worksheets/{id|name}/tables/{id|name}/columns
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ff891-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ff891-117">Optional query parameters</span></span>
<span data-ttu-id="ff891-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ff891-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>  <span data-ttu-id="ff891-119">Для получения надежных результатов применяйте параметры запросов [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) и [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) на странице.</span><span class="sxs-lookup"><span data-stu-id="ff891-119">For reliable results, use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through the results.</span></span> <span data-ttu-id="ff891-120">Это поможет избежать проблем с производительностью, связанных с большими результирующими наборами.</span><span class="sxs-lookup"><span data-stu-id="ff891-120">This will help avoid performance problems related to large result sets.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ff891-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ff891-121">Request headers</span></span>
| <span data-ttu-id="ff891-122">Имя</span><span class="sxs-lookup"><span data-stu-id="ff891-122">Name</span></span>      |<span data-ttu-id="ff891-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ff891-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ff891-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ff891-124">Authorization</span></span>  | <span data-ttu-id="ff891-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ff891-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ff891-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ff891-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="ff891-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="ff891-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff891-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ff891-130">Request body</span></span>
<span data-ttu-id="ff891-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ff891-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff891-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="ff891-132">Response</span></span>

<span data-ttu-id="ff891-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [воркбуктаблеколумн](../resources/tablecolumn.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ff891-133">If successful, this method returns a `200 OK` response code and collection of [WorkbookTableColumn](../resources/tablecolumn.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ff891-134">Пример</span><span class="sxs-lookup"><span data-stu-id="ff891-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ff891-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="ff891-135">Request</span></span>
<span data-ttu-id="ff891-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ff891-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_columns"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns?$top=5&$skip=5
```
##### <a name="response"></a><span data-ttu-id="ff891-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff891-137">Response</span></span>
<span data-ttu-id="ff891-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ff891-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableColumn",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 126

{
  "value": [
    {
      "id": 99,
      "name": "name-value",
      "index": 99,
      "values": "values-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="ff891-141">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="ff891-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ff891-142">C#</span><span class="sxs-lookup"><span data-stu-id="ff891-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_columns-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ff891-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="ff891-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_columns-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="ff891-144">Цель — C</span><span class="sxs-lookup"><span data-stu-id="ff891-144">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_columns-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

> <span data-ttu-id="ff891-145">
  \*\*Примечание.\*\* Используйте параметры запросов [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) и [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter), чтобы просматривать постранично большое количество столбцов.</span><span class="sxs-lookup"><span data-stu-id="ff891-145">**Note:** Use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through large numbers of columns.</span></span>

<span data-ttu-id="ff891-146">Пример.</span><span class="sxs-lookup"><span data-stu-id="ff891-146">Example:</span></span> 

`https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns?$top=5`
`https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns?$top=5&$skip=5`

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List columns",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/table-list-columns.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/table-list-columns.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/table-list-columns.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
