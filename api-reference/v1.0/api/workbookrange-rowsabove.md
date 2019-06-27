---
title: 'workbookRange: rowsAbove'
description: Возвращает определенное количество строк над заданным диапазоном.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: c52172980d84cf53c893a1466913730aa892f64d
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35278486"
---
# <a name="workbookrange-rowsabove"></a><span data-ttu-id="caaa4-103">workbookRange: rowsAbove</span><span class="sxs-lookup"><span data-stu-id="caaa4-103">workbookRange: rowsAbove</span></span>

<span data-ttu-id="caaa4-104">Возвращает определенное количество строк над заданным диапазоном.</span><span class="sxs-lookup"><span data-stu-id="caaa4-104">Gets a certain number of rows above a given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="caaa4-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="caaa4-105">Permissions</span></span>
<span data-ttu-id="caaa4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="caaa4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="caaa4-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="caaa4-108">Permission type</span></span>      | <span data-ttu-id="caaa4-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="caaa4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="caaa4-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="caaa4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="caaa4-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="caaa4-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="caaa4-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="caaa4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="caaa4-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="caaa4-113">Not supported.</span></span>    |
|<span data-ttu-id="caaa4-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="caaa4-114">Application</span></span> | <span data-ttu-id="caaa4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="caaa4-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="caaa4-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="caaa4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/rowsAbove(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="caaa4-117">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="caaa4-117">Function parameters</span></span>

| <span data-ttu-id="caaa4-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="caaa4-118">Parameter</span></span>    | <span data-ttu-id="caaa4-119">Тип</span><span class="sxs-lookup"><span data-stu-id="caaa4-119">Type</span></span>   |<span data-ttu-id="caaa4-120">Описание</span><span class="sxs-lookup"><span data-stu-id="caaa4-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="caaa4-121">count</span><span class="sxs-lookup"><span data-stu-id="caaa4-121">count</span></span>|<span data-ttu-id="caaa4-122">Int32</span><span class="sxs-lookup"><span data-stu-id="caaa4-122">Int32</span></span>|<span data-ttu-id="caaa4-p102">Необязательный. Количество строк, включаемых в полученный диапазон. Чтобы создать диапазон за пределами текущего диапазона, используйте положительное число. Вы также можете использовать отрицательное число, чтобы создать диапазон в рамках текущего диапазона. Значение по умолчанию — 1.</span><span class="sxs-lookup"><span data-stu-id="caaa4-p102">Optional. The number of rows to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="caaa4-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="caaa4-128">Request headers</span></span>
| <span data-ttu-id="caaa4-129">Имя</span><span class="sxs-lookup"><span data-stu-id="caaa4-129">Name</span></span>       | <span data-ttu-id="caaa4-130">Описание</span><span class="sxs-lookup"><span data-stu-id="caaa4-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="caaa4-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="caaa4-131">Authorization</span></span>  | <span data-ttu-id="caaa4-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="caaa4-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="caaa4-134">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="caaa4-134">Workbook-Session-Id</span></span>  | <span data-ttu-id="caaa4-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="caaa4-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="caaa4-137">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="caaa4-137">Request body</span></span>
<span data-ttu-id="caaa4-138">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="caaa4-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="caaa4-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="caaa4-139">Response</span></span>
<span data-ttu-id="caaa4-140">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="caaa4-140">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="caaa4-141">Пример</span><span class="sxs-lookup"><span data-stu-id="caaa4-141">Example</span></span>
<span data-ttu-id="caaa4-142">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="caaa4-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="caaa4-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="caaa4-143">Request</span></span>
<span data-ttu-id="caaa4-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="caaa4-144">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsAbove",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsAbove(count=2)
```

##### <a name="response"></a><span data-ttu-id="caaa4-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="caaa4-145">Response</span></span>
<span data-ttu-id="caaa4-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="caaa4-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 157

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnHidden": true,
  "columnIndex": 99
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="caaa4-149">Образец кода SDK</span><span class="sxs-lookup"><span data-stu-id="caaa4-149">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="caaa4-150">C#</span><span class="sxs-lookup"><span data-stu-id="caaa4-150">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/workbookrange_rowsAbove-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="caaa4-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="caaa4-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/workbookrange_rowsAbove-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="caaa4-152">Цель — C</span><span class="sxs-lookup"><span data-stu-id="caaa4-152">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/workbookrange_rowsAbove-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="caaa4-153">При вызове без обязательного `count` параметра эта функция возвращает одну строку над диапазоном.</span><span class="sxs-lookup"><span data-stu-id="caaa4-153">If called without the optional `count` parameter, this function returns the single row above the range.</span></span>

##### <a name="request"></a><span data-ttu-id="caaa4-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="caaa4-154">Request</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsAbove_nocount",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsAbove
```

##### <a name="response"></a><span data-ttu-id="caaa4-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="caaa4-155">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 157

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnHidden": true,
  "columnIndex": 99
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="caaa4-156">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="caaa4-156">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="caaa4-157">C#</span><span class="sxs-lookup"><span data-stu-id="caaa4-157">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/workbookrange_rowsAbove_nocount-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="caaa4-158">Javascript</span><span class="sxs-lookup"><span data-stu-id="caaa4-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/workbookrange_rowsAbove_nocount-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="caaa4-159">Цель — C</span><span class="sxs-lookup"><span data-stu-id="caaa4-159">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/workbookrange_rowsAbove_nocount-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/workbookrange-rowsabove.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/workbookrange-rowsabove.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/workbookrange-rowsabove.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/workbookrange-rowsabove.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/workbookrange-rowsabove.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
