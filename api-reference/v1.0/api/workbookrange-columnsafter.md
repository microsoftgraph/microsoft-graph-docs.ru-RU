---
title: 'workbookRange: columnsAfter'
description: Возвращает определенное количество столбцов справа от заданного диапазона.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 53bde7340a2f893cb9d473c37f0eb887a4affdcb
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055668"
---
# <a name="workbookrange-columnsafter"></a><span data-ttu-id="3aea5-103">workbookRange: columnsAfter</span><span class="sxs-lookup"><span data-stu-id="3aea5-103">workbookRange: columnsAfter</span></span>

<span data-ttu-id="3aea5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3aea5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3aea5-105">Возвращает определенное количество столбцов справа от заданного диапазона.</span><span class="sxs-lookup"><span data-stu-id="3aea5-105">Gets a certain number of columns to the right of the given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="3aea5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3aea5-106">Permissions</span></span>
<span data-ttu-id="3aea5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3aea5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3aea5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3aea5-109">Permission type</span></span>      | <span data-ttu-id="3aea5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3aea5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3aea5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3aea5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3aea5-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3aea5-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3aea5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3aea5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3aea5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3aea5-114">Not supported.</span></span>    |
|<span data-ttu-id="3aea5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3aea5-115">Application</span></span> | <span data-ttu-id="3aea5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3aea5-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3aea5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3aea5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id}/range/columnsAfter(count=n)
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id}/range/columnsAfter(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="3aea5-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="3aea5-118">Function parameters</span></span>

| <span data-ttu-id="3aea5-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="3aea5-119">Parameter</span></span>    | <span data-ttu-id="3aea5-120">Тип</span><span class="sxs-lookup"><span data-stu-id="3aea5-120">Type</span></span>   |<span data-ttu-id="3aea5-121">Описание</span><span class="sxs-lookup"><span data-stu-id="3aea5-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3aea5-122">count</span><span class="sxs-lookup"><span data-stu-id="3aea5-122">count</span></span>|<span data-ttu-id="3aea5-123">Int32</span><span class="sxs-lookup"><span data-stu-id="3aea5-123">Int32</span></span>|<span data-ttu-id="3aea5-124">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="3aea5-124">Optional.</span></span> <span data-ttu-id="3aea5-125">Количество столбцов, включаемых в полученный диапазон.</span><span class="sxs-lookup"><span data-stu-id="3aea5-125">The number of columns to include in the resulting range.</span></span> <span data-ttu-id="3aea5-126">Чтобы создать диапазон за пределами текущего диапазона, используйте положительное число.</span><span class="sxs-lookup"><span data-stu-id="3aea5-126">In general, use a positive number to create a range outside the current range.</span></span> <span data-ttu-id="3aea5-127">Вы также можете указать отрицательное число, чтобы создать диапазон в рамках текущего диапазона.</span><span class="sxs-lookup"><span data-stu-id="3aea5-127">You can also use a negative number to create a range within the current range.</span></span> <span data-ttu-id="3aea5-128">По умолчанию используется значение 1.</span><span class="sxs-lookup"><span data-stu-id="3aea5-128">The default value is 1</span></span>|

## <a name="request-headers"></a><span data-ttu-id="3aea5-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3aea5-129">Request headers</span></span>
| <span data-ttu-id="3aea5-130">Имя</span><span class="sxs-lookup"><span data-stu-id="3aea5-130">Name</span></span>       | <span data-ttu-id="3aea5-131">Описание</span><span class="sxs-lookup"><span data-stu-id="3aea5-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3aea5-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3aea5-132">Authorization</span></span>  | <span data-ttu-id="3aea5-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3aea5-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3aea5-135">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3aea5-135">Workbook-Session-Id</span></span>  | <span data-ttu-id="3aea5-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="3aea5-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3aea5-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3aea5-138">Request body</span></span>
<span data-ttu-id="3aea5-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3aea5-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3aea5-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="3aea5-140">Response</span></span>
<span data-ttu-id="3aea5-141">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3aea5-141">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3aea5-142">Пример</span><span class="sxs-lookup"><span data-stu-id="3aea5-142">Example</span></span>
<span data-ttu-id="3aea5-143">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="3aea5-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3aea5-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="3aea5-144">Request</span></span>
<span data-ttu-id="3aea5-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3aea5-145">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3aea5-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="3aea5-146">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_columnsafter",
  "idempotent": true
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=2)
```
# <a name="c"></a>[<span data-ttu-id="3aea5-147">C#</span><span class="sxs-lookup"><span data-stu-id="3aea5-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrange-columnsafter-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3aea5-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3aea5-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrange-columnsafter-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3aea5-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3aea5-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrange-columnsafter-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3aea5-150">Java</span><span class="sxs-lookup"><span data-stu-id="3aea5-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrange-columnsafter-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3aea5-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="3aea5-151">Response</span></span>
<span data-ttu-id="3aea5-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3aea5-152">Here is an example of the response.</span></span> <span data-ttu-id="3aea5-153">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3aea5-153">Note: The response object shown here might be shortened for readability.</span></span>
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

