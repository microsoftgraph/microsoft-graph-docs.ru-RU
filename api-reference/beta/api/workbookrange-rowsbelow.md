---
title: 'workbookRange: rowsBelow'
description: Возвращает определенное количество строк под заданным диапазоном.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: d7e1e6b76640601b29bca217be6c5b978223462e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053316"
---
# <a name="workbookrange-rowsbelow"></a><span data-ttu-id="203e9-103">workbookRange: rowsBelow</span><span class="sxs-lookup"><span data-stu-id="203e9-103">workbookRange: rowsBelow</span></span>

<span data-ttu-id="203e9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="203e9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="203e9-105">Возвращает определенное количество строк под заданным диапазоном.</span><span class="sxs-lookup"><span data-stu-id="203e9-105">Gets certain number of rows below a given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="203e9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="203e9-106">Permissions</span></span>
<span data-ttu-id="203e9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="203e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="203e9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="203e9-109">Permission type</span></span>      | <span data-ttu-id="203e9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="203e9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="203e9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="203e9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="203e9-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="203e9-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="203e9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="203e9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="203e9-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="203e9-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="203e9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="203e9-115">Application</span></span> | <span data-ttu-id="203e9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="203e9-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="203e9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="203e9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id}/range/rowsBelow(count=n)
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id}/range/rowsBelow(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="203e9-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="203e9-118">Function parameters</span></span>

| <span data-ttu-id="203e9-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="203e9-119">Parameter</span></span>    | <span data-ttu-id="203e9-120">Тип</span><span class="sxs-lookup"><span data-stu-id="203e9-120">Type</span></span>   |<span data-ttu-id="203e9-121">Описание</span><span class="sxs-lookup"><span data-stu-id="203e9-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="203e9-122">count</span><span class="sxs-lookup"><span data-stu-id="203e9-122">count</span></span>|<span data-ttu-id="203e9-123">Int32</span><span class="sxs-lookup"><span data-stu-id="203e9-123">Int32</span></span>|<span data-ttu-id="203e9-p102">Необязательный. Количество строк, включаемых в полученный диапазон. Чтобы создать диапазон за пределами текущего диапазона, используйте положительное число. Вы также можете использовать отрицательное число, чтобы создать диапазон в рамках текущего диапазона. Значение по умолчанию — 1.</span><span class="sxs-lookup"><span data-stu-id="203e9-p102">Optional. The number of rows to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="203e9-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="203e9-129">Request headers</span></span>
| <span data-ttu-id="203e9-130">Имя</span><span class="sxs-lookup"><span data-stu-id="203e9-130">Name</span></span>       | <span data-ttu-id="203e9-131">Описание</span><span class="sxs-lookup"><span data-stu-id="203e9-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="203e9-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="203e9-132">Authorization</span></span>  | <span data-ttu-id="203e9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="203e9-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="203e9-135">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="203e9-135">Workbook-Session-Id</span></span>  | <span data-ttu-id="203e9-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="203e9-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="203e9-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="203e9-138">Request body</span></span>
<span data-ttu-id="203e9-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="203e9-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="203e9-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="203e9-140">Response</span></span>

<span data-ttu-id="203e9-141">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/workbookrange.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="203e9-141">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="203e9-142">Пример</span><span class="sxs-lookup"><span data-stu-id="203e9-142">Example</span></span>
<span data-ttu-id="203e9-143">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="203e9-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="203e9-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="203e9-144">Request</span></span>
<span data-ttu-id="203e9-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="203e9-145">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="203e9-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="203e9-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookrange_rowsBelow"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=2)
```
# <a name="c"></a>[<span data-ttu-id="203e9-147">C#</span><span class="sxs-lookup"><span data-stu-id="203e9-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrange-rowsbelow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="203e9-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="203e9-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrange-rowsbelow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="203e9-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="203e9-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrange-rowsbelow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="203e9-150">Java</span><span class="sxs-lookup"><span data-stu-id="203e9-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrange-rowsbelow-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="203e9-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="203e9-151">Response</span></span>
<span data-ttu-id="203e9-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="203e9-152">Here is an example of the response.</span></span> <span data-ttu-id="203e9-153">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="203e9-153">Note: The response object shown here might be shortened for readability.</span></span>
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


