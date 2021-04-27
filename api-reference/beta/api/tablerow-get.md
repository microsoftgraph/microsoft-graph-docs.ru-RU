---
title: Получение объекта TableRow
description: Получение свойств и связей объекта tablerow.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 8c759b28da4ec1f44a019ff27d9fd40e7c47bd51
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051825"
---
# <a name="get-tablerow"></a><span data-ttu-id="bb789-103">Получение объекта TableRow</span><span class="sxs-lookup"><span data-stu-id="bb789-103">Get TableRow</span></span>

<span data-ttu-id="bb789-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb789-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb789-105">Получение свойств и связей объекта tablerow.</span><span class="sxs-lookup"><span data-stu-id="bb789-105">Retrieve the properties and relationships of tablerow object.</span></span>
## <a name="permissions"></a><span data-ttu-id="bb789-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bb789-106">Permissions</span></span>
<span data-ttu-id="bb789-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb789-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb789-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bb789-109">Permission type</span></span>      | <span data-ttu-id="bb789-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bb789-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb789-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bb789-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bb789-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bb789-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bb789-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bb789-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb789-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bb789-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bb789-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bb789-115">Application</span></span> | <span data-ttu-id="bb789-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb789-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bb789-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bb789-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/rows/{index}
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/rows/{index}
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/rows/{index}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bb789-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bb789-118">Optional query parameters</span></span>
<span data-ttu-id="bb789-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bb789-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bb789-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bb789-120">Request headers</span></span>
| <span data-ttu-id="bb789-121">Имя</span><span class="sxs-lookup"><span data-stu-id="bb789-121">Name</span></span>      |<span data-ttu-id="bb789-122">Описание</span><span class="sxs-lookup"><span data-stu-id="bb789-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bb789-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bb789-123">Authorization</span></span>  | <span data-ttu-id="bb789-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb789-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bb789-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="bb789-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="bb789-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="bb789-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb789-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bb789-129">Request body</span></span>
<span data-ttu-id="bb789-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bb789-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb789-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb789-131">Response</span></span>

<span data-ttu-id="bb789-132">В случае успеха этот метод возвращает код отклика и объект `200 OK` [workbookTableRow](../resources/workbooktablerow.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="bb789-132">If successful, this method returns a `200 OK` response code and [workbookTableRow](../resources/workbooktablerow.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bb789-133">Пример</span><span class="sxs-lookup"><span data-stu-id="bb789-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bb789-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="bb789-134">Request</span></span>
<span data-ttu-id="bb789-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bb789-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bb789-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="bb789-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tablerow"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}
```
# <a name="c"></a>[<span data-ttu-id="bb789-137">C#</span><span class="sxs-lookup"><span data-stu-id="bb789-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tablerow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bb789-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bb789-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tablerow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bb789-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bb789-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tablerow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bb789-140">Java</span><span class="sxs-lookup"><span data-stu-id="bb789-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tablerow-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="bb789-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb789-141">Response</span></span>
<span data-ttu-id="bb789-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bb789-142">Here is an example of the response.</span></span> <span data-ttu-id="bb789-143">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="bb789-143">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableRow"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get TableRow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
