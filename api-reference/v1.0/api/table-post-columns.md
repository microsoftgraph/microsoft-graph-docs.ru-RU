---
title: Создание объекта TableColumn
description: С помощью этого API можно создать объект TableColumn.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 882d4c697bf2f1463abed90f8dd914c5d9fb3324
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050292"
---
# <a name="create-tablecolumn"></a><span data-ttu-id="339ae-103">Создание объекта TableColumn</span><span class="sxs-lookup"><span data-stu-id="339ae-103">Create TableColumn</span></span>

<span data-ttu-id="339ae-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="339ae-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="339ae-105">С помощью этого API можно создать объект TableColumn.</span><span class="sxs-lookup"><span data-stu-id="339ae-105">Use this API to create a new TableColumn.</span></span>
## <a name="permissions"></a><span data-ttu-id="339ae-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="339ae-106">Permissions</span></span>
<span data-ttu-id="339ae-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="339ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="339ae-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="339ae-109">Permission type</span></span>      | <span data-ttu-id="339ae-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="339ae-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="339ae-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="339ae-111">Delegated (work or school account)</span></span> | <span data-ttu-id="339ae-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="339ae-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="339ae-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="339ae-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="339ae-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="339ae-114">Not supported.</span></span>    |
|<span data-ttu-id="339ae-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="339ae-115">Application</span></span> | <span data-ttu-id="339ae-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="339ae-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="339ae-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="339ae-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/tables/{id|name}/columns
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/columns
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/columns

```
## <a name="request-headers"></a><span data-ttu-id="339ae-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="339ae-118">Request headers</span></span>
| <span data-ttu-id="339ae-119">Имя</span><span class="sxs-lookup"><span data-stu-id="339ae-119">Name</span></span>       | <span data-ttu-id="339ae-120">Описание</span><span class="sxs-lookup"><span data-stu-id="339ae-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="339ae-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="339ae-121">Authorization</span></span>  | <span data-ttu-id="339ae-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="339ae-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="339ae-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="339ae-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="339ae-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="339ae-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="339ae-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="339ae-127">Request body</span></span>
<span data-ttu-id="339ae-128">В корпусе запроса поставляем представление JSON объекта [WorkbookTableColumn.](../resources/workbooktablecolumn.md)</span><span class="sxs-lookup"><span data-stu-id="339ae-128">In the request body, supply a JSON representation of [WorkbookTableColumn](../resources/workbooktablecolumn.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="339ae-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="339ae-129">Response</span></span>

<span data-ttu-id="339ae-130">В случае успешной работы этот метод возвращает код ответа и объект `201 Created` [WorkbookTableColumn](../resources/workbooktablecolumn.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="339ae-130">If successful, this method returns `201 Created` response code and [WorkbookTableColumn](../resources/workbooktablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="339ae-131">Пример</span><span class="sxs-lookup"><span data-stu-id="339ae-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="339ae-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="339ae-132">Request</span></span>
<span data-ttu-id="339ae-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="339ae-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="339ae-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="339ae-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_tablecolumn_from_table"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns
Content-type: application/json
Content-length: 81

{
  "id": "99",
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```
# <a name="c"></a>[<span data-ttu-id="339ae-135">C#</span><span class="sxs-lookup"><span data-stu-id="339ae-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-tablecolumn-from-table-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="339ae-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="339ae-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-tablecolumn-from-table-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="339ae-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="339ae-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-tablecolumn-from-table-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="339ae-138">Java</span><span class="sxs-lookup"><span data-stu-id="339ae-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-tablecolumn-from-table-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="339ae-139">В корпусе запроса поставляем представление JSON объекта [WorkbookTableColumn.](../resources/workbooktablecolumn.md)</span><span class="sxs-lookup"><span data-stu-id="339ae-139">In the request body, supply a JSON representation of [WorkbookTableColumn](../resources/workbooktablecolumn.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="339ae-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="339ae-140">Response</span></span>
<span data-ttu-id="339ae-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="339ae-141">Here is an example of the response.</span></span> <span data-ttu-id="339ae-142">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="339ae-142">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableColumn"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 81

{
  "id": "99",
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create TableColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

