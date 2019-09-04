---
title: 'TableColumnCollection: add'
description: Добавляет новый столбец в таблицу.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 6632ba9b8809500612b312cf792907586a6c6bd7
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36729114"
---
# <a name="tablecolumncollection-add"></a><span data-ttu-id="62837-103">TableColumnCollection: add</span><span class="sxs-lookup"><span data-stu-id="62837-103">TableColumnCollection: add</span></span>

<span data-ttu-id="62837-104">Добавляет новый столбец в таблицу.</span><span class="sxs-lookup"><span data-stu-id="62837-104">Adds a new column to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="62837-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="62837-105">Permissions</span></span>
<span data-ttu-id="62837-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62837-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62837-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="62837-108">Permission type</span></span>      | <span data-ttu-id="62837-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="62837-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="62837-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="62837-110">Delegated (work or school account)</span></span> | <span data-ttu-id="62837-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="62837-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="62837-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="62837-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62837-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62837-113">Not supported.</span></span>    |
|<span data-ttu-id="62837-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="62837-114">Application</span></span> | <span data-ttu-id="62837-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62837-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="62837-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="62837-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/add

```
## <a name="request-headers"></a><span data-ttu-id="62837-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="62837-117">Request headers</span></span>
| <span data-ttu-id="62837-118">Имя</span><span class="sxs-lookup"><span data-stu-id="62837-118">Name</span></span>       | <span data-ttu-id="62837-119">Описание</span><span class="sxs-lookup"><span data-stu-id="62837-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="62837-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="62837-120">Authorization</span></span>  | <span data-ttu-id="62837-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="62837-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="62837-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="62837-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="62837-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="62837-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="62837-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="62837-126">Request body</span></span>
<span data-ttu-id="62837-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="62837-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="62837-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="62837-128">Parameter</span></span>    | <span data-ttu-id="62837-129">Тип</span><span class="sxs-lookup"><span data-stu-id="62837-129">Type</span></span>   |<span data-ttu-id="62837-130">Описание</span><span class="sxs-lookup"><span data-stu-id="62837-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="62837-131">index</span><span class="sxs-lookup"><span data-stu-id="62837-131">index</span></span>|<span data-ttu-id="62837-132">Int32</span><span class="sxs-lookup"><span data-stu-id="62837-132">Int32</span></span>|<span data-ttu-id="62837-p104">Определяет относительную позицию нового столбца. Предыдущий столбец на этой позиции сдвигается вправо. Значение индекса должно быть равно или меньше значения индекса последнего столбца, чтобы его невозможно было использовать для добавления столбца в конце таблицы. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="62837-p104">Specifies the relative position of the new column. The previous column at this position is shifted to the right. The index value should be equal to or less than the last column's index value, so it cannot be used to append a column at the end of the table. Zero-indexed.</span></span>|
|<span data-ttu-id="62837-137">values</span><span class="sxs-lookup"><span data-stu-id="62837-137">values</span></span>|<span data-ttu-id="62837-138">Json</span><span class="sxs-lookup"><span data-stu-id="62837-138">Json</span></span>|<span data-ttu-id="62837-p105">Необязательный параметр. Двухмерный массив неформатированных значений столбца таблицы.</span><span class="sxs-lookup"><span data-stu-id="62837-p105">Optional. A 2-dimensional array of unformatted values of the table column.</span></span>|
|<span data-ttu-id="62837-141">name</span><span class="sxs-lookup"><span data-stu-id="62837-141">name</span></span>|<span data-ttu-id="62837-142">string</span><span class="sxs-lookup"><span data-stu-id="62837-142">string</span></span>|<span data-ttu-id="62837-143">name</span><span class="sxs-lookup"><span data-stu-id="62837-143">name</span></span>
## <a name="response"></a><span data-ttu-id="62837-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="62837-144">Response</span></span>

<span data-ttu-id="62837-145">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект [воркбуктаблеколумн](../resources/workbooktablecolumn.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="62837-145">If successful, this method returns `200 OK` response code and [WorkbookTableColumn](../resources/workbooktablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62837-146">Пример</span><span class="sxs-lookup"><span data-stu-id="62837-146">Example</span></span>
<span data-ttu-id="62837-147">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="62837-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="62837-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="62837-148">Request</span></span>
<span data-ttu-id="62837-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="62837-149">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="62837-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="62837-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tablecolumncollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/add
Content-type: application/json
Content-length: 51

{
  "index": 3,
  "values": [
    {
    }
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="62837-151">C#</span><span class="sxs-lookup"><span data-stu-id="62837-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablecolumncollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="62837-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="62837-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablecolumncollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="62837-153">Цель — C</span><span class="sxs-lookup"><span data-stu-id="62837-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablecolumncollection-add-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="62837-154">Java</span><span class="sxs-lookup"><span data-stu-id="62837-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablecolumncollection-add-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="62837-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="62837-155">Response</span></span>
<span data-ttu-id="62837-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="62837-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableColumnCollection: add",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/api/tablecolumncollection-add.md/tablecolumncollection_add/values:
      Inconsistent types between parameter (Object) and table (None)",
    "Error: /api-reference/v1.0/api/tablecolumncollection-add.md/tablecolumncollection_add/values:
      Type mismatch between example and table. Parameter name: values; example type (Collection(Object)) is a collection, while the table description type (microsoft.graph.Json) is not."
  ],
  "tocPath": ""
}-->
