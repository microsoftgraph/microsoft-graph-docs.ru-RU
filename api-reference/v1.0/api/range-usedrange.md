---
title: 'Range: UsedRange'
description: Возвращает используемый диапазон заданного объекта диапазона.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: dc8a8680154db8a165708eb75818285bc565758c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050369"
---
# <a name="range-usedrange"></a><span data-ttu-id="edbba-103">Range: UsedRange</span><span class="sxs-lookup"><span data-stu-id="edbba-103">Range: UsedRange</span></span>

<span data-ttu-id="edbba-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="edbba-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="edbba-105">Возвращает используемый диапазон заданного объекта диапазона.</span><span class="sxs-lookup"><span data-stu-id="edbba-105">Returns the used range of the given range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="edbba-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="edbba-106">Permissions</span></span>
<span data-ttu-id="edbba-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="edbba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="edbba-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="edbba-109">Permission type</span></span>      | <span data-ttu-id="edbba-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="edbba-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="edbba-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="edbba-111">Delegated (work or school account)</span></span> | <span data-ttu-id="edbba-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="edbba-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="edbba-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="edbba-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="edbba-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="edbba-114">Not supported.</span></span>    |
|<span data-ttu-id="edbba-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="edbba-115">Application</span></span> | <span data-ttu-id="edbba-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="edbba-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="edbba-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="edbba-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/names/{name}/range/usedRange
GET /me/drive/root:/{item-path}:/workbook/names/{name}/range/usedRange
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/usedRange
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/usedRange
GET /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/usedRange
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/usedRange

```
## <a name="request-headers"></a><span data-ttu-id="edbba-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="edbba-118">Request headers</span></span>
| <span data-ttu-id="edbba-119">Имя</span><span class="sxs-lookup"><span data-stu-id="edbba-119">Name</span></span>       | <span data-ttu-id="edbba-120">Описание</span><span class="sxs-lookup"><span data-stu-id="edbba-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="edbba-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="edbba-121">Authorization</span></span>  | <span data-ttu-id="edbba-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="edbba-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="edbba-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="edbba-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="edbba-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="edbba-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="edbba-127">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="edbba-127">Path parameters</span></span>
| <span data-ttu-id="edbba-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="edbba-128">Parameter</span></span>    | <span data-ttu-id="edbba-129">Тип</span><span class="sxs-lookup"><span data-stu-id="edbba-129">Type</span></span>   |<span data-ttu-id="edbba-130">Описание</span><span class="sxs-lookup"><span data-stu-id="edbba-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="edbba-131">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="edbba-131">valuesOnly</span></span>|<span data-ttu-id="edbba-132">boolean</span><span class="sxs-lookup"><span data-stu-id="edbba-132">boolean</span></span>|<span data-ttu-id="edbba-p104">Необязательный. Учитывает только ячейки со значениями.</span><span class="sxs-lookup"><span data-stu-id="edbba-p104">Optional. Considers only cells with values as used cells.</span></span>|

## <a name="response"></a><span data-ttu-id="edbba-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="edbba-135">Response</span></span>

<span data-ttu-id="edbba-136">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="edbba-136">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="edbba-137">Пример</span><span class="sxs-lookup"><span data-stu-id="edbba-137">Example</span></span>
<span data-ttu-id="edbba-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="edbba-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="edbba-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="edbba-139">Request</span></span>
<span data-ttu-id="edbba-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="edbba-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="edbba-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="edbba-141">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_usedrange"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/usedRange
```
# <a name="c"></a>[<span data-ttu-id="edbba-142">C#</span><span class="sxs-lookup"><span data-stu-id="edbba-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-usedrange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="edbba-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="edbba-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-usedrange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="edbba-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="edbba-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-usedrange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="edbba-145">Java</span><span class="sxs-lookup"><span data-stu-id="edbba-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-usedrange-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="edbba-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="edbba-146">Response</span></span>
<span data-ttu-id="edbba-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="edbba-147">Here is an example of the response.</span></span> <span data-ttu-id="edbba-148">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="edbba-148">Note: The response object shown here might be shortened for readability.</span></span>

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

<span data-ttu-id="edbba-149">Вот пример, указывающий необязательный `valuesOnly` параметр.</span><span class="sxs-lookup"><span data-stu-id="edbba-149">Here is an example specifying the optional `valuesOnly` parameter.</span></span>

##### <a name="request"></a><span data-ttu-id="edbba-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="edbba-150">Request</span></span>
<span data-ttu-id="edbba-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="edbba-151">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="edbba-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="edbba-152">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_usedrange_valuesonly"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/usedRange(valuesOnly=true)
```
# <a name="c"></a>[<span data-ttu-id="edbba-153">C#</span><span class="sxs-lookup"><span data-stu-id="edbba-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-usedrange-valuesonly-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="edbba-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="edbba-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-usedrange-valuesonly-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="edbba-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="edbba-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-usedrange-valuesonly-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="edbba-156">Java</span><span class="sxs-lookup"><span data-stu-id="edbba-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-usedrange-valuesonly-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="edbba-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="edbba-157">Response</span></span>

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

