---
title: 'TableColumnCollection: add'
description: Добавляет новый столбец в таблицу.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: c560b6f3d326555e514b9bd73f2aef08a665606e
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2021
ms.locfileid: "50034317"
---
# <a name="tablecolumncollection-add"></a><span data-ttu-id="00f41-103">TableColumnCollection: add</span><span class="sxs-lookup"><span data-stu-id="00f41-103">TableColumnCollection: add</span></span>

<span data-ttu-id="00f41-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00f41-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00f41-105">Добавляет новый столбец в таблицу.</span><span class="sxs-lookup"><span data-stu-id="00f41-105">Adds a new column to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="00f41-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="00f41-106">Permissions</span></span>
<span data-ttu-id="00f41-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00f41-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00f41-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="00f41-109">Permission type</span></span>      | <span data-ttu-id="00f41-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="00f41-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="00f41-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="00f41-111">Delegated (work or school account)</span></span> | <span data-ttu-id="00f41-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00f41-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="00f41-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="00f41-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00f41-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00f41-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="00f41-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="00f41-115">Application</span></span> | <span data-ttu-id="00f41-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00f41-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="00f41-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="00f41-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/add

```
## <a name="request-headers"></a><span data-ttu-id="00f41-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="00f41-118">Request headers</span></span>
| <span data-ttu-id="00f41-119">Имя</span><span class="sxs-lookup"><span data-stu-id="00f41-119">Name</span></span>       | <span data-ttu-id="00f41-120">Описание</span><span class="sxs-lookup"><span data-stu-id="00f41-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="00f41-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="00f41-121">Authorization</span></span>  | <span data-ttu-id="00f41-p102">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="00f41-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="00f41-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="00f41-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="00f41-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="00f41-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="00f41-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="00f41-127">Request body</span></span>
<span data-ttu-id="00f41-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="00f41-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="00f41-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="00f41-129">Parameter</span></span>    | <span data-ttu-id="00f41-130">Тип</span><span class="sxs-lookup"><span data-stu-id="00f41-130">Type</span></span>   |<span data-ttu-id="00f41-131">Описание</span><span class="sxs-lookup"><span data-stu-id="00f41-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="00f41-132">index</span><span class="sxs-lookup"><span data-stu-id="00f41-132">index</span></span>|<span data-ttu-id="00f41-133">number</span><span class="sxs-lookup"><span data-stu-id="00f41-133">number</span></span>|<span data-ttu-id="00f41-p104">Определяет относительную позицию нового столбца. Предыдущий столбец на этой позиции сдвигается вправо. Значение индекса должно быть равно или меньше значения индекса последнего столбца, чтобы его невозможно было использовать для добавления столбца в конце таблицы. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="00f41-p104">Specifies the relative position of the new column. The previous column at this position is shifted to the right. The index value should be equal to or less than the last column's index value, so it cannot be used to append a column at the end of the table. Zero-indexed.</span></span>|
|<span data-ttu-id="00f41-138">values</span><span class="sxs-lookup"><span data-stu-id="00f41-138">values</span></span>|<span data-ttu-id="00f41-139">Коллекция (boolean, string или number)</span><span class="sxs-lookup"><span data-stu-id="00f41-139">(boolean or string or number) collection</span></span>|<span data-ttu-id="00f41-p105">Необязательный параметр. Двухмерный массив неформатированных значений столбца таблицы.</span><span class="sxs-lookup"><span data-stu-id="00f41-p105">Optional. A 2-dimensional array of unformatted values of the table column.</span></span>|

## <a name="response"></a><span data-ttu-id="00f41-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="00f41-142">Response</span></span>

<span data-ttu-id="00f41-143">В случае успеха этот метод возвращает код отклика и объект `200 OK` [workbookTableColumn](../resources/workbooktablecolumn.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="00f41-143">If successful, this method returns `200 OK` response code and [workbookTableColumn](../resources/workbooktablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00f41-144">Пример</span><span class="sxs-lookup"><span data-stu-id="00f41-144">Example</span></span>
<span data-ttu-id="00f41-145">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="00f41-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="00f41-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="00f41-146">Request</span></span>
<span data-ttu-id="00f41-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="00f41-147">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="00f41-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="00f41-148">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="00f41-149">C#</span><span class="sxs-lookup"><span data-stu-id="00f41-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablecolumncollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="00f41-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="00f41-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablecolumncollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="00f41-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="00f41-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablecolumncollection-add-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="00f41-152">Java</span><span class="sxs-lookup"><span data-stu-id="00f41-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablecolumncollection-add-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="00f41-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="00f41-153">Response</span></span>
<span data-ttu-id="00f41-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="00f41-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "TableColumnCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


