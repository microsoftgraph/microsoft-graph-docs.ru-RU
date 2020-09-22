---
title: 'TableColumnCollection: add'
description: Добавляет новый столбец в таблицу.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 9e57e81974f28aefcef35b341c458f8431426308
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48012903"
---
# <a name="tablecolumncollection-add"></a><span data-ttu-id="e7936-103">TableColumnCollection: add</span><span class="sxs-lookup"><span data-stu-id="e7936-103">TableColumnCollection: add</span></span>

<span data-ttu-id="e7936-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7936-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e7936-105">Добавляет новый столбец в таблицу.</span><span class="sxs-lookup"><span data-stu-id="e7936-105">Adds a new column to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="e7936-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e7936-106">Permissions</span></span>
<span data-ttu-id="e7936-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7936-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7936-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e7936-109">Permission type</span></span>      | <span data-ttu-id="e7936-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e7936-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7936-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e7936-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e7936-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e7936-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e7936-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e7936-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7936-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7936-114">Not supported.</span></span>    |
|<span data-ttu-id="e7936-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e7936-115">Application</span></span> | <span data-ttu-id="e7936-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7936-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e7936-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e7936-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/add

```
## <a name="request-headers"></a><span data-ttu-id="e7936-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e7936-118">Request headers</span></span>
| <span data-ttu-id="e7936-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e7936-119">Name</span></span>       | <span data-ttu-id="e7936-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e7936-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e7936-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e7936-121">Authorization</span></span>  | <span data-ttu-id="e7936-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e7936-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e7936-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e7936-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="e7936-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="e7936-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7936-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e7936-127">Request body</span></span>
<span data-ttu-id="e7936-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="e7936-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e7936-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="e7936-129">Parameter</span></span>    | <span data-ttu-id="e7936-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e7936-130">Type</span></span>   |<span data-ttu-id="e7936-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e7936-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e7936-132">index</span><span class="sxs-lookup"><span data-stu-id="e7936-132">index</span></span>|<span data-ttu-id="e7936-133">Int32</span><span class="sxs-lookup"><span data-stu-id="e7936-133">Int32</span></span>|<span data-ttu-id="e7936-p104">Определяет относительную позицию нового столбца. Предыдущий столбец на этой позиции сдвигается вправо. Значение индекса должно быть равно или меньше значения индекса последнего столбца, чтобы его невозможно было использовать для добавления столбца в конце таблицы. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="e7936-p104">Specifies the relative position of the new column. The previous column at this position is shifted to the right. The index value should be equal to or less than the last column's index value, so it cannot be used to append a column at the end of the table. Zero-indexed.</span></span>|
|<span data-ttu-id="e7936-138">values</span><span class="sxs-lookup"><span data-stu-id="e7936-138">values</span></span>|<span data-ttu-id="e7936-139">Json</span><span class="sxs-lookup"><span data-stu-id="e7936-139">Json</span></span>|<span data-ttu-id="e7936-p105">Необязательный параметр. Двухмерный массив неформатированных значений столбца таблицы.</span><span class="sxs-lookup"><span data-stu-id="e7936-p105">Optional. A 2-dimensional array of unformatted values of the table column.</span></span>|
|<span data-ttu-id="e7936-142">name</span><span class="sxs-lookup"><span data-stu-id="e7936-142">name</span></span>|<span data-ttu-id="e7936-143">string</span><span class="sxs-lookup"><span data-stu-id="e7936-143">string</span></span>|<span data-ttu-id="e7936-144">name</span><span class="sxs-lookup"><span data-stu-id="e7936-144">name</span></span>
## <a name="response"></a><span data-ttu-id="e7936-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7936-145">Response</span></span>

<span data-ttu-id="e7936-146">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [воркбуктаблеколумн](../resources/workbooktablecolumn.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e7936-146">If successful, this method returns `200 OK` response code and [WorkbookTableColumn](../resources/workbooktablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7936-147">Пример</span><span class="sxs-lookup"><span data-stu-id="e7936-147">Example</span></span>
<span data-ttu-id="e7936-148">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="e7936-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e7936-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="e7936-149">Request</span></span>
<span data-ttu-id="e7936-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e7936-150">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e7936-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="e7936-151">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e7936-152">C#</span><span class="sxs-lookup"><span data-stu-id="e7936-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablecolumncollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e7936-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e7936-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablecolumncollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e7936-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e7936-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablecolumncollection-add-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e7936-155">Java</span><span class="sxs-lookup"><span data-stu-id="e7936-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablecolumncollection-add-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e7936-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7936-156">Response</span></span>
<span data-ttu-id="e7936-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e7936-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

