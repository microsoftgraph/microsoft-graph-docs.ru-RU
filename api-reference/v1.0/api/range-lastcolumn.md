---
title: 'Range: LastColumn'
description: .
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: bd1fe3b9a1eb2e839f0435b59f29639f00b0a781
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48051636"
---
# <a name="range-lastcolumn"></a><span data-ttu-id="f0159-103">Range: LastColumn</span><span class="sxs-lookup"><span data-stu-id="f0159-103">Range: LastColumn</span></span>

<span data-ttu-id="f0159-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0159-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f0159-p101">Возвращает последний столбец в диапазоне. Например, последний столбец диапазона B2:D5 — D2:D5.</span><span class="sxs-lookup"><span data-stu-id="f0159-p101">Gets the last column within the range. For example, the last column of "B2:D5" is "D2:D5".</span></span>
## <a name="permissions"></a><span data-ttu-id="f0159-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f0159-107">Permissions</span></span>
<span data-ttu-id="f0159-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0159-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0159-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f0159-110">Permission type</span></span>      | <span data-ttu-id="f0159-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f0159-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f0159-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f0159-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f0159-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f0159-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f0159-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f0159-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0159-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0159-115">Not supported.</span></span>    |
|<span data-ttu-id="f0159-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f0159-116">Application</span></span> | <span data-ttu-id="f0159-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0159-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f0159-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f0159-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/lastColumn
GET /workbook/worksheets/{id|name}/range(address='<address>')/lastColumn
GET /workbook/tables/{id|name}/columns/{id|name}/range/lastColumn

```
## <a name="request-headers"></a><span data-ttu-id="f0159-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f0159-119">Request headers</span></span>
| <span data-ttu-id="f0159-120">Имя</span><span class="sxs-lookup"><span data-stu-id="f0159-120">Name</span></span>       | <span data-ttu-id="f0159-121">Описание</span><span class="sxs-lookup"><span data-stu-id="f0159-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f0159-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f0159-122">Authorization</span></span>  | <span data-ttu-id="f0159-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f0159-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f0159-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f0159-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="f0159-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="f0159-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0159-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f0159-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="f0159-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0159-129">Response</span></span>

<span data-ttu-id="f0159-130">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f0159-130">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0159-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f0159-131">Example</span></span>
<span data-ttu-id="f0159-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="f0159-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f0159-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="f0159-133">Request</span></span>
<span data-ttu-id="f0159-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f0159-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f0159-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="f0159-135">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_lastcolumn"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/lastColumn
```
# <a name="c"></a>[<span data-ttu-id="f0159-136">C#</span><span class="sxs-lookup"><span data-stu-id="f0159-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-lastcolumn-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f0159-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f0159-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-lastcolumn-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f0159-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f0159-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-lastcolumn-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f0159-139">Java</span><span class="sxs-lookup"><span data-stu-id="f0159-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-lastcolumn-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f0159-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0159-140">Response</span></span>
<span data-ttu-id="f0159-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f0159-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: LastColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

