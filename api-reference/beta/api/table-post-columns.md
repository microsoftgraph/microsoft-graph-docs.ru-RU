---
title: Создание объекта TableColumn
description: С помощью этого API можно создать объект TableColumn.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: cc86f886f9abde26a6d55f529164e5382537d5b0
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271115"
---
# <a name="create-tablecolumn"></a><span data-ttu-id="c8c22-103">Создание объекта TableColumn</span><span class="sxs-lookup"><span data-stu-id="c8c22-103">Create TableColumn</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8c22-104">С помощью этого API можно создать объект TableColumn.</span><span class="sxs-lookup"><span data-stu-id="c8c22-104">Use this API to create a new TableColumn.</span></span>
## <a name="permissions"></a><span data-ttu-id="c8c22-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c8c22-105">Permissions</span></span>
<span data-ttu-id="c8c22-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8c22-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8c22-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c8c22-108">Permission type</span></span>      | <span data-ttu-id="c8c22-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c8c22-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c8c22-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c8c22-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c8c22-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c8c22-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c8c22-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c8c22-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8c22-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c8c22-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c8c22-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c8c22-114">Application</span></span> | <span data-ttu-id="c8c22-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8c22-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c8c22-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c8c22-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns

```
## <a name="request-headers"></a><span data-ttu-id="c8c22-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c8c22-117">Request headers</span></span>
| <span data-ttu-id="c8c22-118">Имя</span><span class="sxs-lookup"><span data-stu-id="c8c22-118">Name</span></span>       | <span data-ttu-id="c8c22-119">Описание</span><span class="sxs-lookup"><span data-stu-id="c8c22-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c8c22-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c8c22-120">Authorization</span></span>  | <span data-ttu-id="c8c22-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c8c22-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c8c22-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c8c22-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="c8c22-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="c8c22-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8c22-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c8c22-126">Request body</span></span>
<span data-ttu-id="c8c22-127">В тексте запроса добавьте представление объекта [воркбуктаблеколумн](../resources/workbooktablecolumn.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c8c22-127">In the request body, supply a JSON representation of [workbookTableColumn](../resources/workbooktablecolumn.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c8c22-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8c22-128">Response</span></span>

<span data-ttu-id="c8c22-129">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [воркбуктаблеколумн](../resources/workbooktablecolumn.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c8c22-129">If successful, this method returns `201 Created` response code and [workbookTableColumn](../resources/workbooktablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8c22-130">Пример</span><span class="sxs-lookup"><span data-stu-id="c8c22-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c8c22-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8c22-131">Request</span></span>
<span data-ttu-id="c8c22-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c8c22-132">Here is an example of the request.</span></span>
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
<span data-ttu-id="c8c22-133">В тексте запроса добавьте представление объекта [воркбуктаблеколумн](../resources/workbooktablecolumn.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c8c22-133">In the request body, supply a JSON representation of [workbookTableColumn](../resources/workbooktablecolumn.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="c8c22-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8c22-134">Response</span></span>
<span data-ttu-id="c8c22-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c8c22-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c8c22-138">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="c8c22-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c8c22-139">C#</span><span class="sxs-lookup"><span data-stu-id="c8c22-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_tablecolumn_from_table-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c8c22-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="c8c22-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_tablecolumn_from_table-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c8c22-141">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c8c22-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_tablecolumn_from_table-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/table-post-columns.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/table-post-columns.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/table-post-columns.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
