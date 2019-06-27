---
title: 'TableRow: Range'
description: Возвращает объект диапазона, связанный со всей строкой.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6b1ff4f10080e89ab60e17b6733f7bd6b01cc437
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35278752"
---
# <a name="tablerow-range"></a><span data-ttu-id="256d9-103">TableRow: Range</span><span class="sxs-lookup"><span data-stu-id="256d9-103">TableRow: Range</span></span>

<span data-ttu-id="256d9-104">Возвращает объект диапазона, связанный со всей строкой.</span><span class="sxs-lookup"><span data-stu-id="256d9-104">Returns the range object associated with the entire row.</span></span>
## <a name="permissions"></a><span data-ttu-id="256d9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="256d9-105">Permissions</span></span>
<span data-ttu-id="256d9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="256d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="256d9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="256d9-108">Permission type</span></span>      | <span data-ttu-id="256d9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="256d9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="256d9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="256d9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="256d9-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="256d9-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="256d9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="256d9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="256d9-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="256d9-113">Not supported.</span></span>    |
|<span data-ttu-id="256d9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="256d9-114">Application</span></span> | <span data-ttu-id="256d9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="256d9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="256d9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="256d9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/rows/{index}/range
GET /workbook/worksheets/{id|name}/tables/{id|name}/rows/{index}/range

```
## <a name="request-headers"></a><span data-ttu-id="256d9-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="256d9-117">Request headers</span></span>
| <span data-ttu-id="256d9-118">Имя</span><span class="sxs-lookup"><span data-stu-id="256d9-118">Name</span></span>       | <span data-ttu-id="256d9-119">Описание</span><span class="sxs-lookup"><span data-stu-id="256d9-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="256d9-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="256d9-120">Authorization</span></span>  | <span data-ttu-id="256d9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="256d9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="256d9-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="256d9-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="256d9-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="256d9-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="256d9-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="256d9-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="256d9-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="256d9-127">Response</span></span>

<span data-ttu-id="256d9-128">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="256d9-128">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="256d9-129">Пример</span><span class="sxs-lookup"><span data-stu-id="256d9-129">Example</span></span>
<span data-ttu-id="256d9-130">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="256d9-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="256d9-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="256d9-131">Request</span></span>
<span data-ttu-id="256d9-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="256d9-132">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "tablerow_range"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}/range
```

##### <a name="response"></a><span data-ttu-id="256d9-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="256d9-133">Response</span></span>
<span data-ttu-id="256d9-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="256d9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="256d9-137">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="256d9-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="256d9-138">C#</span><span class="sxs-lookup"><span data-stu-id="256d9-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/tablerow_range-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="256d9-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="256d9-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/tablerow_range-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="256d9-140">Цель — C</span><span class="sxs-lookup"><span data-stu-id="256d9-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/tablerow_range-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableRow: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/tablerow-range.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/tablerow-range.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/tablerow-range.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
