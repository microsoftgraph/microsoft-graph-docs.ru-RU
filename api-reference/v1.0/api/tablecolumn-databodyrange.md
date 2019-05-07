---
title: 'TableColumn: DataBodyRange'
description: Получает объект диапазона, связанный с данными столбца.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 44d167ae77880e19d1b4b80e24228dd293494ce8
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33602744"
---
# <a name="tablecolumn-databodyrange"></a><span data-ttu-id="541db-103">TableColumn: DataBodyRange</span><span class="sxs-lookup"><span data-stu-id="541db-103">TableColumn: DataBodyRange</span></span>

<span data-ttu-id="541db-104">Получает объект диапазона, связанный с данными столбца.</span><span class="sxs-lookup"><span data-stu-id="541db-104">Gets the range object associated with the data body of the column.</span></span>
## <a name="permissions"></a><span data-ttu-id="541db-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="541db-105">Permissions</span></span>
<span data-ttu-id="541db-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="541db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="541db-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="541db-108">Permission type</span></span>      | <span data-ttu-id="541db-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="541db-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="541db-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="541db-110">Delegated (work or school account)</span></span> | <span data-ttu-id="541db-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="541db-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="541db-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="541db-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="541db-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="541db-113">Not supported.</span></span>    |
|<span data-ttu-id="541db-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="541db-114">Application</span></span> | <span data-ttu-id="541db-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="541db-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="541db-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="541db-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/dataBodyRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/dataBodyRange

```
## <a name="request-headers"></a><span data-ttu-id="541db-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="541db-117">Request headers</span></span>
| <span data-ttu-id="541db-118">Имя</span><span class="sxs-lookup"><span data-stu-id="541db-118">Name</span></span>       | <span data-ttu-id="541db-119">Описание</span><span class="sxs-lookup"><span data-stu-id="541db-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="541db-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="541db-120">Authorization</span></span>  | <span data-ttu-id="541db-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="541db-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="541db-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="541db-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="541db-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="541db-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="541db-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="541db-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="541db-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="541db-127">Response</span></span>

<span data-ttu-id="541db-128">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="541db-128">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="541db-129">Пример</span><span class="sxs-lookup"><span data-stu-id="541db-129">Example</span></span>
<span data-ttu-id="541db-130">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="541db-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="541db-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="541db-131">Request</span></span>
<span data-ttu-id="541db-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="541db-132">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "tablecolumn_databodyrange",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/dataBodyRange
```

##### <a name="response"></a><span data-ttu-id="541db-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="541db-133">Response</span></span>
<span data-ttu-id="541db-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="541db-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="541db-137">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="541db-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="541db-138">Языках</span><span class="sxs-lookup"><span data-stu-id="541db-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/tablecolumn_databodyrange-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="541db-139">Язык</span><span class="sxs-lookup"><span data-stu-id="541db-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/tablecolumn_databodyrange-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableColumn: DataBodyRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/tablecolumn-databodyrange.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/tablecolumn-databodyrange.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
