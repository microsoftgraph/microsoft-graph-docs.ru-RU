---
title: 'Range: insert'
description: Вставляет ячейку или диапазон ячеек на лист вместо этого диапазона, а также сдвигает другие ячейки, чтобы освободить место. Возвращает новый объект Range в пустом месте.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 96d774a111d8a23f57eb3a1667fbaf8d725291a4
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50573693"
---
# <a name="range-insert"></a><span data-ttu-id="3aca2-104">Range: insert</span><span class="sxs-lookup"><span data-stu-id="3aca2-104">Range: insert</span></span>

<span data-ttu-id="3aca2-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3aca2-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3aca2-p102">Вставляет ячейку или диапазон ячеек на лист вместо этого диапазона, а также сдвигает другие ячейки, чтобы освободить место. Возвращает новый объект Range в пустом месте.</span><span class="sxs-lookup"><span data-stu-id="3aca2-p102">Inserts a cell or a range of cells into the worksheet in place of this range, and shifts the other cells to make space. Returns a new Range object at the now blank space.</span></span>
## <a name="permissions"></a><span data-ttu-id="3aca2-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3aca2-108">Permissions</span></span>
<span data-ttu-id="3aca2-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3aca2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3aca2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3aca2-111">Permission type</span></span>      | <span data-ttu-id="3aca2-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3aca2-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3aca2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3aca2-113">Delegated (work or school account)</span></span> | <span data-ttu-id="3aca2-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3aca2-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3aca2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3aca2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3aca2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3aca2-116">Not supported.</span></span>    |
|<span data-ttu-id="3aca2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3aca2-117">Application</span></span> | <span data-ttu-id="3aca2-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3aca2-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3aca2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3aca2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/names/{name}/range/insert
POST /me/drive/root:/{item-path}:/workbook/names/{name}/range/insert
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/insert
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/insert
POST /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/insert
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/insert

```
## <a name="request-headers"></a><span data-ttu-id="3aca2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3aca2-120">Request headers</span></span>
| <span data-ttu-id="3aca2-121">Имя</span><span class="sxs-lookup"><span data-stu-id="3aca2-121">Name</span></span>       | <span data-ttu-id="3aca2-122">Описание</span><span class="sxs-lookup"><span data-stu-id="3aca2-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3aca2-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3aca2-123">Authorization</span></span>  | <span data-ttu-id="3aca2-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3aca2-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3aca2-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3aca2-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="3aca2-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="3aca2-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3aca2-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3aca2-129">Request body</span></span>
<span data-ttu-id="3aca2-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="3aca2-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3aca2-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="3aca2-131">Parameter</span></span>    | <span data-ttu-id="3aca2-132">Тип</span><span class="sxs-lookup"><span data-stu-id="3aca2-132">Type</span></span>   |<span data-ttu-id="3aca2-133">Описание</span><span class="sxs-lookup"><span data-stu-id="3aca2-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3aca2-134">shift</span><span class="sxs-lookup"><span data-stu-id="3aca2-134">shift</span></span>|<span data-ttu-id="3aca2-135">string</span><span class="sxs-lookup"><span data-stu-id="3aca2-135">string</span></span>|<span data-ttu-id="3aca2-136">Определяет способ сдвига ячеек.</span><span class="sxs-lookup"><span data-stu-id="3aca2-136">Specifies which way to shift the cells.</span></span>  <span data-ttu-id="3aca2-137">Возможные значения: `Down` , `Right` .</span><span class="sxs-lookup"><span data-stu-id="3aca2-137">The possible values are: `Down`, `Right`.</span></span>|

## <a name="response"></a><span data-ttu-id="3aca2-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="3aca2-138">Response</span></span>

<span data-ttu-id="3aca2-139">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3aca2-139">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3aca2-140">Пример</span><span class="sxs-lookup"><span data-stu-id="3aca2-140">Example</span></span>
<span data-ttu-id="3aca2-141">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="3aca2-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3aca2-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="3aca2-142">Request</span></span>
<span data-ttu-id="3aca2-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3aca2-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3aca2-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="3aca2-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "range_insert"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/insert
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```
# <a name="c"></a>[<span data-ttu-id="3aca2-145">C#</span><span class="sxs-lookup"><span data-stu-id="3aca2-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-insert-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3aca2-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3aca2-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-insert-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3aca2-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3aca2-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-insert-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3aca2-148">Java</span><span class="sxs-lookup"><span data-stu-id="3aca2-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-insert-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3aca2-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="3aca2-149">Response</span></span>
<span data-ttu-id="3aca2-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3aca2-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Range: insert",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

