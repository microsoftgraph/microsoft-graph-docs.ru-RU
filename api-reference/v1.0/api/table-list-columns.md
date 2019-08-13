---
title: Список столбцов
description: Получение списка объектов tablecolumn.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 02e741a37afb9fd39ed4507eb33dc9a92293c01a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36341738"
---
# <a name="list-columns"></a><span data-ttu-id="90d7a-103">Список столбцов</span><span class="sxs-lookup"><span data-stu-id="90d7a-103">List columns</span></span>

<span data-ttu-id="90d7a-104">Получение списка объектов tablecolumn.</span><span class="sxs-lookup"><span data-stu-id="90d7a-104">Retrieve a list of tablecolumn objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="90d7a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="90d7a-105">Permissions</span></span>
<span data-ttu-id="90d7a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90d7a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90d7a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="90d7a-108">Permission type</span></span>      | <span data-ttu-id="90d7a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="90d7a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="90d7a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="90d7a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="90d7a-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="90d7a-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="90d7a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="90d7a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90d7a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90d7a-113">Not supported.</span></span>    |
|<span data-ttu-id="90d7a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="90d7a-114">Application</span></span> | <span data-ttu-id="90d7a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90d7a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="90d7a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="90d7a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/columns
GET /workbook/worksheets/{id|name}/tables/{id|name}/columns
```
## <a name="optional-query-parameters"></a><span data-ttu-id="90d7a-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="90d7a-117">Optional query parameters</span></span>
<span data-ttu-id="90d7a-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="90d7a-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>  <span data-ttu-id="90d7a-119">Для получения надежных результатов применяйте параметры запросов [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) и [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) на странице.</span><span class="sxs-lookup"><span data-stu-id="90d7a-119">For reliable results, use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through the results.</span></span> <span data-ttu-id="90d7a-120">Это поможет избежать проблем с производительностью, связанных с большими результирующими наборами.</span><span class="sxs-lookup"><span data-stu-id="90d7a-120">This will help avoid performance problems related to large result sets.</span></span>

## <a name="request-headers"></a><span data-ttu-id="90d7a-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="90d7a-121">Request headers</span></span>
| <span data-ttu-id="90d7a-122">Имя</span><span class="sxs-lookup"><span data-stu-id="90d7a-122">Name</span></span>      |<span data-ttu-id="90d7a-123">Описание</span><span class="sxs-lookup"><span data-stu-id="90d7a-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="90d7a-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="90d7a-124">Authorization</span></span>  | <span data-ttu-id="90d7a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="90d7a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="90d7a-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="90d7a-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="90d7a-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="90d7a-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="90d7a-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="90d7a-130">Request body</span></span>
<span data-ttu-id="90d7a-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="90d7a-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90d7a-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="90d7a-132">Response</span></span>

<span data-ttu-id="90d7a-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [воркбуктаблеколумн](../resources/tablecolumn.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="90d7a-133">If successful, this method returns a `200 OK` response code and collection of [WorkbookTableColumn](../resources/tablecolumn.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="90d7a-134">Пример</span><span class="sxs-lookup"><span data-stu-id="90d7a-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="90d7a-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="90d7a-135">Request</span></span>
<span data-ttu-id="90d7a-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="90d7a-136">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="90d7a-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="90d7a-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_columns"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns?$top=5&$skip=5
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="90d7a-138">C#</span><span class="sxs-lookup"><span data-stu-id="90d7a-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-columns-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="90d7a-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="90d7a-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-columns-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="90d7a-140">Цель — C</span><span class="sxs-lookup"><span data-stu-id="90d7a-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-columns-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="90d7a-141">Java</span><span class="sxs-lookup"><span data-stu-id="90d7a-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-columns-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="90d7a-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="90d7a-142">Response</span></span>
<span data-ttu-id="90d7a-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="90d7a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

> <span data-ttu-id="90d7a-146">
  \*\*Примечание.\*\* Используйте параметры запросов [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) и [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter), чтобы просматривать постранично большое количество столбцов.</span><span class="sxs-lookup"><span data-stu-id="90d7a-146">**Note:** Use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through large numbers of columns.</span></span>

<span data-ttu-id="90d7a-147">Пример.</span><span class="sxs-lookup"><span data-stu-id="90d7a-147">Example:</span></span> 

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
  ]
}-->
