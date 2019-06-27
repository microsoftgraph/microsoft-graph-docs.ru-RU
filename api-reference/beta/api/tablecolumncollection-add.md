---
title: 'TableColumnCollection: add'
description: Добавляет новый столбец в таблицу.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6df308e7076ffce00dcaa7401ea6a921334d62b0
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270898"
---
# <a name="tablecolumncollection-add"></a><span data-ttu-id="5e52e-103">TableColumnCollection: add</span><span class="sxs-lookup"><span data-stu-id="5e52e-103">TableColumnCollection: add</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e52e-104">Добавляет новый столбец в таблицу.</span><span class="sxs-lookup"><span data-stu-id="5e52e-104">Adds a new column to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="5e52e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5e52e-105">Permissions</span></span>
<span data-ttu-id="5e52e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e52e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e52e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5e52e-108">Permission type</span></span>      | <span data-ttu-id="5e52e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5e52e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5e52e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5e52e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5e52e-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5e52e-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5e52e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5e52e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e52e-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5e52e-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5e52e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5e52e-114">Application</span></span> | <span data-ttu-id="5e52e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e52e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5e52e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5e52e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/add

```
## <a name="request-headers"></a><span data-ttu-id="5e52e-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5e52e-117">Request headers</span></span>
| <span data-ttu-id="5e52e-118">Имя</span><span class="sxs-lookup"><span data-stu-id="5e52e-118">Name</span></span>       | <span data-ttu-id="5e52e-119">Описание</span><span class="sxs-lookup"><span data-stu-id="5e52e-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5e52e-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5e52e-120">Authorization</span></span>  | <span data-ttu-id="5e52e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5e52e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5e52e-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5e52e-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="5e52e-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="5e52e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e52e-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5e52e-126">Request body</span></span>
<span data-ttu-id="5e52e-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="5e52e-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5e52e-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="5e52e-128">Parameter</span></span>    | <span data-ttu-id="5e52e-129">Тип</span><span class="sxs-lookup"><span data-stu-id="5e52e-129">Type</span></span>   |<span data-ttu-id="5e52e-130">Описание</span><span class="sxs-lookup"><span data-stu-id="5e52e-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e52e-131">index</span><span class="sxs-lookup"><span data-stu-id="5e52e-131">index</span></span>|<span data-ttu-id="5e52e-132">number</span><span class="sxs-lookup"><span data-stu-id="5e52e-132">number</span></span>|<span data-ttu-id="5e52e-p104">Определяет относительную позицию нового столбца. Предыдущий столбец на этой позиции сдвигается вправо. Значение индекса должно быть равно или меньше значения индекса последнего столбца, чтобы его невозможно было использовать для добавления столбца в конце таблицы. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="5e52e-p104">Specifies the relative position of the new column. The previous column at this position is shifted to the right. The index value should be equal to or less than the last column's index value, so it cannot be used to append a column at the end of the table. Zero-indexed.</span></span>|
|<span data-ttu-id="5e52e-137">values</span><span class="sxs-lookup"><span data-stu-id="5e52e-137">values</span></span>|<span data-ttu-id="5e52e-138">(логическая или числовая) коллекция</span><span class="sxs-lookup"><span data-stu-id="5e52e-138">(boolean or string or number) collection</span></span>|<span data-ttu-id="5e52e-p105">Необязательный параметр. Двухмерный массив неформатированных значений столбца таблицы.</span><span class="sxs-lookup"><span data-stu-id="5e52e-p105">Optional. A 2-dimensional array of unformatted values of the table column.</span></span>|

## <a name="response"></a><span data-ttu-id="5e52e-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e52e-141">Response</span></span>

<span data-ttu-id="5e52e-142">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект [воркбуктаблеколумн](../resources/workbooktablecolumn.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5e52e-142">If successful, this method returns `200 OK` response code and [workbookTableColumn](../resources/workbooktablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e52e-143">Пример</span><span class="sxs-lookup"><span data-stu-id="5e52e-143">Example</span></span>
<span data-ttu-id="5e52e-144">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="5e52e-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5e52e-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="5e52e-145">Request</span></span>
<span data-ttu-id="5e52e-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5e52e-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablecolumncollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/add
Content-type: application/json
Content-length: 51

{
  "index": {
  },
  "values": [
    {
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="5e52e-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e52e-147">Response</span></span>
<span data-ttu-id="5e52e-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5e52e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableColumn"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="5e52e-151">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="5e52e-151">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5e52e-152">C#</span><span class="sxs-lookup"><span data-stu-id="5e52e-152">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/tablecolumncollection_add-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5e52e-153">Javascript</span><span class="sxs-lookup"><span data-stu-id="5e52e-153">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/tablecolumncollection_add-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="5e52e-154">Цель — C</span><span class="sxs-lookup"><span data-stu-id="5e52e-154">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/tablecolumncollection_add-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "TableColumnCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/tablecolumncollection-add.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/tablecolumncollection-add.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/tablecolumncollection-add.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
