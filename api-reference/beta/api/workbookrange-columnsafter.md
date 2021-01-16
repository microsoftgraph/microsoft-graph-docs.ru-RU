---
title: 'workbookRange: columnsAfter'
description: Возвращает определенное количество столбцов справа от заданного диапазона.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: e577b691f1ebf746f4fb90b736924149fa8af770
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/16/2021
ms.locfileid: "49882914"
---
# <a name="workbookrange-columnsafter"></a><span data-ttu-id="f7763-103">workbookRange: columnsAfter</span><span class="sxs-lookup"><span data-stu-id="f7763-103">workbookRange: columnsAfter</span></span>

<span data-ttu-id="f7763-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7763-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7763-105">Возвращает определенное количество столбцов справа от заданного диапазона.</span><span class="sxs-lookup"><span data-stu-id="f7763-105">Gets a certain number of columns to the right of the given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7763-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f7763-106">Permissions</span></span>
<span data-ttu-id="f7763-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7763-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7763-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7763-109">Permission type</span></span>      | <span data-ttu-id="f7763-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7763-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7763-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7763-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f7763-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f7763-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f7763-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7763-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7763-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f7763-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f7763-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f7763-115">Application</span></span> | <span data-ttu-id="f7763-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7763-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7763-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7763-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=n)

```
## <a name="function-parameters"></a><span data-ttu-id="f7763-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="f7763-118">Function parameters</span></span>

| <span data-ttu-id="f7763-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="f7763-119">Parameter</span></span>    | <span data-ttu-id="f7763-120">Тип</span><span class="sxs-lookup"><span data-stu-id="f7763-120">Type</span></span>   |<span data-ttu-id="f7763-121">Описание</span><span class="sxs-lookup"><span data-stu-id="f7763-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f7763-122">count</span><span class="sxs-lookup"><span data-stu-id="f7763-122">count</span></span>|<span data-ttu-id="f7763-123">Int32</span><span class="sxs-lookup"><span data-stu-id="f7763-123">Int32</span></span>|<span data-ttu-id="f7763-p102">Количество столбцов, которые нужно включить в результирующий диапазон. Чтобы создать диапазон за пределами текущего диапазона, используйте положительное число. Вы также можете указать отрицательное число, чтобы создать диапазон в рамках текущего диапазона. По умолчанию используется значение 1.</span><span class="sxs-lookup"><span data-stu-id="f7763-p102">The number of columns to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1</span></span>|

## <a name="request-headers"></a><span data-ttu-id="f7763-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f7763-128">Request headers</span></span>
| <span data-ttu-id="f7763-129">Имя</span><span class="sxs-lookup"><span data-stu-id="f7763-129">Name</span></span>       | <span data-ttu-id="f7763-130">Описание</span><span class="sxs-lookup"><span data-stu-id="f7763-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f7763-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f7763-131">Authorization</span></span>  | <span data-ttu-id="f7763-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7763-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f7763-134">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f7763-134">Workbook-Session-Id</span></span>  | <span data-ttu-id="f7763-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="f7763-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7763-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f7763-137">Request body</span></span>
<span data-ttu-id="f7763-138">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f7763-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7763-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7763-139">Response</span></span>

<span data-ttu-id="f7763-140">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/workbookrange.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f7763-140">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7763-141">Пример</span><span class="sxs-lookup"><span data-stu-id="f7763-141">Example</span></span>
<span data-ttu-id="f7763-142">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="f7763-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f7763-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7763-143">Request</span></span>
<span data-ttu-id="f7763-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f7763-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f7763-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7763-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookrange_columnsafter"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=2)
```
# <a name="c"></a>[<span data-ttu-id="f7763-146">C#</span><span class="sxs-lookup"><span data-stu-id="f7763-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrange-columnsafter-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f7763-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f7763-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrange-columnsafter-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f7763-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f7763-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrange-columnsafter-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f7763-149">Java</span><span class="sxs-lookup"><span data-stu-id="f7763-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrange-columnsafter-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f7763-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7763-150">Response</span></span>
<span data-ttu-id="f7763-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f7763-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


