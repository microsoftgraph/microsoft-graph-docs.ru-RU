---
title: 'Range: EntireRow'
description: Возвращает объект, представляющий всю строку диапазона.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: f09acc2238cc7d814e3047e17a0604978f54af96
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048675"
---
# <a name="range-entirerow"></a><span data-ttu-id="ee34d-103">Range: EntireRow</span><span class="sxs-lookup"><span data-stu-id="ee34d-103">Range: EntireRow</span></span>

<span data-ttu-id="ee34d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee34d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ee34d-105">Возвращает объект, представляющий всю строку диапазона.</span><span class="sxs-lookup"><span data-stu-id="ee34d-105">Gets an object that represents the entire row of the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="ee34d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ee34d-106">Permissions</span></span>
<span data-ttu-id="ee34d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee34d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee34d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee34d-109">Permission type</span></span>      | <span data-ttu-id="ee34d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee34d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee34d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee34d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ee34d-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ee34d-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ee34d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee34d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee34d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee34d-114">Not supported.</span></span>    |
|<span data-ttu-id="ee34d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ee34d-115">Application</span></span> | <span data-ttu-id="ee34d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee34d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee34d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee34d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/names/{name}/range/entireRow
GET /me/drive/root:/{item-path}:/workbook/names/{name}/range/entireRow
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>'/entireRow
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>'/entireRow
GET /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/entireRow
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/entireRow

```
## <a name="request-headers"></a><span data-ttu-id="ee34d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ee34d-118">Request headers</span></span>
| <span data-ttu-id="ee34d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ee34d-119">Name</span></span>       | <span data-ttu-id="ee34d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ee34d-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ee34d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ee34d-121">Authorization</span></span>  | <span data-ttu-id="ee34d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ee34d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ee34d-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ee34d-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="ee34d-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="ee34d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee34d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ee34d-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="ee34d-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee34d-128">Response</span></span>

<span data-ttu-id="ee34d-129">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ee34d-129">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee34d-130">Пример</span><span class="sxs-lookup"><span data-stu-id="ee34d-130">Example</span></span>
<span data-ttu-id="ee34d-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="ee34d-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ee34d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ee34d-132">Request</span></span>
<span data-ttu-id="ee34d-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ee34d-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ee34d-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="ee34d-134">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_entirerow"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/entireRow
```
# <a name="c"></a>[<span data-ttu-id="ee34d-135">C#</span><span class="sxs-lookup"><span data-stu-id="ee34d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-entirerow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ee34d-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ee34d-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-entirerow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ee34d-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ee34d-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-entirerow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ee34d-138">Java</span><span class="sxs-lookup"><span data-stu-id="ee34d-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-entirerow-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ee34d-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee34d-139">Response</span></span>
<span data-ttu-id="ee34d-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ee34d-140">Here is an example of the response.</span></span> <span data-ttu-id="ee34d-141">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ee34d-141">Note: The response object shown here might be shortened for readability.</span></span>
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
  "description": "Range: EntireRow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

