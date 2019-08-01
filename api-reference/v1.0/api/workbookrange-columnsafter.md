---
title: 'workbookRange: columnsAfter'
description: Возвращает определенное количество столбцов справа от заданного диапазона.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: a7ae4e9d0a268979f133b703dca68499a6e903d0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36026406"
---
# <a name="workbookrange-columnsafter"></a><span data-ttu-id="6d42b-103">workbookRange: columnsAfter</span><span class="sxs-lookup"><span data-stu-id="6d42b-103">workbookRange: columnsAfter</span></span>

<span data-ttu-id="6d42b-104">Возвращает определенное количество столбцов справа от заданного диапазона.</span><span class="sxs-lookup"><span data-stu-id="6d42b-104">Gets a certain number of columns to the right of the given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="6d42b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6d42b-105">Permissions</span></span>
<span data-ttu-id="6d42b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d42b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d42b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6d42b-108">Permission type</span></span>      | <span data-ttu-id="6d42b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6d42b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6d42b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6d42b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6d42b-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6d42b-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6d42b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6d42b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d42b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d42b-113">Not supported.</span></span>    |
|<span data-ttu-id="6d42b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6d42b-114">Application</span></span> | <span data-ttu-id="6d42b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d42b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6d42b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6d42b-116">HTTP request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6d42b-117">HTTP</span><span class="sxs-lookup"><span data-stu-id="6d42b-117">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="6d42b-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="6d42b-118">Function parameters</span></span>

| <span data-ttu-id="6d42b-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="6d42b-119">Parameter</span></span>    | <span data-ttu-id="6d42b-120">Тип</span><span class="sxs-lookup"><span data-stu-id="6d42b-120">Type</span></span>   |<span data-ttu-id="6d42b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="6d42b-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6d42b-122">count</span><span class="sxs-lookup"><span data-stu-id="6d42b-122">count</span></span>|<span data-ttu-id="6d42b-123">Int32</span><span class="sxs-lookup"><span data-stu-id="6d42b-123">Int32</span></span>|<span data-ttu-id="6d42b-124">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="6d42b-124">Optional.</span></span> <span data-ttu-id="6d42b-125">Количество столбцов, включаемых в полученный диапазон.</span><span class="sxs-lookup"><span data-stu-id="6d42b-125">The number of columns to include in the resulting range.</span></span> <span data-ttu-id="6d42b-126">Чтобы создать диапазон за пределами текущего диапазона, используйте положительное число.</span><span class="sxs-lookup"><span data-stu-id="6d42b-126">In general, use a positive number to create a range outside the current range.</span></span> <span data-ttu-id="6d42b-127">Вы также можете указать отрицательное число, чтобы создать диапазон в рамках текущего диапазона.</span><span class="sxs-lookup"><span data-stu-id="6d42b-127">You can also use a negative number to create a range within the current range.</span></span> <span data-ttu-id="6d42b-128">По умолчанию используется значение 1.</span><span class="sxs-lookup"><span data-stu-id="6d42b-128">The default value is 1</span></span>|

## <a name="request-headers"></a><span data-ttu-id="6d42b-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6d42b-129">Request headers</span></span>
| <span data-ttu-id="6d42b-130">Имя</span><span class="sxs-lookup"><span data-stu-id="6d42b-130">Name</span></span>       | <span data-ttu-id="6d42b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6d42b-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6d42b-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6d42b-132">Authorization</span></span>  | <span data-ttu-id="6d42b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6d42b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6d42b-135">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="6d42b-135">Workbook-Session-Id</span></span>  | <span data-ttu-id="6d42b-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="6d42b-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d42b-138">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6d42b-138">Request body</span></span>
<span data-ttu-id="6d42b-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6d42b-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6d42b-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d42b-140">Response</span></span>
<span data-ttu-id="6d42b-141">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6d42b-141">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d42b-142">Пример</span><span class="sxs-lookup"><span data-stu-id="6d42b-142">Example</span></span>
<span data-ttu-id="6d42b-143">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="6d42b-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6d42b-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="6d42b-144">Request</span></span>
<span data-ttu-id="6d42b-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6d42b-145">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_columnsafter",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=2)
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6d42b-146">C#</span><span class="sxs-lookup"><span data-stu-id="6d42b-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrange-columnsafter-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6d42b-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="6d42b-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrange-columnsafter-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6d42b-148">Цель — C</span><span class="sxs-lookup"><span data-stu-id="6d42b-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrange-columnsafter-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6d42b-149">Java</span><span class="sxs-lookup"><span data-stu-id="6d42b-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrange-columnsafter-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6d42b-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d42b-150">Response</span></span>
<span data-ttu-id="6d42b-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6d42b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
