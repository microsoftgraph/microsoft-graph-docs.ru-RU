---
title: Создание объекта TableColumn
description: С помощью этого API можно создать объект TableColumn.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 6d843ae7acc71f9d519bf0c59ab056bf0c393254
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35991151"
---
# <a name="create-tablecolumn"></a><span data-ttu-id="a7fb9-103">Создание объекта TableColumn</span><span class="sxs-lookup"><span data-stu-id="a7fb9-103">Create TableColumn</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7fb9-104">С помощью этого API можно создать объект TableColumn.</span><span class="sxs-lookup"><span data-stu-id="a7fb9-104">Use this API to create a new TableColumn.</span></span>
## <a name="permissions"></a><span data-ttu-id="a7fb9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a7fb9-105">Permissions</span></span>
<span data-ttu-id="a7fb9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7fb9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7fb9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a7fb9-108">Permission type</span></span>      | <span data-ttu-id="a7fb9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a7fb9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a7fb9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a7fb9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a7fb9-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a7fb9-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a7fb9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a7fb9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7fb9-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a7fb9-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a7fb9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a7fb9-114">Application</span></span> | <span data-ttu-id="a7fb9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7fb9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a7fb9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a7fb9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns

```
## <a name="request-headers"></a><span data-ttu-id="a7fb9-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a7fb9-117">Request headers</span></span>
| <span data-ttu-id="a7fb9-118">Имя</span><span class="sxs-lookup"><span data-stu-id="a7fb9-118">Name</span></span>       | <span data-ttu-id="a7fb9-119">Описание</span><span class="sxs-lookup"><span data-stu-id="a7fb9-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a7fb9-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a7fb9-120">Authorization</span></span>  | <span data-ttu-id="a7fb9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a7fb9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a7fb9-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a7fb9-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="a7fb9-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="a7fb9-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7fb9-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a7fb9-126">Request body</span></span>
<span data-ttu-id="a7fb9-127">В тексте запроса добавьте представление объекта [воркбуктаблеколумн](../resources/workbooktablecolumn.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a7fb9-127">In the request body, supply a JSON representation of [workbookTableColumn](../resources/workbooktablecolumn.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a7fb9-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7fb9-128">Response</span></span>

<span data-ttu-id="a7fb9-129">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [воркбуктаблеколумн](../resources/workbooktablecolumn.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a7fb9-129">If successful, this method returns `201 Created` response code and [workbookTableColumn](../resources/workbooktablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7fb9-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a7fb9-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a7fb9-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a7fb9-131">Request</span></span>
<span data-ttu-id="a7fb9-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a7fb9-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a7fb9-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a7fb9-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_tablecolumn_from_table"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a7fb9-134">C#</span><span class="sxs-lookup"><span data-stu-id="a7fb9-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-tablecolumn-from-table-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a7fb9-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="a7fb9-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-tablecolumn-from-table-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a7fb9-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="a7fb9-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-tablecolumn-from-table-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a7fb9-137">Java</span><span class="sxs-lookup"><span data-stu-id="a7fb9-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-tablecolumn-from-table-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="a7fb9-138">В тексте запроса добавьте представление объекта [воркбуктаблеколумн](../resources/workbooktablecolumn.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a7fb9-138">In the request body, supply a JSON representation of [workbookTableColumn](../resources/workbooktablecolumn.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="a7fb9-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7fb9-139">Response</span></span>
<span data-ttu-id="a7fb9-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a7fb9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "id": 99,
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
