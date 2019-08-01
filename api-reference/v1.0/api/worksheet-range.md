---
title: 'Worksheet: Range'
description: Возвращает объект диапазона, указанный по адресу или имени.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: f7d20ad3de65e04e6d5807db50e2b41a9631a09d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36026119"
---
# <a name="worksheet-range"></a><span data-ttu-id="c84f5-103">Worksheet: Range</span><span class="sxs-lookup"><span data-stu-id="c84f5-103">Worksheet: Range</span></span>

<span data-ttu-id="c84f5-104">Возвращает объект диапазона, указанный по адресу или имени.</span><span class="sxs-lookup"><span data-stu-id="c84f5-104">Gets the range object specified by the address or name.</span></span>
## <a name="permissions"></a><span data-ttu-id="c84f5-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c84f5-105">Permissions</span></span>
<span data-ttu-id="c84f5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c84f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c84f5-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c84f5-108">Permission type</span></span>      | <span data-ttu-id="c84f5-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c84f5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c84f5-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c84f5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c84f5-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c84f5-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c84f5-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c84f5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c84f5-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c84f5-113">Not supported.</span></span>    |
|<span data-ttu-id="c84f5-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c84f5-114">Application</span></span> | <span data-ttu-id="c84f5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c84f5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c84f5-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c84f5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/range

```
## <a name="request-headers"></a><span data-ttu-id="c84f5-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c84f5-117">Request headers</span></span>
| <span data-ttu-id="c84f5-118">Имя</span><span class="sxs-lookup"><span data-stu-id="c84f5-118">Name</span></span>       | <span data-ttu-id="c84f5-119">Описание</span><span class="sxs-lookup"><span data-stu-id="c84f5-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c84f5-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c84f5-120">Authorization</span></span>  | <span data-ttu-id="c84f5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c84f5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c84f5-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c84f5-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="c84f5-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="c84f5-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="function-parameters"></a><span data-ttu-id="c84f5-126">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="c84f5-126">Function parameters</span></span>

| <span data-ttu-id="c84f5-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="c84f5-127">Parameter</span></span>    | <span data-ttu-id="c84f5-128">Тип</span><span class="sxs-lookup"><span data-stu-id="c84f5-128">Type</span></span>   |<span data-ttu-id="c84f5-129">Описание</span><span class="sxs-lookup"><span data-stu-id="c84f5-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c84f5-130">address</span><span class="sxs-lookup"><span data-stu-id="c84f5-130">address</span></span>|<span data-ttu-id="c84f5-131">string</span><span class="sxs-lookup"><span data-stu-id="c84f5-131">string</span></span>|<span data-ttu-id="c84f5-p104">Необязательный параметр. Адрес или имя диапазона. Если аргумент не указан, возвращается весь диапазон листа.</span><span class="sxs-lookup"><span data-stu-id="c84f5-p104">Optional. The address or the name of the range. If not specified, the entire worksheet range is returned.</span></span>|

## <a name="response"></a><span data-ttu-id="c84f5-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="c84f5-135">Response</span></span>

<span data-ttu-id="c84f5-136">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c84f5-136">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c84f5-137">Пример</span><span class="sxs-lookup"><span data-stu-id="c84f5-137">Example</span></span>
<span data-ttu-id="c84f5-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="c84f5-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c84f5-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="c84f5-139">Request</span></span>
<span data-ttu-id="c84f5-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c84f5-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c84f5-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="c84f5-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "worksheet_range"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='A1:B2')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c84f5-142">C#</span><span class="sxs-lookup"><span data-stu-id="c84f5-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheet-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c84f5-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="c84f5-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheet-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c84f5-144">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c84f5-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheet-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c84f5-145">Java</span><span class="sxs-lookup"><span data-stu-id="c84f5-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheet-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c84f5-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="c84f5-146">Response</span></span>
<span data-ttu-id="c84f5-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c84f5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<span data-ttu-id="c84f5-150">Если необязательный `address` параметр не указан, эта функция возвращает весь диапазон листа.</span><span class="sxs-lookup"><span data-stu-id="c84f5-150">If the optional `address` parameter is not specified, this function returns the entire worksheet range.</span></span>

##### <a name="request"></a><span data-ttu-id="c84f5-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="c84f5-151">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c84f5-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="c84f5-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "worksheet_range_noaddress"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/range
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c84f5-153">C#</span><span class="sxs-lookup"><span data-stu-id="c84f5-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheet-range-noaddress-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c84f5-154">Javascript</span><span class="sxs-lookup"><span data-stu-id="c84f5-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheet-range-noaddress-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c84f5-155">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c84f5-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheet-range-noaddress-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c84f5-156">Java</span><span class="sxs-lookup"><span data-stu-id="c84f5-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheet-range-noaddress-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c84f5-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="c84f5-157">Response</span></span>

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
