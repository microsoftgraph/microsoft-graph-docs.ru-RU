---
title: 'workbookRange: columnsBefore'
description: Возвращает определенное количество столбцов слева от заданного диапазона.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 7ef6a350e3da997f0f33423a779e6301023753d7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35866329"
---
# <a name="workbookrange-columnsbefore"></a><span data-ttu-id="dce1c-103">workbookRange: columnsBefore</span><span class="sxs-lookup"><span data-stu-id="dce1c-103">workbookRange: columnsBefore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dce1c-104">Возвращает определенное количество столбцов слева от заданного диапазона.</span><span class="sxs-lookup"><span data-stu-id="dce1c-104">Gets a certain number of columns to the left of the given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="dce1c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dce1c-105">Permissions</span></span>
<span data-ttu-id="dce1c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dce1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dce1c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dce1c-108">Permission type</span></span>      | <span data-ttu-id="dce1c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dce1c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dce1c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dce1c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dce1c-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dce1c-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dce1c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dce1c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dce1c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dce1c-113">Not supported.</span></span>    |
|<span data-ttu-id="dce1c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dce1c-114">Application</span></span> | <span data-ttu-id="dce1c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dce1c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dce1c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dce1c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/columnsBefore(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="dce1c-117">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="dce1c-117">Function parameters</span></span>

| <span data-ttu-id="dce1c-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="dce1c-118">Parameter</span></span>    | <span data-ttu-id="dce1c-119">Тип</span><span class="sxs-lookup"><span data-stu-id="dce1c-119">Type</span></span>   |<span data-ttu-id="dce1c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="dce1c-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dce1c-121">count</span><span class="sxs-lookup"><span data-stu-id="dce1c-121">count</span></span>|<span data-ttu-id="dce1c-122">Int32</span><span class="sxs-lookup"><span data-stu-id="dce1c-122">Int32</span></span>|<span data-ttu-id="dce1c-p102">Количество столбцов, которые нужно включить в результирующий диапазон. Чтобы создать диапазон за пределами текущего диапазона, используйте положительное число. Вы также можете использовать отрицательное число, чтобы создать диапазон в рамках текущего диапазона. Значение по умолчанию — 1.</span><span class="sxs-lookup"><span data-stu-id="dce1c-p102">The number of columns to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="dce1c-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dce1c-127">Request headers</span></span>
| <span data-ttu-id="dce1c-128">Имя</span><span class="sxs-lookup"><span data-stu-id="dce1c-128">Name</span></span>       | <span data-ttu-id="dce1c-129">Описание</span><span class="sxs-lookup"><span data-stu-id="dce1c-129">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="dce1c-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dce1c-130">Authorization</span></span>  | <span data-ttu-id="dce1c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dce1c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dce1c-133">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="dce1c-133">Workbook-Session-Id</span></span>  | <span data-ttu-id="dce1c-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="dce1c-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dce1c-136">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dce1c-136">Request body</span></span>
<span data-ttu-id="dce1c-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dce1c-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dce1c-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="dce1c-138">Response</span></span>
<span data-ttu-id="dce1c-139">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/workbookrange.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="dce1c-139">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dce1c-140">Пример</span><span class="sxs-lookup"><span data-stu-id="dce1c-140">Example</span></span>
<span data-ttu-id="dce1c-141">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="dce1c-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="dce1c-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="dce1c-142">Request</span></span>
<span data-ttu-id="dce1c-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dce1c-143">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="dce1c-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="dce1c-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookrange_columnsbefore"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range/columnsBefore(count=2)
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dce1c-145">C#</span><span class="sxs-lookup"><span data-stu-id="dce1c-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrange-columnsbefore-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dce1c-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="dce1c-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrange-columnsbefore-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dce1c-147">Цель — C</span><span class="sxs-lookup"><span data-stu-id="dce1c-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrange-columnsbefore-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="dce1c-148">Java</span><span class="sxs-lookup"><span data-stu-id="dce1c-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrange-columnsbefore-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="dce1c-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="dce1c-149">Response</span></span>
<span data-ttu-id="dce1c-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dce1c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
