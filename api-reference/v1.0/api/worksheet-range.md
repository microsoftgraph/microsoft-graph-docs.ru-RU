---
title: 'Worksheet: Range'
description: Возвращает объект диапазона, указанный по адресу или имени.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 7fcc975891dca549f52cc8611107ef94655e6032
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094549"
---
# <a name="worksheet-range"></a><span data-ttu-id="0b5a3-103">Worksheet: Range</span><span class="sxs-lookup"><span data-stu-id="0b5a3-103">Worksheet: Range</span></span>

<span data-ttu-id="0b5a3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b5a3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0b5a3-105">Возвращает объект диапазона, указанный по адресу или имени.</span><span class="sxs-lookup"><span data-stu-id="0b5a3-105">Gets the range object specified by the address or name.</span></span>
## <a name="permissions"></a><span data-ttu-id="0b5a3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0b5a3-106">Permissions</span></span>
<span data-ttu-id="0b5a3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b5a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b5a3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0b5a3-109">Permission type</span></span>      | <span data-ttu-id="0b5a3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0b5a3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b5a3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0b5a3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0b5a3-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0b5a3-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0b5a3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0b5a3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b5a3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b5a3-114">Not supported.</span></span>    |
|<span data-ttu-id="0b5a3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0b5a3-115">Application</span></span> | <span data-ttu-id="0b5a3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b5a3-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0b5a3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0b5a3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/range

```
## <a name="request-headers"></a><span data-ttu-id="0b5a3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0b5a3-118">Request headers</span></span>
| <span data-ttu-id="0b5a3-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0b5a3-119">Name</span></span>       | <span data-ttu-id="0b5a3-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0b5a3-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0b5a3-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0b5a3-121">Authorization</span></span>  | <span data-ttu-id="0b5a3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0b5a3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0b5a3-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0b5a3-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="0b5a3-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="0b5a3-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="function-parameters"></a><span data-ttu-id="0b5a3-127">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="0b5a3-127">Function parameters</span></span>

| <span data-ttu-id="0b5a3-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="0b5a3-128">Parameter</span></span>    | <span data-ttu-id="0b5a3-129">Тип</span><span class="sxs-lookup"><span data-stu-id="0b5a3-129">Type</span></span>   |<span data-ttu-id="0b5a3-130">Описание</span><span class="sxs-lookup"><span data-stu-id="0b5a3-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b5a3-131">address</span><span class="sxs-lookup"><span data-stu-id="0b5a3-131">address</span></span>|<span data-ttu-id="0b5a3-132">string</span><span class="sxs-lookup"><span data-stu-id="0b5a3-132">string</span></span>|<span data-ttu-id="0b5a3-p104">Необязательный параметр. Адрес или имя диапазона. Если аргумент не указан, возвращается весь диапазон листа.</span><span class="sxs-lookup"><span data-stu-id="0b5a3-p104">Optional. The address or the name of the range. If not specified, the entire worksheet range is returned.</span></span>|

## <a name="response"></a><span data-ttu-id="0b5a3-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b5a3-136">Response</span></span>

<span data-ttu-id="0b5a3-137">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0b5a3-137">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b5a3-138">Пример</span><span class="sxs-lookup"><span data-stu-id="0b5a3-138">Example</span></span>
<span data-ttu-id="0b5a3-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="0b5a3-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0b5a3-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="0b5a3-140">Request</span></span>
<span data-ttu-id="0b5a3-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0b5a3-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0b5a3-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b5a3-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "worksheet_range"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='A1:B2')
```
# <a name="c"></a>[<span data-ttu-id="0b5a3-143">C#</span><span class="sxs-lookup"><span data-stu-id="0b5a3-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheet-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0b5a3-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b5a3-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheet-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0b5a3-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b5a3-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheet-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0b5a3-146">Java</span><span class="sxs-lookup"><span data-stu-id="0b5a3-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheet-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0b5a3-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b5a3-147">Response</span></span>
<span data-ttu-id="0b5a3-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0b5a3-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<span data-ttu-id="0b5a3-151">Если необязательный `address` параметр не указан, эта функция возвращает весь диапазон листа.</span><span class="sxs-lookup"><span data-stu-id="0b5a3-151">If the optional `address` parameter is not specified, this function returns the entire worksheet range.</span></span>

##### <a name="request"></a><span data-ttu-id="0b5a3-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="0b5a3-152">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="0b5a3-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b5a3-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "worksheet_range_noaddress"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/range
```
# <a name="c"></a>[<span data-ttu-id="0b5a3-154">C#</span><span class="sxs-lookup"><span data-stu-id="0b5a3-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheet-range-noaddress-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0b5a3-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b5a3-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheet-range-noaddress-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0b5a3-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b5a3-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheet-range-noaddress-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0b5a3-157">Java</span><span class="sxs-lookup"><span data-stu-id="0b5a3-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheet-range-noaddress-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0b5a3-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b5a3-158">Response</span></span>

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

