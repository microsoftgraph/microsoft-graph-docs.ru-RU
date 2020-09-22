---
title: 'workbookRange: rowsBelow'
description: Возвращает определенное количество строк под заданным диапазоном.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: c013e2889e03d73010dcf6ca67ee0e4ba422f6a6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091910"
---
# <a name="workbookrange-rowsbelow"></a><span data-ttu-id="834bc-103">workbookRange: rowsBelow</span><span class="sxs-lookup"><span data-stu-id="834bc-103">workbookRange: rowsBelow</span></span>

<span data-ttu-id="834bc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="834bc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="834bc-105">Возвращает определенное количество строк под заданным диапазоном.</span><span class="sxs-lookup"><span data-stu-id="834bc-105">Gets certain number of rows below a given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="834bc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="834bc-106">Permissions</span></span>
<span data-ttu-id="834bc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="834bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="834bc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="834bc-109">Permission type</span></span>      | <span data-ttu-id="834bc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="834bc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="834bc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="834bc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="834bc-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="834bc-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="834bc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="834bc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="834bc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="834bc-114">Not supported.</span></span>    |
|<span data-ttu-id="834bc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="834bc-115">Application</span></span> | <span data-ttu-id="834bc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="834bc-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="834bc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="834bc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="834bc-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="834bc-118">Function parameters</span></span>

| <span data-ttu-id="834bc-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="834bc-119">Parameter</span></span>    | <span data-ttu-id="834bc-120">Тип</span><span class="sxs-lookup"><span data-stu-id="834bc-120">Type</span></span>   |<span data-ttu-id="834bc-121">Описание</span><span class="sxs-lookup"><span data-stu-id="834bc-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="834bc-122">count</span><span class="sxs-lookup"><span data-stu-id="834bc-122">count</span></span>|<span data-ttu-id="834bc-123">Int32</span><span class="sxs-lookup"><span data-stu-id="834bc-123">Int32</span></span>| <span data-ttu-id="834bc-p102">Необязательный. Количество строк, включаемых в полученный диапазон. Чтобы создать диапазон за пределами текущего диапазона, используйте положительное число. Вы также можете использовать отрицательное число, чтобы создать диапазон в рамках текущего диапазона. Значение по умолчанию — 1.</span><span class="sxs-lookup"><span data-stu-id="834bc-p102">Optional. The number of rows to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="834bc-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="834bc-129">Request headers</span></span>
| <span data-ttu-id="834bc-130">Имя</span><span class="sxs-lookup"><span data-stu-id="834bc-130">Name</span></span>       | <span data-ttu-id="834bc-131">Описание</span><span class="sxs-lookup"><span data-stu-id="834bc-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="834bc-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="834bc-132">Authorization</span></span>  | <span data-ttu-id="834bc-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="834bc-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="834bc-135">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="834bc-135">Workbook-Session-Id</span></span>  | <span data-ttu-id="834bc-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="834bc-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="834bc-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="834bc-138">Request body</span></span>
<span data-ttu-id="834bc-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="834bc-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="834bc-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="834bc-140">Response</span></span>
<span data-ttu-id="834bc-141">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="834bc-141">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="834bc-142">Пример</span><span class="sxs-lookup"><span data-stu-id="834bc-142">Example</span></span>
<span data-ttu-id="834bc-143">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="834bc-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="834bc-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="834bc-144">Request</span></span>
<span data-ttu-id="834bc-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="834bc-145">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="834bc-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="834bc-146">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsBelow",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=2)
```
# <a name="c"></a>[<span data-ttu-id="834bc-147">C#</span><span class="sxs-lookup"><span data-stu-id="834bc-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrange-rowsbelow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="834bc-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="834bc-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrange-rowsbelow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="834bc-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="834bc-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrange-rowsbelow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="834bc-150">Java</span><span class="sxs-lookup"><span data-stu-id="834bc-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrange-rowsbelow-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="834bc-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="834bc-151">Response</span></span>
<span data-ttu-id="834bc-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="834bc-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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

<span data-ttu-id="834bc-155">При вызове без `count` параметра эта функция принимает значение по умолчанию, равное одной строке.</span><span class="sxs-lookup"><span data-stu-id="834bc-155">If called without the `count` parameter, this function defaults to one row.</span></span>

##### <a name="request"></a><span data-ttu-id="834bc-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="834bc-156">Request</span></span>
<span data-ttu-id="834bc-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="834bc-157">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="834bc-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="834bc-158">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsBelow_nocount",
  "idempotent": true
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsBelow
```
# <a name="c"></a>[<span data-ttu-id="834bc-159">C#</span><span class="sxs-lookup"><span data-stu-id="834bc-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrange-rowsbelow-nocount-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="834bc-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="834bc-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrange-rowsbelow-nocount-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="834bc-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="834bc-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrange-rowsbelow-nocount-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="834bc-162">Java</span><span class="sxs-lookup"><span data-stu-id="834bc-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrange-rowsbelow-nocount-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="834bc-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="834bc-163">Response</span></span>
<span data-ttu-id="834bc-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="834bc-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

