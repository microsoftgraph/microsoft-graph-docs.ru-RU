---
title: Создание объекта TableColumn
description: С помощью этого API можно создать объект TableColumn.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 00faf3bb2523ed4cfdd4467dcd1a1d1ce0fa2856
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2021
ms.locfileid: "50034256"
---
# <a name="create-tablecolumn"></a><span data-ttu-id="e5902-103">Создание объекта TableColumn</span><span class="sxs-lookup"><span data-stu-id="e5902-103">Create TableColumn</span></span>

<span data-ttu-id="e5902-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5902-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5902-105">С помощью этого API можно создать объект TableColumn.</span><span class="sxs-lookup"><span data-stu-id="e5902-105">Use this API to create a new TableColumn.</span></span>
## <a name="permissions"></a><span data-ttu-id="e5902-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e5902-106">Permissions</span></span>
<span data-ttu-id="e5902-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5902-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5902-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5902-109">Permission type</span></span>      | <span data-ttu-id="e5902-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5902-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5902-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5902-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e5902-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e5902-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e5902-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5902-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5902-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e5902-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e5902-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e5902-115">Application</span></span> | <span data-ttu-id="e5902-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5902-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e5902-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5902-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns

```
## <a name="request-headers"></a><span data-ttu-id="e5902-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e5902-118">Request headers</span></span>
| <span data-ttu-id="e5902-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e5902-119">Name</span></span>       | <span data-ttu-id="e5902-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e5902-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e5902-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e5902-121">Authorization</span></span>  | <span data-ttu-id="e5902-p102">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e5902-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e5902-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e5902-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="e5902-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="e5902-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5902-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e5902-127">Request body</span></span>
<span data-ttu-id="e5902-128">В теле запроса укажу представление объекта [workbookTableColumn](../resources/workbooktablecolumn.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="e5902-128">In the request body, supply a JSON representation of [workbookTableColumn](../resources/workbooktablecolumn.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e5902-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5902-129">Response</span></span>

<span data-ttu-id="e5902-130">В случае успеха этот метод возвращает код отклика и объект `201 Created` [workbookTableColumn](../resources/workbooktablecolumn.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e5902-130">If successful, this method returns `201 Created` response code and [workbookTableColumn](../resources/workbooktablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5902-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e5902-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e5902-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5902-132">Request</span></span>
<span data-ttu-id="e5902-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e5902-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e5902-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="e5902-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_tablecolumn_from_table"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns
Content-type: application/json
Content-length: 81

{
  "id": "99",
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```
# <a name="c"></a>[<span data-ttu-id="e5902-135">C#</span><span class="sxs-lookup"><span data-stu-id="e5902-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-tablecolumn-from-table-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e5902-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e5902-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-tablecolumn-from-table-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e5902-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e5902-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-tablecolumn-from-table-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e5902-138">Java</span><span class="sxs-lookup"><span data-stu-id="e5902-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-tablecolumn-from-table-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="e5902-139">В теле запроса укажу представление объекта [workbookTableColumn](../resources/workbooktablecolumn.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="e5902-139">In the request body, supply a JSON representation of [workbookTableColumn](../resources/workbooktablecolumn.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e5902-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5902-140">Response</span></span>
<span data-ttu-id="e5902-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e5902-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create TableColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


