---
title: Список столбцов
description: Получение списка объектов tablecolumn.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: eafbbdef90484d9fabba731ec6a7a4c0055b8a6c
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2021
ms.locfileid: "50034207"
---
# <a name="list-columns"></a><span data-ttu-id="4eae4-103">Перечисление столбцов</span><span class="sxs-lookup"><span data-stu-id="4eae4-103">List columns</span></span>

<span data-ttu-id="4eae4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4eae4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4eae4-105">Получение списка объектов tablecolumn.</span><span class="sxs-lookup"><span data-stu-id="4eae4-105">Retrieve a list of tablecolumn objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="4eae4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4eae4-106">Permissions</span></span>
<span data-ttu-id="4eae4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4eae4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4eae4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4eae4-109">Permission type</span></span>      | <span data-ttu-id="4eae4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4eae4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4eae4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4eae4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4eae4-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4eae4-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4eae4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4eae4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4eae4-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4eae4-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4eae4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4eae4-115">Application</span></span> | <span data-ttu-id="4eae4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4eae4-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4eae4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4eae4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/columns
GET /workbook/worksheets/{id|name}/tables/{id|name}/columns
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4eae4-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4eae4-118">Optional query parameters</span></span>
<span data-ttu-id="4eae4-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4eae4-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span> <span data-ttu-id="4eae4-120">Для получения надежных результатов применяйте параметры запросов [$top](/graph/query-parameters#top) и [$skip](/graph/query-parameters#skip-parameter) на странице.</span><span class="sxs-lookup"><span data-stu-id="4eae4-120">For reliable results, use the [$top](/graph/query-parameters#top) and [$skip](/graph/query-parameters#skip-parameter) query parameters to page through the results.</span></span> <span data-ttu-id="4eae4-121">Это поможет избежать проблем с производительностью, связанных с большими результирующими наборами.</span><span class="sxs-lookup"><span data-stu-id="4eae4-121">This will help avoid performance problems related to large result sets.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4eae4-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4eae4-122">Request headers</span></span>
| <span data-ttu-id="4eae4-123">Имя</span><span class="sxs-lookup"><span data-stu-id="4eae4-123">Name</span></span>      |<span data-ttu-id="4eae4-124">Описание</span><span class="sxs-lookup"><span data-stu-id="4eae4-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4eae4-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4eae4-125">Authorization</span></span>  | <span data-ttu-id="4eae4-p103">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4eae4-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4eae4-128">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4eae4-128">Workbook-Session-Id</span></span>  | <span data-ttu-id="4eae4-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="4eae4-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4eae4-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4eae4-131">Request body</span></span>
<span data-ttu-id="4eae4-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4eae4-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4eae4-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="4eae4-133">Response</span></span>

<span data-ttu-id="4eae4-134">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [workbookTableColumn](../resources/workbooktablecolumn.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4eae4-134">If successful, this method returns a `200 OK` response code and collection of [workbookTableColumn](../resources/workbooktablecolumn.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4eae4-135">Пример</span><span class="sxs-lookup"><span data-stu-id="4eae4-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4eae4-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="4eae4-136">Request</span></span>
<span data-ttu-id="4eae4-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4eae4-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4eae4-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="4eae4-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_columns"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns?$top=5&$skip=5
```
# <a name="c"></a>[<span data-ttu-id="4eae4-139">C#</span><span class="sxs-lookup"><span data-stu-id="4eae4-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-columns-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4eae4-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4eae4-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-columns-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4eae4-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4eae4-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-columns-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4eae4-142">Java</span><span class="sxs-lookup"><span data-stu-id="4eae4-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-columns-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4eae4-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="4eae4-143">Response</span></span>
<span data-ttu-id="4eae4-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4eae4-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "id": "99",
      "name": "name-value",
      "index": 99,
      "values": "values-value"
    }
  ]
}
```

> <span data-ttu-id="4eae4-147">
  \*\*Примечание.\*\* Используйте параметры запросов [$top](/graph/query-parameters#top) и [$skip](/graph/query-parameters#skip-parameter), чтобы просматривать постранично большое количество столбцов.</span><span class="sxs-lookup"><span data-stu-id="4eae4-147">**Note:** Use the [$top](/graph/query-parameters#top) and [$skip](/graph/query-parameters#skip-parameter) query parameters to page through large numbers of columns.</span></span>

<span data-ttu-id="4eae4-148">Пример:</span><span class="sxs-lookup"><span data-stu-id="4eae4-148">Example:</span></span> 

`https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns?$top=5`
`https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns?$top=5&$skip=5`

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List columns",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
