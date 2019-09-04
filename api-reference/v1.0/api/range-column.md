---
title: 'Range: Column'
description: Возвращает столбец в диапазоне.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: fa3c54928498b3cad7aeb70666436e1bd4fbcb5c
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36728421"
---
# <a name="range-column"></a><span data-ttu-id="bec94-103">Range: Column</span><span class="sxs-lookup"><span data-stu-id="bec94-103">Range: Column</span></span>

<span data-ttu-id="bec94-104">Возвращает столбец в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="bec94-104">Gets a column contained in the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="bec94-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bec94-105">Permissions</span></span>
<span data-ttu-id="bec94-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bec94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bec94-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bec94-108">Permission type</span></span>      | <span data-ttu-id="bec94-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bec94-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bec94-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bec94-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bec94-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bec94-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bec94-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bec94-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bec94-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bec94-113">Not supported.</span></span>    |
|<span data-ttu-id="bec94-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bec94-114">Application</span></span> | <span data-ttu-id="bec94-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bec94-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bec94-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bec94-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/column
GET /workbook/worksheets/{id|name}/range(address='<address>')/column
GET /workbook/tables/{id|name}/columns/{id|name}/range/column

```
## <a name="request-headers"></a><span data-ttu-id="bec94-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bec94-117">Request headers</span></span>
| <span data-ttu-id="bec94-118">Имя</span><span class="sxs-lookup"><span data-stu-id="bec94-118">Name</span></span>       | <span data-ttu-id="bec94-119">Описание</span><span class="sxs-lookup"><span data-stu-id="bec94-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bec94-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bec94-120">Authorization</span></span>  | <span data-ttu-id="bec94-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bec94-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bec94-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="bec94-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="bec94-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="bec94-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="bec94-126">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="bec94-126">Path parameters</span></span>
<span data-ttu-id="bec94-127">В пути запроса укажите следующие параметры.</span><span class="sxs-lookup"><span data-stu-id="bec94-127">In the request path, provide the following parameters.</span></span>

| <span data-ttu-id="bec94-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="bec94-128">Parameter</span></span>    | <span data-ttu-id="bec94-129">Тип</span><span class="sxs-lookup"><span data-stu-id="bec94-129">Type</span></span>   |<span data-ttu-id="bec94-130">Описание</span><span class="sxs-lookup"><span data-stu-id="bec94-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bec94-131">column</span><span class="sxs-lookup"><span data-stu-id="bec94-131">column</span></span>|<span data-ttu-id="bec94-132">Int32</span><span class="sxs-lookup"><span data-stu-id="bec94-132">Int32</span></span>|<span data-ttu-id="bec94-p104">Номер столбца диапазона, который требуется извлечь. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="bec94-p104">Column number of the range to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="bec94-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="bec94-135">Response</span></span>

<span data-ttu-id="bec94-136">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="bec94-136">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bec94-137">Пример</span><span class="sxs-lookup"><span data-stu-id="bec94-137">Example</span></span>
<span data-ttu-id="bec94-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="bec94-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="bec94-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="bec94-139">Request</span></span>
<span data-ttu-id="bec94-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bec94-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bec94-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="bec94-141">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_column"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/column(column=5)
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bec94-142">C#</span><span class="sxs-lookup"><span data-stu-id="bec94-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-column-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bec94-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bec94-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-column-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bec94-144">Цель — C</span><span class="sxs-lookup"><span data-stu-id="bec94-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-column-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="bec94-145">Java</span><span class="sxs-lookup"><span data-stu-id="bec94-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-column-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="bec94-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="bec94-146">Response</span></span>
<span data-ttu-id="bec94-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bec94-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: Column",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
