---
title: 'Range: insert'
description: Вставляет ячейку или диапазон ячеек на лист вместо этого диапазона, а также сдвигает другие ячейки, чтобы освободить место. Возвращает новый объект Range в пустом месте.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: daa52980d2cec9eb987810dd6083a2b5f723b462
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055108"
---
# <a name="range-insert"></a><span data-ttu-id="2ef9c-104">Range: insert</span><span class="sxs-lookup"><span data-stu-id="2ef9c-104">Range: insert</span></span>

<span data-ttu-id="2ef9c-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ef9c-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ef9c-p102">Вставляет ячейку или диапазон ячеек на лист вместо этого диапазона, а также сдвигает другие ячейки, чтобы освободить место. Возвращает новый объект Range в пустом месте.</span><span class="sxs-lookup"><span data-stu-id="2ef9c-p102">Inserts a cell or a range of cells into the worksheet in place of this range, and shifts the other cells to make space. Returns a new Range object at the now blank space.</span></span>
## <a name="permissions"></a><span data-ttu-id="2ef9c-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2ef9c-108">Permissions</span></span>
<span data-ttu-id="2ef9c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ef9c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ef9c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2ef9c-111">Permission type</span></span>      | <span data-ttu-id="2ef9c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2ef9c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ef9c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2ef9c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="2ef9c-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2ef9c-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2ef9c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2ef9c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ef9c-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2ef9c-116">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2ef9c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2ef9c-117">Application</span></span> | <span data-ttu-id="2ef9c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ef9c-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ef9c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2ef9c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/names/{name}/range/insert
POST /me/drive/root:/{item-path}:/workbook/names/{name}/range/insert
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/insert
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/insert
POST /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/insert
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/insert

```
## <a name="request-headers"></a><span data-ttu-id="2ef9c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2ef9c-120">Request headers</span></span>
| <span data-ttu-id="2ef9c-121">Имя</span><span class="sxs-lookup"><span data-stu-id="2ef9c-121">Name</span></span>       | <span data-ttu-id="2ef9c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="2ef9c-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2ef9c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2ef9c-123">Authorization</span></span>  | <span data-ttu-id="2ef9c-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2ef9c-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2ef9c-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2ef9c-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="2ef9c-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="2ef9c-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ef9c-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2ef9c-129">Request body</span></span>
<span data-ttu-id="2ef9c-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="2ef9c-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2ef9c-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="2ef9c-131">Parameter</span></span>    | <span data-ttu-id="2ef9c-132">Тип</span><span class="sxs-lookup"><span data-stu-id="2ef9c-132">Type</span></span>   |<span data-ttu-id="2ef9c-133">Описание</span><span class="sxs-lookup"><span data-stu-id="2ef9c-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2ef9c-134">shift</span><span class="sxs-lookup"><span data-stu-id="2ef9c-134">shift</span></span>|<span data-ttu-id="2ef9c-135">string</span><span class="sxs-lookup"><span data-stu-id="2ef9c-135">string</span></span>|<span data-ttu-id="2ef9c-p106">Указывает направление сдвига ячеек.  Возможные значения: `Down`, `Right`.</span><span class="sxs-lookup"><span data-stu-id="2ef9c-p106">Specifies which way to shift the cells.  Possible values are: `Down`, `Right`.</span></span>|

## <a name="response"></a><span data-ttu-id="2ef9c-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ef9c-138">Response</span></span>

<span data-ttu-id="2ef9c-139">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/workbookrange.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2ef9c-139">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ef9c-140">Пример</span><span class="sxs-lookup"><span data-stu-id="2ef9c-140">Example</span></span>
<span data-ttu-id="2ef9c-141">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="2ef9c-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2ef9c-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ef9c-142">Request</span></span>
<span data-ttu-id="2ef9c-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2ef9c-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2ef9c-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ef9c-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "range_insert"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/insert
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```
# <a name="c"></a>[<span data-ttu-id="2ef9c-145">C#</span><span class="sxs-lookup"><span data-stu-id="2ef9c-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-insert-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2ef9c-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ef9c-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-insert-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2ef9c-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ef9c-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-insert-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2ef9c-148">Java</span><span class="sxs-lookup"><span data-stu-id="2ef9c-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-insert-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2ef9c-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ef9c-149">Response</span></span>
<span data-ttu-id="2ef9c-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2ef9c-150">Here is an example of the response.</span></span> <span data-ttu-id="2ef9c-151">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2ef9c-151">Note: The response object shown here might be shortened for readability.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Range: insert",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


