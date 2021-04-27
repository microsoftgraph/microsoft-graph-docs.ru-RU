---
title: Список TableColumnCollection
description: Получение списка объектов tablecolumn.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: e60e79e836c3bfcc4ff06dd5652f5f238dc1cfb0
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054814"
---
# <a name="list-tablecolumncollection"></a><span data-ttu-id="55577-103">Список TableColumnCollection</span><span class="sxs-lookup"><span data-stu-id="55577-103">List TableColumnCollection</span></span>

<span data-ttu-id="55577-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55577-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55577-105">Получение списка объектов tablecolumn.</span><span class="sxs-lookup"><span data-stu-id="55577-105">Retrieve a list of tablecolumn objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="55577-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="55577-106">Permissions</span></span>
<span data-ttu-id="55577-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55577-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55577-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="55577-109">Permission type</span></span>      | <span data-ttu-id="55577-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="55577-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="55577-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="55577-111">Delegated (work or school account)</span></span> | <span data-ttu-id="55577-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="55577-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="55577-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="55577-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55577-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="55577-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="55577-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="55577-115">Application</span></span> | <span data-ttu-id="55577-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55577-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="55577-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="55577-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/tables/{id|name}/columns
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/columns
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/columns
```
## <a name="optional-query-parameters"></a><span data-ttu-id="55577-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="55577-118">Optional query parameters</span></span>
<span data-ttu-id="55577-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="55577-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="55577-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="55577-120">Request headers</span></span>
| <span data-ttu-id="55577-121">Имя</span><span class="sxs-lookup"><span data-stu-id="55577-121">Name</span></span>      |<span data-ttu-id="55577-122">Описание</span><span class="sxs-lookup"><span data-stu-id="55577-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="55577-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="55577-123">Authorization</span></span>  | <span data-ttu-id="55577-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="55577-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="55577-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="55577-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="55577-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="55577-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="55577-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="55577-129">Request body</span></span>
<span data-ttu-id="55577-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="55577-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55577-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="55577-131">Response</span></span>

<span data-ttu-id="55577-132">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [workbookTableColumn](../resources/workbooktablecolumn.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="55577-132">If successful, this method returns a `200 OK` response code and collection of [workbookTableColumn](../resources/workbooktablecolumn.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="55577-133">Пример</span><span class="sxs-lookup"><span data-stu-id="55577-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="55577-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="55577-134">Request</span></span>
<span data-ttu-id="55577-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="55577-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="55577-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="55577-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tablecolumncollection"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns
```
# <a name="c"></a>[<span data-ttu-id="55577-137">C#</span><span class="sxs-lookup"><span data-stu-id="55577-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tablecolumncollection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="55577-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="55577-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tablecolumncollection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="55577-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="55577-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tablecolumncollection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="55577-140">Java</span><span class="sxs-lookup"><span data-stu-id="55577-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tablecolumncollection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="55577-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="55577-141">Response</span></span>
<span data-ttu-id="55577-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="55577-142">Here is an example of the response.</span></span> <span data-ttu-id="55577-143">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="55577-143">Note: The response object shown here might be shortened for readability.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List TableColumnCollection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
