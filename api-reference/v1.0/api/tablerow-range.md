---
title: 'TableRow: Range'
description: Возвращает объект диапазона, связанный со всей строкой.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 218233d61ceb79e950fdb3c796ce16afad85e582
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50575093"
---
# <a name="tablerow-range"></a><span data-ttu-id="a6899-103">TableRow: Range</span><span class="sxs-lookup"><span data-stu-id="a6899-103">TableRow: Range</span></span>

<span data-ttu-id="a6899-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6899-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a6899-105">Возвращает объект диапазона, связанный со всей строкой.</span><span class="sxs-lookup"><span data-stu-id="a6899-105">Returns the range object associated with the entire row.</span></span>
## <a name="permissions"></a><span data-ttu-id="a6899-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a6899-106">Permissions</span></span>
<span data-ttu-id="a6899-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6899-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6899-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a6899-109">Permission type</span></span>      | <span data-ttu-id="a6899-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a6899-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6899-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a6899-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a6899-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a6899-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a6899-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a6899-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6899-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6899-114">Not supported.</span></span>    |
|<span data-ttu-id="a6899-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a6899-115">Application</span></span> | <span data-ttu-id="a6899-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6899-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6899-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a6899-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}/range
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/rows/{index}/range
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/rows/{index}/range
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/rows/{index}/range

```
## <a name="request-headers"></a><span data-ttu-id="a6899-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a6899-118">Request headers</span></span>
| <span data-ttu-id="a6899-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a6899-119">Name</span></span>       | <span data-ttu-id="a6899-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a6899-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a6899-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a6899-121">Authorization</span></span>  | <span data-ttu-id="a6899-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a6899-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a6899-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a6899-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="a6899-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="a6899-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6899-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a6899-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="a6899-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6899-128">Response</span></span>

<span data-ttu-id="a6899-129">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a6899-129">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6899-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a6899-130">Example</span></span>
<span data-ttu-id="a6899-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="a6899-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a6899-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a6899-132">Request</span></span>
<span data-ttu-id="a6899-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a6899-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a6899-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="a6899-134">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "tablerow_range"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}/range
```
# <a name="c"></a>[<span data-ttu-id="a6899-135">C#</span><span class="sxs-lookup"><span data-stu-id="a6899-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablerow-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a6899-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a6899-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablerow-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a6899-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a6899-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablerow-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a6899-138">Java</span><span class="sxs-lookup"><span data-stu-id="a6899-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablerow-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a6899-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6899-139">Response</span></span>
<span data-ttu-id="a6899-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a6899-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "TableRow: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

