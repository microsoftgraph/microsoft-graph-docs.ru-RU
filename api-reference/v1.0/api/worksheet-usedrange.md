---
title: 'Worksheet: UsedRange'
description: Используемый диапазон — это наименьший диапазон, включающий в себя все ячейки, которые содержат значение или форматирование. Если лист пустой, эта функция вернет верхнюю левую ячейку.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 060aa6e30443c75707146dbdf00fb911ace6eb06
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051160"
---
# <a name="worksheet-usedrange"></a><span data-ttu-id="c47e9-104">Worksheet: UsedRange</span><span class="sxs-lookup"><span data-stu-id="c47e9-104">Worksheet: UsedRange</span></span>

<span data-ttu-id="c47e9-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c47e9-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c47e9-p102">Используемый диапазон — это наименьший диапазон, включающий в себя все ячейки, которые содержат значение или форматирование. Если лист пустой, эта функция вернет верхнюю левую ячейку.</span><span class="sxs-lookup"><span data-stu-id="c47e9-p102">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>
## <a name="permissions"></a><span data-ttu-id="c47e9-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c47e9-108">Permissions</span></span>
<span data-ttu-id="c47e9-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c47e9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c47e9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c47e9-111">Permission type</span></span>      | <span data-ttu-id="c47e9-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c47e9-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c47e9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c47e9-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c47e9-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c47e9-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c47e9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c47e9-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c47e9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c47e9-116">Not supported.</span></span>    |
|<span data-ttu-id="c47e9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c47e9-117">Application</span></span> | <span data-ttu-id="c47e9-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c47e9-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c47e9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c47e9-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/usedRange
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/usedRange

```

## <a name="function-parameters"></a><span data-ttu-id="c47e9-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="c47e9-120">Function parameters</span></span>
<span data-ttu-id="c47e9-121">В URL-адресе запроса могут быть указаны необязательные параметры.</span><span class="sxs-lookup"><span data-stu-id="c47e9-121">In the request URL you may provide optional parameters.</span></span>

| <span data-ttu-id="c47e9-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="c47e9-122">Parameter</span></span>    | <span data-ttu-id="c47e9-123">Тип</span><span class="sxs-lookup"><span data-stu-id="c47e9-123">Type</span></span>   |<span data-ttu-id="c47e9-124">Описание</span><span class="sxs-lookup"><span data-stu-id="c47e9-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c47e9-125">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="c47e9-125">valuesOnly</span></span>|<span data-ttu-id="c47e9-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="c47e9-126">Boolean</span></span>|<span data-ttu-id="c47e9-p104">Необязательный параметр. Учитывает только ячейки со значениями (игнорирует форматирование).</span><span class="sxs-lookup"><span data-stu-id="c47e9-p104">Optional. Considers only cells with values as used cells (ignores formatting).</span></span>|

## <a name="request-headers"></a><span data-ttu-id="c47e9-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c47e9-129">Request headers</span></span>
| <span data-ttu-id="c47e9-130">Имя</span><span class="sxs-lookup"><span data-stu-id="c47e9-130">Name</span></span>       | <span data-ttu-id="c47e9-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c47e9-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c47e9-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c47e9-132">Authorization</span></span>  | <span data-ttu-id="c47e9-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c47e9-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c47e9-135">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c47e9-135">Workbook-Session-Id</span></span>  | <span data-ttu-id="c47e9-p106">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="c47e9-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c47e9-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c47e9-138">Request body</span></span>
<span data-ttu-id="c47e9-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c47e9-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c47e9-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="c47e9-140">Response</span></span>

<span data-ttu-id="c47e9-141">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c47e9-141">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c47e9-142">Пример</span><span class="sxs-lookup"><span data-stu-id="c47e9-142">Example</span></span>
<span data-ttu-id="c47e9-143">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="c47e9-143">Here is an example that shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="c47e9-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="c47e9-144">Request</span></span>
<span data-ttu-id="c47e9-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c47e9-145">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c47e9-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="c47e9-146">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "worksheet_usedrange"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/usedRange
```
# <a name="c"></a>[<span data-ttu-id="c47e9-147">C#</span><span class="sxs-lookup"><span data-stu-id="c47e9-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheet-usedrange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c47e9-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c47e9-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheet-usedrange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c47e9-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c47e9-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheet-usedrange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c47e9-150">Java</span><span class="sxs-lookup"><span data-stu-id="c47e9-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheet-usedrange-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c47e9-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="c47e9-151">Response</span></span>
<span data-ttu-id="c47e9-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c47e9-152">Here is an example of the response.</span></span> <span data-ttu-id="c47e9-153">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c47e9-153">Note: The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value"
}
```

<span data-ttu-id="c47e9-154">Кроме того, эту функцию можно назвать с необязательным `valuesOnly` параметром.</span><span class="sxs-lookup"><span data-stu-id="c47e9-154">Alternatively, this function can be called with the optional `valuesOnly` parameter.</span></span>

##### <a name="request"></a><span data-ttu-id="c47e9-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="c47e9-155">Request</span></span>
<span data-ttu-id="c47e9-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c47e9-156">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c47e9-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="c47e9-157">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "worksheet_usedrange_valuesonly"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/usedRange(valuesOnly=true)
```
# <a name="c"></a>[<span data-ttu-id="c47e9-158">C#</span><span class="sxs-lookup"><span data-stu-id="c47e9-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheet-usedrange-valuesonly-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c47e9-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c47e9-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheet-usedrange-valuesonly-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c47e9-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c47e9-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheet-usedrange-valuesonly-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c47e9-161">Java</span><span class="sxs-lookup"><span data-stu-id="c47e9-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheet-usedrange-valuesonly-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c47e9-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="c47e9-162">Response</span></span>
<span data-ttu-id="c47e9-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c47e9-163">Here is an example of the response.</span></span> <span data-ttu-id="c47e9-164">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c47e9-164">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

