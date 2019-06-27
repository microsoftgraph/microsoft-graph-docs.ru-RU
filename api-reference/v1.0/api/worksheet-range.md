---
title: 'Worksheet: Range'
description: Возвращает объект диапазона, указанный по адресу или имени.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: a5e1d2ba70e5cdb5ca1e38e4baba0ddf9977fc9c
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35278311"
---
# <a name="worksheet-range"></a><span data-ttu-id="b6066-103">Worksheet: Range</span><span class="sxs-lookup"><span data-stu-id="b6066-103">Worksheet: Range</span></span>

<span data-ttu-id="b6066-104">Возвращает объект диапазона, указанный по адресу или имени.</span><span class="sxs-lookup"><span data-stu-id="b6066-104">Gets the range object specified by the address or name.</span></span>
## <a name="permissions"></a><span data-ttu-id="b6066-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b6066-105">Permissions</span></span>
<span data-ttu-id="b6066-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6066-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6066-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b6066-108">Permission type</span></span>      | <span data-ttu-id="b6066-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b6066-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b6066-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b6066-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b6066-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b6066-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b6066-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b6066-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6066-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6066-113">Not supported.</span></span>    |
|<span data-ttu-id="b6066-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b6066-114">Application</span></span> | <span data-ttu-id="b6066-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6066-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b6066-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b6066-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/range

```
## <a name="request-headers"></a><span data-ttu-id="b6066-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b6066-117">Request headers</span></span>
| <span data-ttu-id="b6066-118">Имя</span><span class="sxs-lookup"><span data-stu-id="b6066-118">Name</span></span>       | <span data-ttu-id="b6066-119">Описание</span><span class="sxs-lookup"><span data-stu-id="b6066-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b6066-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b6066-120">Authorization</span></span>  | <span data-ttu-id="b6066-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b6066-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b6066-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b6066-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="b6066-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="b6066-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="function-parameters"></a><span data-ttu-id="b6066-126">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="b6066-126">Function parameters</span></span>

| <span data-ttu-id="b6066-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="b6066-127">Parameter</span></span>    | <span data-ttu-id="b6066-128">Тип</span><span class="sxs-lookup"><span data-stu-id="b6066-128">Type</span></span>   |<span data-ttu-id="b6066-129">Описание</span><span class="sxs-lookup"><span data-stu-id="b6066-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b6066-130">address</span><span class="sxs-lookup"><span data-stu-id="b6066-130">address</span></span>|<span data-ttu-id="b6066-131">string</span><span class="sxs-lookup"><span data-stu-id="b6066-131">string</span></span>|<span data-ttu-id="b6066-p104">Необязательный параметр. Адрес или имя диапазона. Если аргумент не указан, возвращается весь диапазон листа.</span><span class="sxs-lookup"><span data-stu-id="b6066-p104">Optional. The address or the name of the range. If not specified, the entire worksheet range is returned.</span></span>|

## <a name="response"></a><span data-ttu-id="b6066-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6066-135">Response</span></span>

<span data-ttu-id="b6066-136">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b6066-136">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6066-137">Пример</span><span class="sxs-lookup"><span data-stu-id="b6066-137">Example</span></span>
<span data-ttu-id="b6066-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="b6066-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b6066-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="b6066-139">Request</span></span>
<span data-ttu-id="b6066-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b6066-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_range"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='A1:B2')
```

##### <a name="response"></a><span data-ttu-id="b6066-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="b6066-141">Response</span></span>
<span data-ttu-id="b6066-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b6066-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="b6066-145">Образец кода SDK</span><span class="sxs-lookup"><span data-stu-id="b6066-145">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b6066-146">C#</span><span class="sxs-lookup"><span data-stu-id="b6066-146">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/worksheet_range-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b6066-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="b6066-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/worksheet_range-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="b6066-148">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b6066-148">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/worksheet_range-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="b6066-149">Если необязательный `address` параметр не указан, эта функция возвращает весь диапазон листа.</span><span class="sxs-lookup"><span data-stu-id="b6066-149">If the optional `address` parameter is not specified, this function returns the entire worksheet range.</span></span>

##### <a name="request"></a><span data-ttu-id="b6066-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="b6066-150">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "worksheet_range_noaddress"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/range
```

##### <a name="response"></a><span data-ttu-id="b6066-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6066-151">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="b6066-152">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="b6066-152">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b6066-153">C#</span><span class="sxs-lookup"><span data-stu-id="b6066-153">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/worksheet_range_noaddress-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b6066-154">Javascript</span><span class="sxs-lookup"><span data-stu-id="b6066-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/worksheet_range_noaddress-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="b6066-155">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b6066-155">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/worksheet_range_noaddress-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/worksheet-range.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/worksheet-range.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/worksheet-range.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/worksheet-range.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/worksheet-range.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
