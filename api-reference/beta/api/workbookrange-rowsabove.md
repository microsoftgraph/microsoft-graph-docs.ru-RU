---
title: 'workbookRange: rowsAbove'
description: Возвращает определенное количество строк над заданным диапазоном.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 508994ff0d5e71368d6f6aed04d2718d941bb5df
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/16/2021
ms.locfileid: "49882985"
---
# <a name="workbookrange-rowsabove"></a><span data-ttu-id="e4cfe-103">workbookRange: rowsAbove</span><span class="sxs-lookup"><span data-stu-id="e4cfe-103">workbookRange: rowsAbove</span></span>

<span data-ttu-id="e4cfe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4cfe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4cfe-105">Возвращает определенное количество строк над заданным диапазоном.</span><span class="sxs-lookup"><span data-stu-id="e4cfe-105">Gets a certain number of rows above a given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="e4cfe-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e4cfe-106">Permissions</span></span>
<span data-ttu-id="e4cfe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4cfe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4cfe-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e4cfe-109">Permission type</span></span>      | <span data-ttu-id="e4cfe-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e4cfe-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4cfe-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e4cfe-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e4cfe-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e4cfe-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e4cfe-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e4cfe-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4cfe-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e4cfe-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e4cfe-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e4cfe-115">Application</span></span> | <span data-ttu-id="e4cfe-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4cfe-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e4cfe-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e4cfe-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/workbook/worksheets/{id}/range/rowsAbove(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="e4cfe-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="e4cfe-118">Function parameters</span></span>

| <span data-ttu-id="e4cfe-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="e4cfe-119">Parameter</span></span>    | <span data-ttu-id="e4cfe-120">Тип</span><span class="sxs-lookup"><span data-stu-id="e4cfe-120">Type</span></span>   |<span data-ttu-id="e4cfe-121">Описание</span><span class="sxs-lookup"><span data-stu-id="e4cfe-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e4cfe-122">count</span><span class="sxs-lookup"><span data-stu-id="e4cfe-122">count</span></span>|<span data-ttu-id="e4cfe-123">Int32</span><span class="sxs-lookup"><span data-stu-id="e4cfe-123">Int32</span></span>|<span data-ttu-id="e4cfe-p102">Необязательный. Количество строк, включаемых в полученный диапазон. Чтобы создать диапазон за пределами текущего диапазона, используйте положительное число. Вы также можете использовать отрицательное число, чтобы создать диапазон в рамках текущего диапазона. Значение по умолчанию — 1.</span><span class="sxs-lookup"><span data-stu-id="e4cfe-p102">Optional. The number of rows to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="e4cfe-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e4cfe-129">Request headers</span></span>
| <span data-ttu-id="e4cfe-130">Имя</span><span class="sxs-lookup"><span data-stu-id="e4cfe-130">Name</span></span>       | <span data-ttu-id="e4cfe-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e4cfe-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e4cfe-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e4cfe-132">Authorization</span></span>  | <span data-ttu-id="e4cfe-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e4cfe-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e4cfe-135">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e4cfe-135">Workbook-Session-Id</span></span>  | <span data-ttu-id="e4cfe-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="e4cfe-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4cfe-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e4cfe-138">Request body</span></span>
<span data-ttu-id="e4cfe-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e4cfe-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4cfe-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4cfe-140">Response</span></span>

<span data-ttu-id="e4cfe-141">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/workbookrange.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e4cfe-141">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4cfe-142">Пример</span><span class="sxs-lookup"><span data-stu-id="e4cfe-142">Example</span></span>
<span data-ttu-id="e4cfe-143">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="e4cfe-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e4cfe-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="e4cfe-144">Request</span></span>
<span data-ttu-id="e4cfe-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e4cfe-145">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e4cfe-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="e4cfe-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookrange_rowsAbove"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range/rowsAbove(count=2)
```
# <a name="c"></a>[<span data-ttu-id="e4cfe-147">C#</span><span class="sxs-lookup"><span data-stu-id="e4cfe-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrange-rowsabove-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e4cfe-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e4cfe-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrange-rowsabove-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e4cfe-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e4cfe-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrange-rowsabove-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e4cfe-150">Java</span><span class="sxs-lookup"><span data-stu-id="e4cfe-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrange-rowsabove-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e4cfe-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4cfe-151">Response</span></span>
<span data-ttu-id="e4cfe-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e4cfe-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


