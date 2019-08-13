---
title: 'Worksheet: UsedRange'
description: Используемый диапазон — это наименьший диапазон, включающий в себя все ячейки, которые содержат значение или форматирование. Если лист пустой, эта функция вернет верхнюю левую ячейку.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 1c8edff55502261902f6cfe717e7ded2ad3d8618
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358085"
---
# <a name="worksheet-usedrange"></a><span data-ttu-id="e2789-104">Worksheet: UsedRange</span><span class="sxs-lookup"><span data-stu-id="e2789-104">Worksheet: UsedRange</span></span>

<span data-ttu-id="e2789-p102">Используемый диапазон — это наименьший диапазон, включающий в себя все ячейки, которые содержат значение или форматирование. Если лист пустой, эта функция вернет верхнюю левую ячейку.</span><span class="sxs-lookup"><span data-stu-id="e2789-p102">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>
## <a name="permissions"></a><span data-ttu-id="e2789-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e2789-107">Permissions</span></span>
<span data-ttu-id="e2789-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2789-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2789-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e2789-110">Permission type</span></span>      | <span data-ttu-id="e2789-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e2789-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2789-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e2789-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e2789-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e2789-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e2789-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e2789-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2789-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2789-115">Not supported.</span></span>    |
|<span data-ttu-id="e2789-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e2789-116">Application</span></span> | <span data-ttu-id="e2789-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2789-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2789-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e2789-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/UsedRange

```

## <a name="function-parameters"></a><span data-ttu-id="e2789-119">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="e2789-119">Function parameters</span></span>
<span data-ttu-id="e2789-120">В URL-адресе запроса предоставьте необязательный параметр запросов.</span><span class="sxs-lookup"><span data-stu-id="e2789-120">In the request URL, provide an optional query parameter.</span></span>

| <span data-ttu-id="e2789-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="e2789-121">Parameter</span></span>    | <span data-ttu-id="e2789-122">Тип</span><span class="sxs-lookup"><span data-stu-id="e2789-122">Type</span></span>   |<span data-ttu-id="e2789-123">Описание</span><span class="sxs-lookup"><span data-stu-id="e2789-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e2789-124">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="e2789-124">valuesOnly</span></span>|<span data-ttu-id="e2789-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2789-125">Boolean</span></span>|<span data-ttu-id="e2789-p104">Необязательный параметр. Учитывает только ячейки со значениями (игнорирует форматирование).</span><span class="sxs-lookup"><span data-stu-id="e2789-p104">Optional. Considers only cells with values as used cells (ignores formatting).</span></span>|

## <a name="request-headers"></a><span data-ttu-id="e2789-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e2789-128">Request headers</span></span>
| <span data-ttu-id="e2789-129">Имя</span><span class="sxs-lookup"><span data-stu-id="e2789-129">Name</span></span>       | <span data-ttu-id="e2789-130">Описание</span><span class="sxs-lookup"><span data-stu-id="e2789-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e2789-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e2789-131">Authorization</span></span>  | <span data-ttu-id="e2789-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e2789-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e2789-134">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e2789-134">Workbook-Session-Id</span></span>  | <span data-ttu-id="e2789-p106">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="e2789-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2789-137">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e2789-137">Request body</span></span>
<span data-ttu-id="e2789-138">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e2789-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2789-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2789-139">Response</span></span>

<span data-ttu-id="e2789-140">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/workbookrange.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e2789-140">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2789-141">Пример</span><span class="sxs-lookup"><span data-stu-id="e2789-141">Example</span></span>
<span data-ttu-id="e2789-142">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="e2789-142">Here is an example that shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e2789-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="e2789-143">Request</span></span>
<span data-ttu-id="e2789-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e2789-144">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e2789-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="e2789-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "worksheet_usedrange"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/UsedRange(valuesOnly=true)
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e2789-146">C#</span><span class="sxs-lookup"><span data-stu-id="e2789-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheet-usedrange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e2789-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e2789-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheet-usedrange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e2789-148">Цель — C</span><span class="sxs-lookup"><span data-stu-id="e2789-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheet-usedrange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e2789-149">Java</span><span class="sxs-lookup"><span data-stu-id="e2789-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheet-usedrange-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e2789-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2789-150">Response</span></span>
<span data-ttu-id="e2789-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e2789-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
