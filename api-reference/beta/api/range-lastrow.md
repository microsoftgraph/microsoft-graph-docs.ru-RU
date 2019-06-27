---
title: 'Range: LastRow'
description: .
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 0bd18479f62b88d98064380e07a32d9c36c2ae96
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35265550"
---
# <a name="range-lastrow"></a><span data-ttu-id="270b0-103">Range: LastRow</span><span class="sxs-lookup"><span data-stu-id="270b0-103">Range: LastRow</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="270b0-p101">Возвращает последнюю строку в диапазоне. Например, последняя строка в диапазоне "B2:D5" — "B5:D5".</span><span class="sxs-lookup"><span data-stu-id="270b0-p101">Gets the last row within the range. For example, the last row of "B2:D5" is "B5:D5".</span></span>
## <a name="permissions"></a><span data-ttu-id="270b0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="270b0-106">Permissions</span></span>
<span data-ttu-id="270b0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="270b0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="270b0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="270b0-109">Permission type</span></span>      | <span data-ttu-id="270b0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="270b0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="270b0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="270b0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="270b0-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="270b0-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="270b0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="270b0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="270b0-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="270b0-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="270b0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="270b0-115">Application</span></span> | <span data-ttu-id="270b0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="270b0-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="270b0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="270b0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/LastRow
GET /workbook/worksheets/{id|name}/range(address='<address>')/LastRow
GET /workbook/tables/{id|name}/columns/{id|name}/range/LastRow

```
## <a name="request-headers"></a><span data-ttu-id="270b0-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="270b0-118">Request headers</span></span>
| <span data-ttu-id="270b0-119">Имя</span><span class="sxs-lookup"><span data-stu-id="270b0-119">Name</span></span>       | <span data-ttu-id="270b0-120">Описание</span><span class="sxs-lookup"><span data-stu-id="270b0-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="270b0-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="270b0-121">Authorization</span></span>  | <span data-ttu-id="270b0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="270b0-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="270b0-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="270b0-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="270b0-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="270b0-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="270b0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="270b0-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="270b0-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="270b0-128">Response</span></span>

<span data-ttu-id="270b0-129">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/workbookrange.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="270b0-129">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="270b0-130">Пример</span><span class="sxs-lookup"><span data-stu-id="270b0-130">Example</span></span>
<span data-ttu-id="270b0-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="270b0-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="270b0-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="270b0-132">Request</span></span>
<span data-ttu-id="270b0-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="270b0-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_lastrow"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/LastRow
```

##### <a name="response"></a><span data-ttu-id="270b0-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="270b0-134">Response</span></span>
<span data-ttu-id="270b0-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="270b0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="270b0-138">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="270b0-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="270b0-139">C#</span><span class="sxs-lookup"><span data-stu-id="270b0-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/range_lastrow-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="270b0-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="270b0-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/range_lastrow-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="270b0-141">Цель — C</span><span class="sxs-lookup"><span data-stu-id="270b0-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/range_lastrow-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Range: LastRow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/range-lastrow.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/range-lastrow.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/range-lastrow.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
