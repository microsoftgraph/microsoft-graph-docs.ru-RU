---
title: Список таблиц
description: Получение списка объектов таблиц.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 14ef87f57976a95c9fa668cef6432650d5255fca
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962684"
---
# <a name="list-tables"></a><span data-ttu-id="01a49-103">Перечисление таблиц</span><span class="sxs-lookup"><span data-stu-id="01a49-103">List tables</span></span>

<span data-ttu-id="01a49-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01a49-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01a49-105">Получение списка объектов таблиц.</span><span class="sxs-lookup"><span data-stu-id="01a49-105">Retrieve a list of table objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="01a49-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="01a49-106">Permissions</span></span>
<span data-ttu-id="01a49-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01a49-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01a49-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01a49-109">Permission type</span></span>      | <span data-ttu-id="01a49-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="01a49-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01a49-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01a49-111">Delegated (work or school account)</span></span> | <span data-ttu-id="01a49-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="01a49-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="01a49-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01a49-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01a49-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="01a49-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="01a49-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01a49-115">Application</span></span> | <span data-ttu-id="01a49-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01a49-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="01a49-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01a49-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/tables
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables
```
## <a name="optional-query-parameters"></a><span data-ttu-id="01a49-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="01a49-118">Optional query parameters</span></span>
<span data-ttu-id="01a49-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="01a49-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="01a49-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="01a49-120">Request headers</span></span>
| <span data-ttu-id="01a49-121">Имя</span><span class="sxs-lookup"><span data-stu-id="01a49-121">Name</span></span>      |<span data-ttu-id="01a49-122">Описание</span><span class="sxs-lookup"><span data-stu-id="01a49-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="01a49-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="01a49-123">Authorization</span></span>  | <span data-ttu-id="01a49-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="01a49-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="01a49-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="01a49-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="01a49-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="01a49-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="01a49-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="01a49-129">Request body</span></span>
<span data-ttu-id="01a49-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="01a49-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01a49-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="01a49-131">Response</span></span>

<span data-ttu-id="01a49-132">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [workbookTable](../resources/workbooktable.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="01a49-132">If successful, this method returns a `200 OK` response code and collection of [workbookTable](../resources/workbooktable.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="01a49-133">Пример</span><span class="sxs-lookup"><span data-stu-id="01a49-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="01a49-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="01a49-134">Request</span></span>
<span data-ttu-id="01a49-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="01a49-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="01a49-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="01a49-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tables_3"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/tables
```
# <a name="c"></a>[<span data-ttu-id="01a49-137">C#</span><span class="sxs-lookup"><span data-stu-id="01a49-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tables-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="01a49-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="01a49-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tables-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="01a49-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="01a49-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tables-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="01a49-140">Java</span><span class="sxs-lookup"><span data-stu-id="01a49-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tables-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="01a49-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="01a49-141">Response</span></span>
<span data-ttu-id="01a49-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="01a49-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
