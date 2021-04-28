---
title: 'Range: EntireColumn'
description: Возвращает объект, представляющий весь столбец диапазона.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: c9ee39c01e85b2525f4dc798c8c775b217733c53
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053043"
---
# <a name="range-entirecolumn"></a><span data-ttu-id="34d01-103">Range: EntireColumn</span><span class="sxs-lookup"><span data-stu-id="34d01-103">Range: EntireColumn</span></span>

<span data-ttu-id="34d01-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34d01-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="34d01-105">Возвращает объект, представляющий весь столбец диапазона.</span><span class="sxs-lookup"><span data-stu-id="34d01-105">Gets an object that represents the entire column of the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="34d01-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="34d01-106">Permissions</span></span>
<span data-ttu-id="34d01-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34d01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34d01-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="34d01-109">Permission type</span></span>      | <span data-ttu-id="34d01-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="34d01-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="34d01-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="34d01-111">Delegated (work or school account)</span></span> | <span data-ttu-id="34d01-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34d01-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="34d01-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="34d01-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34d01-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34d01-114">Not supported.</span></span>    |
|<span data-ttu-id="34d01-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="34d01-115">Application</span></span> | <span data-ttu-id="34d01-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34d01-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="34d01-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="34d01-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/names/{name}/range/entireColumn
GET /me/drive/root:/{item-path}:/workbook/names/{name}/range/entireColumn
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/entireColumn
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/entireColumn
GET /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/entireColumn
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/entireColumn

```
## <a name="request-headers"></a><span data-ttu-id="34d01-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="34d01-118">Request headers</span></span>
| <span data-ttu-id="34d01-119">Имя</span><span class="sxs-lookup"><span data-stu-id="34d01-119">Name</span></span>       | <span data-ttu-id="34d01-120">Описание</span><span class="sxs-lookup"><span data-stu-id="34d01-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="34d01-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="34d01-121">Authorization</span></span>  | <span data-ttu-id="34d01-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="34d01-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="34d01-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="34d01-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="34d01-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="34d01-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="34d01-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="34d01-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="34d01-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="34d01-128">Response</span></span>

<span data-ttu-id="34d01-129">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="34d01-129">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34d01-130">Пример</span><span class="sxs-lookup"><span data-stu-id="34d01-130">Example</span></span>
<span data-ttu-id="34d01-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="34d01-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="34d01-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="34d01-132">Request</span></span>
<span data-ttu-id="34d01-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="34d01-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="34d01-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="34d01-134">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_entirecolumn"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/entireColumn
```
# <a name="c"></a>[<span data-ttu-id="34d01-135">C#</span><span class="sxs-lookup"><span data-stu-id="34d01-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-entirecolumn-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="34d01-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="34d01-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-entirecolumn-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="34d01-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="34d01-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-entirecolumn-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="34d01-138">Java</span><span class="sxs-lookup"><span data-stu-id="34d01-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-entirecolumn-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="34d01-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="34d01-139">Response</span></span>
<span data-ttu-id="34d01-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="34d01-140">Here is an example of the response.</span></span> <span data-ttu-id="34d01-141">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="34d01-141">Note: The response object shown here might be shortened for readability.</span></span>
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
  "description": "Range: EntireColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

