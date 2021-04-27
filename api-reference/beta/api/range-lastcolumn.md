---
title: 'Range: LastColumn'
description: .
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 7c0c9605ea3af342b114fb56e7d605fb82d04799
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055087"
---
# <a name="range-lastcolumn"></a><span data-ttu-id="7555f-103">Range: LastColumn</span><span class="sxs-lookup"><span data-stu-id="7555f-103">Range: LastColumn</span></span>

<span data-ttu-id="7555f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7555f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7555f-p101">Возвращает последний столбец в диапазоне. Например, последний столбец диапазона B2:D5 — D2:D5.</span><span class="sxs-lookup"><span data-stu-id="7555f-p101">Gets the last column within the range. For example, the last column of "B2:D5" is "D2:D5".</span></span>
## <a name="permissions"></a><span data-ttu-id="7555f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7555f-107">Permissions</span></span>
<span data-ttu-id="7555f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7555f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7555f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7555f-110">Permission type</span></span>      | <span data-ttu-id="7555f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7555f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7555f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7555f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7555f-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7555f-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7555f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7555f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7555f-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7555f-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7555f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7555f-116">Application</span></span> | <span data-ttu-id="7555f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7555f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7555f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7555f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/names/{name}/range/LastColumn
GET /me/drive/root:/{item-path}:/workbook/names/{name}/range/LastColumn
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/LastColumn
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/LastColumn
GET /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/LastColumn
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/LastColumn

```
## <a name="request-headers"></a><span data-ttu-id="7555f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7555f-119">Request headers</span></span>
| <span data-ttu-id="7555f-120">Имя</span><span class="sxs-lookup"><span data-stu-id="7555f-120">Name</span></span>       | <span data-ttu-id="7555f-121">Описание</span><span class="sxs-lookup"><span data-stu-id="7555f-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7555f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7555f-122">Authorization</span></span>  | <span data-ttu-id="7555f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7555f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7555f-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7555f-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="7555f-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="7555f-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7555f-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7555f-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="7555f-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="7555f-129">Response</span></span>

<span data-ttu-id="7555f-130">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/workbookrange.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7555f-130">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7555f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="7555f-131">Example</span></span>
<span data-ttu-id="7555f-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="7555f-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7555f-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="7555f-133">Request</span></span>
<span data-ttu-id="7555f-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7555f-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7555f-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="7555f-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "range_lastcolumn"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/LastColumn
```
# <a name="c"></a>[<span data-ttu-id="7555f-136">C#</span><span class="sxs-lookup"><span data-stu-id="7555f-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-lastcolumn-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7555f-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7555f-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-lastcolumn-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7555f-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7555f-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-lastcolumn-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7555f-139">Java</span><span class="sxs-lookup"><span data-stu-id="7555f-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-lastcolumn-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7555f-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="7555f-140">Response</span></span>
<span data-ttu-id="7555f-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7555f-141">Here is an example of the response.</span></span> <span data-ttu-id="7555f-142">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7555f-142">Note: The response object shown here might be shortened for readability.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Range: LastColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


