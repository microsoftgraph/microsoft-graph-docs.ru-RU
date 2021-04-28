---
title: 'workbookTable: диапазон'
description: Получает объект диапазона, связанный со всей таблицей.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: e1b01a3a8df2288084803fb07ba5ccd489844a23
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054401"
---
# <a name="workbooktable-range"></a><span data-ttu-id="2ef97-103">workbookTable: диапазон</span><span class="sxs-lookup"><span data-stu-id="2ef97-103">workbookTable: range</span></span>

<span data-ttu-id="2ef97-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ef97-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2ef97-105">Получите объект диапазона, связанный со всей таблицей.</span><span class="sxs-lookup"><span data-stu-id="2ef97-105">Get the range object associated with the entire table.</span></span>
## <a name="permissions"></a><span data-ttu-id="2ef97-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2ef97-106">Permissions</span></span>
<span data-ttu-id="2ef97-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ef97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ef97-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2ef97-109">Permission type</span></span>      | <span data-ttu-id="2ef97-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2ef97-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ef97-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2ef97-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2ef97-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2ef97-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2ef97-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2ef97-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ef97-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ef97-114">Not supported.</span></span>    |
|<span data-ttu-id="2ef97-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2ef97-115">Application</span></span> | <span data-ttu-id="2ef97-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ef97-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ef97-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2ef97-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/tables/{id|name}/range
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/range
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/range
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/range

```
## <a name="request-headers"></a><span data-ttu-id="2ef97-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2ef97-118">Request headers</span></span>
| <span data-ttu-id="2ef97-119">Имя</span><span class="sxs-lookup"><span data-stu-id="2ef97-119">Name</span></span>       | <span data-ttu-id="2ef97-120">Описание</span><span class="sxs-lookup"><span data-stu-id="2ef97-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2ef97-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2ef97-121">Authorization</span></span>  | <span data-ttu-id="2ef97-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2ef97-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2ef97-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2ef97-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="2ef97-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="2ef97-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ef97-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2ef97-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="2ef97-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ef97-128">Response</span></span>

<span data-ttu-id="2ef97-129">В случае успешной работы этот метод возвращает код отклика и `200 OK` объект [workbookRange](../resources/range.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="2ef97-129">If successful, this method returns a `200 OK` response code and a [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ef97-130">Пример</span><span class="sxs-lookup"><span data-stu-id="2ef97-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ef97-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ef97-131">Request</span></span>
<span data-ttu-id="2ef97-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2ef97-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2ef97-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ef97-133">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "table_range",
  "idempotent": true
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/range
```
# <a name="c"></a>[<span data-ttu-id="2ef97-134">C#</span><span class="sxs-lookup"><span data-stu-id="2ef97-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/table-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2ef97-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ef97-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/table-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2ef97-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ef97-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/table-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2ef97-137">Java</span><span class="sxs-lookup"><span data-stu-id="2ef97-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/table-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2ef97-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ef97-138">Response</span></span>
<span data-ttu-id="2ef97-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2ef97-139">The following is an example of the response.</span></span> 

><span data-ttu-id="2ef97-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2ef97-140">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "description": "Table: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

