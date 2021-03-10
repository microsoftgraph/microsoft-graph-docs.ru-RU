---
title: 'Range: UsedRange'
description: Возвращает используемый диапазон заданного объекта диапазона.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: a56aec44618ef160853d058263a31a0d335d8442
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50576150"
---
# <a name="range-usedrange"></a><span data-ttu-id="bc2dd-103">Range: UsedRange</span><span class="sxs-lookup"><span data-stu-id="bc2dd-103">Range: UsedRange</span></span>

<span data-ttu-id="bc2dd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc2dd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bc2dd-105">Возвращает используемый диапазон заданного объекта диапазона.</span><span class="sxs-lookup"><span data-stu-id="bc2dd-105">Returns the used range of the given range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="bc2dd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bc2dd-106">Permissions</span></span>
<span data-ttu-id="bc2dd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc2dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc2dd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bc2dd-109">Permission type</span></span>      | <span data-ttu-id="bc2dd-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bc2dd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc2dd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bc2dd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bc2dd-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc2dd-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bc2dd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bc2dd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc2dd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc2dd-114">Not supported.</span></span>    |
|<span data-ttu-id="bc2dd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bc2dd-115">Application</span></span> | <span data-ttu-id="bc2dd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc2dd-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc2dd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bc2dd-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/names/{name}/range/usedRange
GET /me/drive/root:/{item-path}:/workbook/names/{name}/range/usedRange
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/usedRange
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/usedRange
GET /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/usedRange
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/usedRange

```
## <a name="request-headers"></a><span data-ttu-id="bc2dd-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bc2dd-118">Request headers</span></span>
| <span data-ttu-id="bc2dd-119">Имя</span><span class="sxs-lookup"><span data-stu-id="bc2dd-119">Name</span></span>       | <span data-ttu-id="bc2dd-120">Описание</span><span class="sxs-lookup"><span data-stu-id="bc2dd-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bc2dd-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bc2dd-121">Authorization</span></span>  | <span data-ttu-id="bc2dd-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bc2dd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bc2dd-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="bc2dd-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="bc2dd-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="bc2dd-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="bc2dd-127">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="bc2dd-127">Path parameters</span></span>
| <span data-ttu-id="bc2dd-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="bc2dd-128">Parameter</span></span>    | <span data-ttu-id="bc2dd-129">Тип</span><span class="sxs-lookup"><span data-stu-id="bc2dd-129">Type</span></span>   |<span data-ttu-id="bc2dd-130">Описание</span><span class="sxs-lookup"><span data-stu-id="bc2dd-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bc2dd-131">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="bc2dd-131">valuesOnly</span></span>|<span data-ttu-id="bc2dd-132">boolean</span><span class="sxs-lookup"><span data-stu-id="bc2dd-132">boolean</span></span>|<span data-ttu-id="bc2dd-p104">Необязательный. Учитывает только ячейки со значениями.</span><span class="sxs-lookup"><span data-stu-id="bc2dd-p104">Optional. Considers only cells with values as used cells.</span></span>|

## <a name="response"></a><span data-ttu-id="bc2dd-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc2dd-135">Response</span></span>

<span data-ttu-id="bc2dd-136">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="bc2dd-136">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc2dd-137">Пример</span><span class="sxs-lookup"><span data-stu-id="bc2dd-137">Example</span></span>
<span data-ttu-id="bc2dd-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="bc2dd-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="bc2dd-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc2dd-139">Request</span></span>
<span data-ttu-id="bc2dd-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bc2dd-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bc2dd-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="bc2dd-141">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_usedrange"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/usedRange
```
# <a name="c"></a>[<span data-ttu-id="bc2dd-142">C#</span><span class="sxs-lookup"><span data-stu-id="bc2dd-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-usedrange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bc2dd-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bc2dd-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-usedrange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bc2dd-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bc2dd-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-usedrange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bc2dd-145">Java</span><span class="sxs-lookup"><span data-stu-id="bc2dd-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-usedrange-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="bc2dd-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc2dd-146">Response</span></span>
<span data-ttu-id="bc2dd-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="bc2dd-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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

<span data-ttu-id="bc2dd-150">Вот пример, указывающий необязательный `valuesOnly` параметр.</span><span class="sxs-lookup"><span data-stu-id="bc2dd-150">Here is an example specifying the optional `valuesOnly` parameter.</span></span>

##### <a name="request"></a><span data-ttu-id="bc2dd-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc2dd-151">Request</span></span>
<span data-ttu-id="bc2dd-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bc2dd-152">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bc2dd-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="bc2dd-153">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_usedrange_valuesonly"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/usedRange(valuesOnly=true)
```
# <a name="c"></a>[<span data-ttu-id="bc2dd-154">C#</span><span class="sxs-lookup"><span data-stu-id="bc2dd-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-usedrange-valuesonly-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bc2dd-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bc2dd-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-usedrange-valuesonly-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bc2dd-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bc2dd-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-usedrange-valuesonly-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bc2dd-157">Java</span><span class="sxs-lookup"><span data-stu-id="bc2dd-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-usedrange-valuesonly-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="bc2dd-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc2dd-158">Response</span></span>

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
  "cellCount": 90,
  "columnCount": 90,
  "columnIndex": 90,
  "valueTypes": "valueTypes-value"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

