---
title: 'TableColumnCollection: add'
description: Добавляет новый столбец в таблицу.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 656340fafa39b074f7a1438b2ed9902b4e975ee4
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052679"
---
# <a name="tablecolumncollection-add"></a><span data-ttu-id="bf43f-103">TableColumnCollection: add</span><span class="sxs-lookup"><span data-stu-id="bf43f-103">TableColumnCollection: add</span></span>

<span data-ttu-id="bf43f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf43f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf43f-105">Добавляет новый столбец в таблицу.</span><span class="sxs-lookup"><span data-stu-id="bf43f-105">Adds a new column to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="bf43f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bf43f-106">Permissions</span></span>
<span data-ttu-id="bf43f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf43f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf43f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bf43f-109">Permission type</span></span>      | <span data-ttu-id="bf43f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bf43f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bf43f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bf43f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bf43f-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bf43f-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bf43f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bf43f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf43f-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bf43f-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bf43f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bf43f-115">Application</span></span> | <span data-ttu-id="bf43f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf43f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bf43f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bf43f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/tables/{id|name}/columns/add
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/add
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/columns/add
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/columns/add

```
## <a name="request-headers"></a><span data-ttu-id="bf43f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bf43f-118">Request headers</span></span>
| <span data-ttu-id="bf43f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="bf43f-119">Name</span></span>       | <span data-ttu-id="bf43f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="bf43f-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bf43f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bf43f-121">Authorization</span></span>  | <span data-ttu-id="bf43f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bf43f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bf43f-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="bf43f-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="bf43f-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="bf43f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf43f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bf43f-127">Request body</span></span>
<span data-ttu-id="bf43f-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="bf43f-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="bf43f-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="bf43f-129">Parameter</span></span>    | <span data-ttu-id="bf43f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="bf43f-130">Type</span></span>   |<span data-ttu-id="bf43f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="bf43f-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bf43f-132">index</span><span class="sxs-lookup"><span data-stu-id="bf43f-132">index</span></span>|<span data-ttu-id="bf43f-133">number</span><span class="sxs-lookup"><span data-stu-id="bf43f-133">number</span></span>|<span data-ttu-id="bf43f-p104">Определяет относительную позицию нового столбца. Предыдущий столбец на этой позиции сдвигается вправо. Значение индекса должно быть равно или меньше значения индекса последнего столбца, чтобы его невозможно было использовать для добавления столбца в конце таблицы. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="bf43f-p104">Specifies the relative position of the new column. The previous column at this position is shifted to the right. The index value should be equal to or less than the last column's index value, so it cannot be used to append a column at the end of the table. Zero-indexed.</span></span>|
|<span data-ttu-id="bf43f-138">values</span><span class="sxs-lookup"><span data-stu-id="bf43f-138">values</span></span>|<span data-ttu-id="bf43f-139">(boolean или string or number) collection</span><span class="sxs-lookup"><span data-stu-id="bf43f-139">(boolean or string or number) collection</span></span>|<span data-ttu-id="bf43f-p105">Необязательный параметр. Двухмерный массив неформатированных значений столбца таблицы.</span><span class="sxs-lookup"><span data-stu-id="bf43f-p105">Optional. A 2-dimensional array of unformatted values of the table column.</span></span>|

## <a name="response"></a><span data-ttu-id="bf43f-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf43f-142">Response</span></span>

<span data-ttu-id="bf43f-143">В случае успешной работы этот метод возвращает код ответа и объект `200 OK` [workbookTableColumn](../resources/workbooktablecolumn.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="bf43f-143">If successful, this method returns `200 OK` response code and [workbookTableColumn](../resources/workbooktablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf43f-144">Пример</span><span class="sxs-lookup"><span data-stu-id="bf43f-144">Example</span></span>
<span data-ttu-id="bf43f-145">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="bf43f-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="bf43f-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf43f-146">Request</span></span>
<span data-ttu-id="bf43f-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bf43f-147">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bf43f-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="bf43f-148">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="bf43f-149">C#</span><span class="sxs-lookup"><span data-stu-id="bf43f-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablecolumncollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bf43f-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bf43f-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablecolumncollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bf43f-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bf43f-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablecolumncollection-add-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bf43f-152">Java</span><span class="sxs-lookup"><span data-stu-id="bf43f-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablecolumncollection-add-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="bf43f-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf43f-153">Response</span></span>
<span data-ttu-id="bf43f-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bf43f-154">Here is an example of the response.</span></span> <span data-ttu-id="bf43f-155">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="bf43f-155">Note: The response object shown here might be shortened for readability.</span></span>
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


