---
title: Список таблиц
description: Получение списка объектов таблиц.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 32ace87283cc1f0a9ef07f52acae34632f6942a5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52036130"
---
# <a name="list-tables"></a><span data-ttu-id="c0dbb-103">Перечисление таблиц</span><span class="sxs-lookup"><span data-stu-id="c0dbb-103">List tables</span></span>

<span data-ttu-id="c0dbb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0dbb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0dbb-105">Получение списка объектов таблиц.</span><span class="sxs-lookup"><span data-stu-id="c0dbb-105">Retrieve a list of table objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="c0dbb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c0dbb-106">Permissions</span></span>
<span data-ttu-id="c0dbb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0dbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0dbb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c0dbb-109">Permission type</span></span>      | <span data-ttu-id="c0dbb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c0dbb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0dbb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c0dbb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c0dbb-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0dbb-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c0dbb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c0dbb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0dbb-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0dbb-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c0dbb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c0dbb-115">Application</span></span> | <span data-ttu-id="c0dbb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0dbb-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0dbb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c0dbb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/tables
GET /me/drive/root:/{item-path}:/workbook/tables
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c0dbb-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c0dbb-118">Optional query parameters</span></span>
<span data-ttu-id="c0dbb-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c0dbb-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c0dbb-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c0dbb-120">Request headers</span></span>
| <span data-ttu-id="c0dbb-121">Имя</span><span class="sxs-lookup"><span data-stu-id="c0dbb-121">Name</span></span>      |<span data-ttu-id="c0dbb-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c0dbb-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c0dbb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c0dbb-123">Authorization</span></span>  | <span data-ttu-id="c0dbb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c0dbb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c0dbb-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c0dbb-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="c0dbb-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="c0dbb-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0dbb-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c0dbb-129">Request body</span></span>
<span data-ttu-id="c0dbb-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c0dbb-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0dbb-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0dbb-131">Response</span></span>

<span data-ttu-id="c0dbb-132">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [workbookTable](../resources/workbooktable.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c0dbb-132">If successful, this method returns a `200 OK` response code and collection of [workbookTable](../resources/workbooktable.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c0dbb-133">Пример</span><span class="sxs-lookup"><span data-stu-id="c0dbb-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c0dbb-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="c0dbb-134">Request</span></span>
<span data-ttu-id="c0dbb-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c0dbb-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c0dbb-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="c0dbb-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tables_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables
```
# <a name="c"></a>[<span data-ttu-id="c0dbb-137">C#</span><span class="sxs-lookup"><span data-stu-id="c0dbb-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tables-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c0dbb-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c0dbb-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tables-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c0dbb-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c0dbb-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tables-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c0dbb-140">Java</span><span class="sxs-lookup"><span data-stu-id="c0dbb-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tables-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c0dbb-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0dbb-141">Response</span></span>
<span data-ttu-id="c0dbb-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c0dbb-142">Here is an example of the response.</span></span> <span data-ttu-id="c0dbb-143">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c0dbb-143">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTable",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 158

{
  "value": [
    {
      "id": "99",
      "name": "name-value",
      "showHeaders": true,
      "showTotals": true,
      "style": "style-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List tables",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
