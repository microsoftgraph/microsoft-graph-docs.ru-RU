---
title: 'workbookRange: rowsBelow'
description: Возвращает определенное количество строк под заданным диапазоном.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 714743d68d31439afaa8aa648dfdf0f305f758ae
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50575504"
---
# <a name="workbookrange-rowsbelow"></a><span data-ttu-id="8ada4-103">workbookRange: rowsBelow</span><span class="sxs-lookup"><span data-stu-id="8ada4-103">workbookRange: rowsBelow</span></span>

<span data-ttu-id="8ada4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ada4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8ada4-105">Возвращает определенное количество строк под заданным диапазоном.</span><span class="sxs-lookup"><span data-stu-id="8ada4-105">Gets certain number of rows below a given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="8ada4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8ada4-106">Permissions</span></span>
<span data-ttu-id="8ada4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ada4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ada4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8ada4-109">Permission type</span></span>      | <span data-ttu-id="8ada4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8ada4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8ada4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8ada4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8ada4-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8ada4-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8ada4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8ada4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ada4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ada4-114">Not supported.</span></span>    |
|<span data-ttu-id="8ada4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8ada4-115">Application</span></span> | <span data-ttu-id="8ada4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ada4-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ada4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8ada4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id}/range/rowsBelow(count=n)
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id}/range/rowsBelow(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="8ada4-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="8ada4-118">Function parameters</span></span>

| <span data-ttu-id="8ada4-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="8ada4-119">Parameter</span></span>    | <span data-ttu-id="8ada4-120">Тип</span><span class="sxs-lookup"><span data-stu-id="8ada4-120">Type</span></span>   |<span data-ttu-id="8ada4-121">Описание</span><span class="sxs-lookup"><span data-stu-id="8ada4-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8ada4-122">count</span><span class="sxs-lookup"><span data-stu-id="8ada4-122">count</span></span>|<span data-ttu-id="8ada4-123">Int32</span><span class="sxs-lookup"><span data-stu-id="8ada4-123">Int32</span></span>| <span data-ttu-id="8ada4-p102">Необязательный. Количество строк, включаемых в полученный диапазон. Чтобы создать диапазон за пределами текущего диапазона, используйте положительное число. Вы также можете использовать отрицательное число, чтобы создать диапазон в рамках текущего диапазона. Значение по умолчанию — 1.</span><span class="sxs-lookup"><span data-stu-id="8ada4-p102">Optional. The number of rows to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="8ada4-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8ada4-129">Request headers</span></span>
| <span data-ttu-id="8ada4-130">Имя</span><span class="sxs-lookup"><span data-stu-id="8ada4-130">Name</span></span>       | <span data-ttu-id="8ada4-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8ada4-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8ada4-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8ada4-132">Authorization</span></span>  | <span data-ttu-id="8ada4-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8ada4-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8ada4-135">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8ada4-135">Workbook-Session-Id</span></span>  | <span data-ttu-id="8ada4-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="8ada4-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ada4-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8ada4-138">Request body</span></span>
<span data-ttu-id="8ada4-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8ada4-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ada4-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ada4-140">Response</span></span>
<span data-ttu-id="8ada4-141">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8ada4-141">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ada4-142">Пример</span><span class="sxs-lookup"><span data-stu-id="8ada4-142">Example</span></span>
<span data-ttu-id="8ada4-143">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="8ada4-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8ada4-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="8ada4-144">Request</span></span>
<span data-ttu-id="8ada4-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8ada4-145">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8ada4-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="8ada4-146">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsBelow",
  "idempotent": true
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=2)
```
# <a name="c"></a>[<span data-ttu-id="8ada4-147">C#</span><span class="sxs-lookup"><span data-stu-id="8ada4-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrange-rowsbelow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8ada4-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8ada4-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrange-rowsbelow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8ada4-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8ada4-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrange-rowsbelow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8ada4-150">Java</span><span class="sxs-lookup"><span data-stu-id="8ada4-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrange-rowsbelow-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8ada4-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ada4-151">Response</span></span>
<span data-ttu-id="8ada4-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8ada4-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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

<span data-ttu-id="8ada4-155">Если она вызвана без `count` параметра, эта функция по умолчанию передается в одну строку.</span><span class="sxs-lookup"><span data-stu-id="8ada4-155">If called without the `count` parameter, this function defaults to one row.</span></span>

##### <a name="request"></a><span data-ttu-id="8ada4-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="8ada4-156">Request</span></span>
<span data-ttu-id="8ada4-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8ada4-157">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8ada4-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="8ada4-158">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsBelow_nocount",
  "idempotent": true
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsBelow
```
# <a name="c"></a>[<span data-ttu-id="8ada4-159">C#</span><span class="sxs-lookup"><span data-stu-id="8ada4-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrange-rowsbelow-nocount-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8ada4-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8ada4-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrange-rowsbelow-nocount-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8ada4-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8ada4-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrange-rowsbelow-nocount-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8ada4-162">Java</span><span class="sxs-lookup"><span data-stu-id="8ada4-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrange-rowsbelow-nocount-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8ada4-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ada4-163">Response</span></span>
<span data-ttu-id="8ada4-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8ada4-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

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

