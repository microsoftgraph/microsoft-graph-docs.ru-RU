---
title: Создание объекта TableColumn
description: С помощью этого API можно создать объект TableColumn.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: e89fa2a7f1db2811cd3d01b036a12fee51550bd0
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33602835"
---
# <a name="create-tablecolumn"></a><span data-ttu-id="d00d5-103">Создание объекта TableColumn</span><span class="sxs-lookup"><span data-stu-id="d00d5-103">Create TableColumn</span></span>

<span data-ttu-id="d00d5-104">С помощью этого API можно создать объект TableColumn.</span><span class="sxs-lookup"><span data-stu-id="d00d5-104">Use this API to create a new TableColumn.</span></span>
## <a name="permissions"></a><span data-ttu-id="d00d5-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d00d5-105">Permissions</span></span>
<span data-ttu-id="d00d5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d00d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d00d5-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d00d5-108">Permission type</span></span>      | <span data-ttu-id="d00d5-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d00d5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d00d5-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d00d5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d00d5-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d00d5-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d00d5-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d00d5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d00d5-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d00d5-113">Not supported.</span></span>    |
|<span data-ttu-id="d00d5-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d00d5-114">Application</span></span> | <span data-ttu-id="d00d5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d00d5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d00d5-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d00d5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns

```
## <a name="request-headers"></a><span data-ttu-id="d00d5-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d00d5-117">Request headers</span></span>
| <span data-ttu-id="d00d5-118">Имя</span><span class="sxs-lookup"><span data-stu-id="d00d5-118">Name</span></span>       | <span data-ttu-id="d00d5-119">Описание</span><span class="sxs-lookup"><span data-stu-id="d00d5-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d00d5-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d00d5-120">Authorization</span></span>  | <span data-ttu-id="d00d5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d00d5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d00d5-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d00d5-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="d00d5-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="d00d5-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d00d5-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d00d5-126">Request body</span></span>
<span data-ttu-id="d00d5-127">В тексте запроса добавьте представление объекта [Воркбуктаблеколумн](../resources/tablecolumn.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d00d5-127">In the request body, supply a JSON representation of [WorkbookTableColumn](../resources/tablecolumn.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d00d5-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="d00d5-128">Response</span></span>

<span data-ttu-id="d00d5-129">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [воркбуктаблеколумн](../resources/tablecolumn.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d00d5-129">If successful, this method returns `201 Created` response code and [WorkbookTableColumn](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d00d5-130">Пример</span><span class="sxs-lookup"><span data-stu-id="d00d5-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d00d5-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="d00d5-131">Request</span></span>
<span data-ttu-id="d00d5-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d00d5-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_tablecolumn_from_table"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```
<span data-ttu-id="d00d5-133">В тексте запроса добавьте представление объекта [Воркбуктаблеколумн](../resources/tablecolumn.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d00d5-133">In the request body, supply a JSON representation of [WorkbookTableColumn](../resources/tablecolumn.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="d00d5-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d00d5-134">Response</span></span>
<span data-ttu-id="d00d5-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d00d5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d00d5-138">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="d00d5-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d00d5-139">Языках</span><span class="sxs-lookup"><span data-stu-id="d00d5-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_tablecolumn_from_table-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d00d5-140">Язык</span><span class="sxs-lookup"><span data-stu-id="d00d5-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_tablecolumn_from_table-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create TableColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/table-post-columns.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/table-post-columns.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
