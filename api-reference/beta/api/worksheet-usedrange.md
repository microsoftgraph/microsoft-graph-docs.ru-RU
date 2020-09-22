---
title: 'Worksheet: UsedRange'
description: Используемый диапазон — это наименьший диапазон, включающий в себя все ячейки, которые содержат значение или форматирование. Если лист пустой, эта функция вернет верхнюю левую ячейку.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 003f6e0a5b8a36a6184ac745e6ff7983f9b619a5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973983"
---
# <a name="worksheet-usedrange"></a><span data-ttu-id="4e435-104">Worksheet: UsedRange</span><span class="sxs-lookup"><span data-stu-id="4e435-104">Worksheet: UsedRange</span></span>

<span data-ttu-id="4e435-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e435-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4e435-p102">Используемый диапазон — это наименьший диапазон, включающий в себя все ячейки, которые содержат значение или форматирование. Если лист пустой, эта функция вернет верхнюю левую ячейку.</span><span class="sxs-lookup"><span data-stu-id="4e435-p102">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>
## <a name="permissions"></a><span data-ttu-id="4e435-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4e435-108">Permissions</span></span>
<span data-ttu-id="4e435-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e435-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e435-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e435-111">Permission type</span></span>      | <span data-ttu-id="4e435-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e435-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4e435-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e435-113">Delegated (work or school account)</span></span> | <span data-ttu-id="4e435-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4e435-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4e435-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e435-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e435-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e435-116">Not supported.</span></span>    |
|<span data-ttu-id="4e435-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4e435-117">Application</span></span> | <span data-ttu-id="4e435-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e435-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4e435-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e435-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/UsedRange

```

## <a name="function-parameters"></a><span data-ttu-id="4e435-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="4e435-120">Function parameters</span></span>
<span data-ttu-id="4e435-121">В URL-адресе запроса предоставьте необязательный параметр запросов.</span><span class="sxs-lookup"><span data-stu-id="4e435-121">In the request URL, provide an optional query parameter.</span></span>

| <span data-ttu-id="4e435-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="4e435-122">Parameter</span></span>    | <span data-ttu-id="4e435-123">Тип</span><span class="sxs-lookup"><span data-stu-id="4e435-123">Type</span></span>   |<span data-ttu-id="4e435-124">Описание</span><span class="sxs-lookup"><span data-stu-id="4e435-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4e435-125">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="4e435-125">valuesOnly</span></span>|<span data-ttu-id="4e435-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="4e435-126">Boolean</span></span>|<span data-ttu-id="4e435-p104">Необязательный параметр. Учитывает только ячейки со значениями (игнорирует форматирование).</span><span class="sxs-lookup"><span data-stu-id="4e435-p104">Optional. Considers only cells with values as used cells (ignores formatting).</span></span>|

## <a name="request-headers"></a><span data-ttu-id="4e435-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4e435-129">Request headers</span></span>
| <span data-ttu-id="4e435-130">Имя</span><span class="sxs-lookup"><span data-stu-id="4e435-130">Name</span></span>       | <span data-ttu-id="4e435-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4e435-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4e435-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4e435-132">Authorization</span></span>  | <span data-ttu-id="4e435-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4e435-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4e435-135">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4e435-135">Workbook-Session-Id</span></span>  | <span data-ttu-id="4e435-p106">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="4e435-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e435-138">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4e435-138">Request body</span></span>
<span data-ttu-id="4e435-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4e435-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4e435-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e435-140">Response</span></span>

<span data-ttu-id="4e435-141">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/workbookrange.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4e435-141">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e435-142">Пример</span><span class="sxs-lookup"><span data-stu-id="4e435-142">Example</span></span>
<span data-ttu-id="4e435-143">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="4e435-143">Here is an example that shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4e435-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e435-144">Request</span></span>
<span data-ttu-id="4e435-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4e435-145">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4e435-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="4e435-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "worksheet_usedrange"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/UsedRange(valuesOnly=true)
```
# <a name="c"></a>[<span data-ttu-id="4e435-147">C#</span><span class="sxs-lookup"><span data-stu-id="4e435-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheet-usedrange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4e435-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4e435-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheet-usedrange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4e435-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4e435-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheet-usedrange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4e435-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e435-150">Response</span></span>
<span data-ttu-id="4e435-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4e435-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


