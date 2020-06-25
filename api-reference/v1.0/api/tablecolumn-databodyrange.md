---
title: 'TableColumn: DataBodyRange'
description: Получает объект диапазона, связанный с данными столбца.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: cb9ee795c7291def2c5e8120fae0d0a7496ed455
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863983"
---
# <a name="tablecolumn-databodyrange"></a><span data-ttu-id="4becd-103">TableColumn: DataBodyRange</span><span class="sxs-lookup"><span data-stu-id="4becd-103">TableColumn: DataBodyRange</span></span>

<span data-ttu-id="4becd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4becd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4becd-105">Получает объект диапазона, связанный с данными столбца.</span><span class="sxs-lookup"><span data-stu-id="4becd-105">Gets the range object associated with the data body of the column.</span></span>
## <a name="permissions"></a><span data-ttu-id="4becd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4becd-106">Permissions</span></span>
<span data-ttu-id="4becd-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="4becd-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="4becd-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4becd-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4becd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4becd-109">Permission type</span></span>      | <span data-ttu-id="4becd-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4becd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4becd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4becd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4becd-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4becd-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4becd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4becd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4becd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4becd-114">Not supported.</span></span>    |
|<span data-ttu-id="4becd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4becd-115">Application</span></span> | <span data-ttu-id="4becd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4becd-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4becd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4becd-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/columns/{id|name}/dataBodyRange
GET /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/dataBodyRange

```
## <a name="request-headers"></a><span data-ttu-id="4becd-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4becd-118">Request headers</span></span>
| <span data-ttu-id="4becd-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4becd-119">Name</span></span>       | <span data-ttu-id="4becd-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4becd-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4becd-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4becd-121">Authorization</span></span>  | <span data-ttu-id="4becd-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="4becd-122">Bearer {token}.</span></span> <span data-ttu-id="4becd-123">Required.</span><span class="sxs-lookup"><span data-stu-id="4becd-123">Required.</span></span> |
| <span data-ttu-id="4becd-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4becd-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="4becd-125">Workbook session Id that determines if changes are persisted or not.</span><span class="sxs-lookup"><span data-stu-id="4becd-125">Workbook session Id that determines if changes are persisted or not.</span></span> <span data-ttu-id="4becd-126">Optional.</span><span class="sxs-lookup"><span data-stu-id="4becd-126">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4becd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4becd-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="4becd-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="4becd-128">Response</span></span>

<span data-ttu-id="4becd-129">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4becd-129">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4becd-130">Пример</span><span class="sxs-lookup"><span data-stu-id="4becd-130">Example</span></span>
<span data-ttu-id="4becd-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="4becd-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4becd-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4becd-132">Request</span></span>
<span data-ttu-id="4becd-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4becd-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4becd-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="4becd-134">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "tablecolumn_databodyrange",
  "idempotent": true
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/dataBodyRange
```
# <a name="c"></a>[<span data-ttu-id="4becd-135">C#</span><span class="sxs-lookup"><span data-stu-id="4becd-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablecolumn-databodyrange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4becd-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4becd-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablecolumn-databodyrange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4becd-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4becd-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablecolumn-databodyrange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4becd-138">Java</span><span class="sxs-lookup"><span data-stu-id="4becd-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablecolumn-databodyrange-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4becd-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="4becd-139">Response</span></span>
<span data-ttu-id="4becd-140">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="4becd-140">Here is an example of the response.</span></span> <span data-ttu-id="4becd-141">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="4becd-141">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="4becd-142">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="4becd-142">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableColumn: DataBodyRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
