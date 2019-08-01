---
title: 'workbookRange: rowsAbove'
description: Возвращает определенное количество строк над заданным диапазоном.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 4ab586ac1a3a876984c3118ec2c956ccf4ea9fa2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36026350"
---
# <a name="workbookrange-rowsabove"></a><span data-ttu-id="99d00-103">workbookRange: rowsAbove</span><span class="sxs-lookup"><span data-stu-id="99d00-103">workbookRange: rowsAbove</span></span>

<span data-ttu-id="99d00-104">Возвращает определенное количество строк над заданным диапазоном.</span><span class="sxs-lookup"><span data-stu-id="99d00-104">Gets a certain number of rows above a given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="99d00-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="99d00-105">Permissions</span></span>
<span data-ttu-id="99d00-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99d00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99d00-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="99d00-108">Permission type</span></span>      | <span data-ttu-id="99d00-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="99d00-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99d00-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="99d00-110">Delegated (work or school account)</span></span> | <span data-ttu-id="99d00-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="99d00-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="99d00-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="99d00-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99d00-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99d00-113">Not supported.</span></span>    |
|<span data-ttu-id="99d00-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="99d00-114">Application</span></span> | <span data-ttu-id="99d00-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99d00-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="99d00-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="99d00-116">HTTP request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="99d00-117">HTTP</span><span class="sxs-lookup"><span data-stu-id="99d00-117">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/rowsAbove(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="99d00-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="99d00-118">Function parameters</span></span>

| <span data-ttu-id="99d00-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="99d00-119">Parameter</span></span>    | <span data-ttu-id="99d00-120">Тип</span><span class="sxs-lookup"><span data-stu-id="99d00-120">Type</span></span>   |<span data-ttu-id="99d00-121">Описание</span><span class="sxs-lookup"><span data-stu-id="99d00-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="99d00-122">count</span><span class="sxs-lookup"><span data-stu-id="99d00-122">count</span></span>|<span data-ttu-id="99d00-123">Int32</span><span class="sxs-lookup"><span data-stu-id="99d00-123">Int32</span></span>|<span data-ttu-id="99d00-p102">Необязательный. Количество строк, включаемых в полученный диапазон. Чтобы создать диапазон за пределами текущего диапазона, используйте положительное число. Вы также можете использовать отрицательное число, чтобы создать диапазон в рамках текущего диапазона. Значение по умолчанию — 1.</span><span class="sxs-lookup"><span data-stu-id="99d00-p102">Optional. The number of rows to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="99d00-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="99d00-129">Request headers</span></span>
| <span data-ttu-id="99d00-130">Имя</span><span class="sxs-lookup"><span data-stu-id="99d00-130">Name</span></span>       | <span data-ttu-id="99d00-131">Описание</span><span class="sxs-lookup"><span data-stu-id="99d00-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="99d00-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="99d00-132">Authorization</span></span>  | <span data-ttu-id="99d00-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="99d00-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="99d00-135">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="99d00-135">Workbook-Session-Id</span></span>  | <span data-ttu-id="99d00-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="99d00-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="99d00-138">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="99d00-138">Request body</span></span>
<span data-ttu-id="99d00-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="99d00-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="99d00-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="99d00-140">Response</span></span>
<span data-ttu-id="99d00-141">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="99d00-141">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99d00-142">Пример</span><span class="sxs-lookup"><span data-stu-id="99d00-142">Example</span></span>
<span data-ttu-id="99d00-143">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="99d00-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="99d00-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="99d00-144">Request</span></span>
<span data-ttu-id="99d00-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="99d00-145">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsAbove",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsAbove(count=2)
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="99d00-146">C#</span><span class="sxs-lookup"><span data-stu-id="99d00-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrange-rowsabove-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="99d00-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="99d00-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrange-rowsabove-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="99d00-148">Цель — C</span><span class="sxs-lookup"><span data-stu-id="99d00-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrange-rowsabove-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="99d00-149">Java</span><span class="sxs-lookup"><span data-stu-id="99d00-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrange-rowsabove-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="99d00-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="99d00-150">Response</span></span>
<span data-ttu-id="99d00-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="99d00-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="99d00-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="99d00-154">HTTP</span></span>](#tab/http)
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

<span data-ttu-id="99d00-155">При вызове без обязательного `count` параметра эта функция возвращает одну строку над диапазоном.</span><span class="sxs-lookup"><span data-stu-id="99d00-155">If called without the optional `count` parameter, this function returns the single row above the range.</span></span>

##### <a name="request"></a><span data-ttu-id="99d00-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="99d00-156">Request</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsAbove_nocount",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsAbove
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="99d00-157">C#</span><span class="sxs-lookup"><span data-stu-id="99d00-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrange-rowsabove-nocount-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="99d00-158">Javascript</span><span class="sxs-lookup"><span data-stu-id="99d00-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrange-rowsabove-nocount-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="99d00-159">Цель — C</span><span class="sxs-lookup"><span data-stu-id="99d00-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrange-rowsabove-nocount-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="99d00-160">Java</span><span class="sxs-lookup"><span data-stu-id="99d00-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrange-rowsabove-nocount-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="99d00-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="99d00-161">Response</span></span>
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
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
