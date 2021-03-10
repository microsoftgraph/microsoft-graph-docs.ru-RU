---
title: 'Range: Column'
description: Возвращает столбец в диапазоне.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 5fd63973a74b9ee7f283b1c526f819aac463a859
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50577781"
---
# <a name="range-column"></a><span data-ttu-id="0c8b9-103">Range: Column</span><span class="sxs-lookup"><span data-stu-id="0c8b9-103">Range: Column</span></span>

<span data-ttu-id="0c8b9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c8b9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0c8b9-105">Возвращает столбец в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="0c8b9-105">Gets a column contained in the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="0c8b9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0c8b9-106">Permissions</span></span>
<span data-ttu-id="0c8b9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c8b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c8b9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0c8b9-109">Permission type</span></span>      | <span data-ttu-id="0c8b9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0c8b9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0c8b9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0c8b9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0c8b9-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0c8b9-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0c8b9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0c8b9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c8b9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c8b9-114">Not supported.</span></span>    |
|<span data-ttu-id="0c8b9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0c8b9-115">Application</span></span> | <span data-ttu-id="0c8b9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c8b9-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0c8b9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0c8b9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/names/{name}/range/column
GET /me/drive/root:/{item-path}:/workbook/names/{name}/range/column
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/column
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/column
GET /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/column
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/column

```
## <a name="request-headers"></a><span data-ttu-id="0c8b9-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0c8b9-118">Request headers</span></span>
| <span data-ttu-id="0c8b9-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0c8b9-119">Name</span></span>       | <span data-ttu-id="0c8b9-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0c8b9-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0c8b9-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0c8b9-121">Authorization</span></span>  | <span data-ttu-id="0c8b9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0c8b9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0c8b9-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0c8b9-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="0c8b9-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="0c8b9-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="0c8b9-127">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="0c8b9-127">Path parameters</span></span>
<span data-ttu-id="0c8b9-128">В пути запроса укай следующие параметры.</span><span class="sxs-lookup"><span data-stu-id="0c8b9-128">In the request path, provide the following parameters.</span></span>

| <span data-ttu-id="0c8b9-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="0c8b9-129">Parameter</span></span>    | <span data-ttu-id="0c8b9-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0c8b9-130">Type</span></span>   |<span data-ttu-id="0c8b9-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0c8b9-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c8b9-132">column</span><span class="sxs-lookup"><span data-stu-id="0c8b9-132">column</span></span>|<span data-ttu-id="0c8b9-133">Int32</span><span class="sxs-lookup"><span data-stu-id="0c8b9-133">Int32</span></span>|<span data-ttu-id="0c8b9-p104">Номер столбца диапазона, который требуется извлечь. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="0c8b9-p104">Column number of the range to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="0c8b9-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c8b9-136">Response</span></span>

<span data-ttu-id="0c8b9-137">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0c8b9-137">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c8b9-138">Пример</span><span class="sxs-lookup"><span data-stu-id="0c8b9-138">Example</span></span>
<span data-ttu-id="0c8b9-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="0c8b9-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0c8b9-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="0c8b9-140">Request</span></span>
<span data-ttu-id="0c8b9-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0c8b9-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0c8b9-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="0c8b9-142">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_column"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/column(column=5)
```
# <a name="c"></a>[<span data-ttu-id="0c8b9-143">C#</span><span class="sxs-lookup"><span data-stu-id="0c8b9-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-column-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0c8b9-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0c8b9-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-column-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0c8b9-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0c8b9-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-column-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0c8b9-146">Java</span><span class="sxs-lookup"><span data-stu-id="0c8b9-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-column-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0c8b9-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c8b9-147">Response</span></span>
<span data-ttu-id="0c8b9-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0c8b9-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

