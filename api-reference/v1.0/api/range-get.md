---
title: Получение объекта Range
description: Получение свойств и связей объекта диапазона.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 7ca1fc1369aaf46fb808b1f88da1ed01cf39a943
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52035087"
---
# <a name="get-range"></a><span data-ttu-id="edef1-103">Получение диапазона</span><span class="sxs-lookup"><span data-stu-id="edef1-103">Get Range</span></span>

<span data-ttu-id="edef1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="edef1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="edef1-105">Получение свойств и связей объекта диапазона.</span><span class="sxs-lookup"><span data-stu-id="edef1-105">Retrieve the properties and relationships of range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="edef1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="edef1-106">Permissions</span></span>
<span data-ttu-id="edef1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="edef1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="edef1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="edef1-109">Permission type</span></span>      | <span data-ttu-id="edef1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="edef1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="edef1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="edef1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="edef1-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="edef1-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="edef1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="edef1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="edef1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="edef1-114">Not supported.</span></span>    |
|<span data-ttu-id="edef1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="edef1-115">Application</span></span> | <span data-ttu-id="edef1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="edef1-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="edef1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="edef1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')
GET /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range
```
## <a name="optional-query-parameters"></a><span data-ttu-id="edef1-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="edef1-118">Optional query parameters</span></span>
<span data-ttu-id="edef1-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="edef1-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="edef1-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="edef1-120">Request headers</span></span>
| <span data-ttu-id="edef1-121">Имя</span><span class="sxs-lookup"><span data-stu-id="edef1-121">Name</span></span>      |<span data-ttu-id="edef1-122">Описание</span><span class="sxs-lookup"><span data-stu-id="edef1-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="edef1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="edef1-123">Authorization</span></span>  | <span data-ttu-id="edef1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="edef1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="edef1-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="edef1-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="edef1-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="edef1-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="edef1-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="edef1-129">Request body</span></span>
<span data-ttu-id="edef1-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="edef1-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="edef1-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="edef1-131">Response</span></span>

<span data-ttu-id="edef1-132">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="edef1-132">If successful, this method returns a `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="edef1-133">Пример</span><span class="sxs-lookup"><span data-stu-id="edef1-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="edef1-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="edef1-134">Request</span></span>
<span data-ttu-id="edef1-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="edef1-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="edef1-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="edef1-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_range"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range
```
# <a name="c"></a>[<span data-ttu-id="edef1-137">C#</span><span class="sxs-lookup"><span data-stu-id="edef1-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="edef1-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="edef1-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="edef1-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="edef1-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="edef1-140">Java</span><span class="sxs-lookup"><span data-stu-id="edef1-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="edef1-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="edef1-141">Response</span></span>
<span data-ttu-id="edef1-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="edef1-142">Here is an example of the response.</span></span> <span data-ttu-id="edef1-143">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="edef1-143">Note: The response object shown here might be shortened for readability.</span></span>
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
  "description": "Get Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
