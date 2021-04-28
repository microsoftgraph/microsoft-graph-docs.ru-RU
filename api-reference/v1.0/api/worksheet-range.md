---
title: 'Worksheet: Range'
description: Возвращает объект диапазона, указанный по адресу или имени.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 1ef406f134ca5d5a04aecf7cc37e069b4dd5eef9
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053694"
---
# <a name="worksheet-range"></a><span data-ttu-id="16614-103">Worksheet: Range</span><span class="sxs-lookup"><span data-stu-id="16614-103">Worksheet: Range</span></span>

<span data-ttu-id="16614-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16614-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="16614-105">Возвращает объект диапазона, указанный по адресу или имени.</span><span class="sxs-lookup"><span data-stu-id="16614-105">Gets the range object specified by the address or name.</span></span>
## <a name="permissions"></a><span data-ttu-id="16614-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="16614-106">Permissions</span></span>
<span data-ttu-id="16614-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16614-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16614-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16614-109">Permission type</span></span>      | <span data-ttu-id="16614-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="16614-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16614-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16614-111">Delegated (work or school account)</span></span> | <span data-ttu-id="16614-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="16614-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="16614-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16614-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16614-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16614-114">Not supported.</span></span>    |
|<span data-ttu-id="16614-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="16614-115">Application</span></span> | <span data-ttu-id="16614-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16614-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="16614-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16614-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/range
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range

```
## <a name="request-headers"></a><span data-ttu-id="16614-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="16614-118">Request headers</span></span>
| <span data-ttu-id="16614-119">Имя</span><span class="sxs-lookup"><span data-stu-id="16614-119">Name</span></span>       | <span data-ttu-id="16614-120">Описание</span><span class="sxs-lookup"><span data-stu-id="16614-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="16614-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="16614-121">Authorization</span></span>  | <span data-ttu-id="16614-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="16614-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="16614-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="16614-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="16614-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="16614-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="function-parameters"></a><span data-ttu-id="16614-127">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="16614-127">Function parameters</span></span>

| <span data-ttu-id="16614-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="16614-128">Parameter</span></span>    | <span data-ttu-id="16614-129">Тип</span><span class="sxs-lookup"><span data-stu-id="16614-129">Type</span></span>   |<span data-ttu-id="16614-130">Описание</span><span class="sxs-lookup"><span data-stu-id="16614-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="16614-131">address</span><span class="sxs-lookup"><span data-stu-id="16614-131">address</span></span>|<span data-ttu-id="16614-132">string</span><span class="sxs-lookup"><span data-stu-id="16614-132">string</span></span>|<span data-ttu-id="16614-p104">Необязательный параметр. Адрес или имя диапазона. Если аргумент не указан, возвращается весь диапазон листа.</span><span class="sxs-lookup"><span data-stu-id="16614-p104">Optional. The address or the name of the range. If not specified, the entire worksheet range is returned.</span></span>|

## <a name="response"></a><span data-ttu-id="16614-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="16614-136">Response</span></span>

<span data-ttu-id="16614-137">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="16614-137">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16614-138">Пример</span><span class="sxs-lookup"><span data-stu-id="16614-138">Example</span></span>
<span data-ttu-id="16614-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="16614-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="16614-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="16614-140">Request</span></span>
<span data-ttu-id="16614-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="16614-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="16614-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="16614-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "worksheet_range"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='A1:B2')
```
# <a name="c"></a>[<span data-ttu-id="16614-143">C#</span><span class="sxs-lookup"><span data-stu-id="16614-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheet-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="16614-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="16614-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheet-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="16614-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="16614-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheet-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="16614-146">Java</span><span class="sxs-lookup"><span data-stu-id="16614-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheet-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="16614-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="16614-147">Response</span></span>
<span data-ttu-id="16614-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="16614-148">Here is an example of the response.</span></span> <span data-ttu-id="16614-149">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="16614-149">Note: The response object shown here might be shortened for readability.</span></span>
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

<span data-ttu-id="16614-150">Если необязательный параметр не указан, эта функция возвращает весь диапазон `address` таблиц.</span><span class="sxs-lookup"><span data-stu-id="16614-150">If the optional `address` parameter is not specified, this function returns the entire worksheet range.</span></span>

##### <a name="request"></a><span data-ttu-id="16614-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="16614-151">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="16614-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="16614-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "worksheet_range_noaddress"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/range
```
# <a name="c"></a>[<span data-ttu-id="16614-153">C#</span><span class="sxs-lookup"><span data-stu-id="16614-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheet-range-noaddress-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="16614-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="16614-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheet-range-noaddress-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="16614-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="16614-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheet-range-noaddress-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="16614-156">Java</span><span class="sxs-lookup"><span data-stu-id="16614-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheet-range-noaddress-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="16614-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="16614-157">Response</span></span>

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
  "description": "Worksheet: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

