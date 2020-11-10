---
title: 'Worksheet: UsedRange'
description: Используемый диапазон — это наименьший диапазон, включающий в себя все ячейки, которые содержат значение или форматирование. Если лист пустой, эта функция вернет верхнюю левую ячейку.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: cc587a9a18193dd18756809f7865afd4e809be28
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980153"
---
# <a name="worksheet-usedrange"></a><span data-ttu-id="9a293-104">Worksheet: UsedRange</span><span class="sxs-lookup"><span data-stu-id="9a293-104">Worksheet: UsedRange</span></span>

<span data-ttu-id="9a293-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a293-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9a293-p102">Используемый диапазон — это наименьший диапазон, включающий в себя все ячейки, которые содержат значение или форматирование. Если лист пустой, эта функция вернет верхнюю левую ячейку.</span><span class="sxs-lookup"><span data-stu-id="9a293-p102">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>
## <a name="permissions"></a><span data-ttu-id="9a293-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9a293-108">Permissions</span></span>
<span data-ttu-id="9a293-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a293-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a293-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9a293-111">Permission type</span></span>      | <span data-ttu-id="9a293-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9a293-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a293-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9a293-113">Delegated (work or school account)</span></span> | <span data-ttu-id="9a293-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9a293-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9a293-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9a293-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a293-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a293-116">Not supported.</span></span>    |
|<span data-ttu-id="9a293-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9a293-117">Application</span></span> | <span data-ttu-id="9a293-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a293-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a293-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9a293-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/UsedRange

```

## <a name="function-parameters"></a><span data-ttu-id="9a293-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="9a293-120">Function parameters</span></span>
<span data-ttu-id="9a293-121">В URL-адресе запроса предоставьте необязательный параметр запросов.</span><span class="sxs-lookup"><span data-stu-id="9a293-121">In the request URL, provide an optional query parameter.</span></span>

| <span data-ttu-id="9a293-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="9a293-122">Parameter</span></span>    | <span data-ttu-id="9a293-123">Тип</span><span class="sxs-lookup"><span data-stu-id="9a293-123">Type</span></span>   |<span data-ttu-id="9a293-124">Описание</span><span class="sxs-lookup"><span data-stu-id="9a293-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9a293-125">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="9a293-125">valuesOnly</span></span>|<span data-ttu-id="9a293-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a293-126">Boolean</span></span>|<span data-ttu-id="9a293-p104">Необязательный параметр. Учитывает только ячейки со значениями (игнорирует форматирование).</span><span class="sxs-lookup"><span data-stu-id="9a293-p104">Optional. Considers only cells with values as used cells (ignores formatting).</span></span>|

## <a name="request-headers"></a><span data-ttu-id="9a293-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9a293-129">Request headers</span></span>
| <span data-ttu-id="9a293-130">Имя</span><span class="sxs-lookup"><span data-stu-id="9a293-130">Name</span></span>       | <span data-ttu-id="9a293-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9a293-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9a293-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9a293-132">Authorization</span></span>  | <span data-ttu-id="9a293-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9a293-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9a293-135">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9a293-135">Workbook-Session-Id</span></span>  | <span data-ttu-id="9a293-p106">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="9a293-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a293-138">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9a293-138">Request body</span></span>
<span data-ttu-id="9a293-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9a293-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a293-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a293-140">Response</span></span>

<span data-ttu-id="9a293-141">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/workbookrange.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9a293-141">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a293-142">Пример</span><span class="sxs-lookup"><span data-stu-id="9a293-142">Example</span></span>
<span data-ttu-id="9a293-143">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="9a293-143">Here is an example that shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9a293-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="9a293-144">Request</span></span>
<span data-ttu-id="9a293-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9a293-145">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9a293-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="9a293-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "worksheet_usedrange"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/UsedRange(valuesOnly=true)
```
# <a name="c"></a>[<span data-ttu-id="9a293-147">C#</span><span class="sxs-lookup"><span data-stu-id="9a293-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheet-usedrange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9a293-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9a293-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheet-usedrange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9a293-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9a293-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheet-usedrange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9a293-150">Java</span><span class="sxs-lookup"><span data-stu-id="9a293-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheet-usedrange-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9a293-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a293-151">Response</span></span>
<span data-ttu-id="9a293-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9a293-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


