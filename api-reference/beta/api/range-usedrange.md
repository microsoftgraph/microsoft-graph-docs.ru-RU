---
title: 'Range: UsedRange'
description: Возвращает используемый диапазон заданного объекта диапазона.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: b5f208469ed1d472c61b07c2d51edcd7dc2c3ade
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36723254"
---
# <a name="range-usedrange"></a><span data-ttu-id="0ed01-103">Range: UsedRange</span><span class="sxs-lookup"><span data-stu-id="0ed01-103">Range: UsedRange</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ed01-104">Возвращает используемый диапазон заданного объекта диапазона.</span><span class="sxs-lookup"><span data-stu-id="0ed01-104">Returns the used range of the given range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0ed01-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0ed01-105">Permissions</span></span>
<span data-ttu-id="0ed01-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ed01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ed01-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ed01-108">Permission type</span></span>      | <span data-ttu-id="0ed01-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ed01-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ed01-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ed01-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0ed01-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ed01-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0ed01-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ed01-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ed01-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ed01-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0ed01-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0ed01-114">Application</span></span> | <span data-ttu-id="0ed01-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ed01-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ed01-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ed01-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/UsedRange
GET /workbook/worksheets/{id|name}/range(address='<address>')/UsedRange
GET /workbook/tables/{id|name}/columns/{id|name}/range/UsedRange

```
## <a name="request-headers"></a><span data-ttu-id="0ed01-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0ed01-117">Request headers</span></span>
| <span data-ttu-id="0ed01-118">Имя</span><span class="sxs-lookup"><span data-stu-id="0ed01-118">Name</span></span>       | <span data-ttu-id="0ed01-119">Описание</span><span class="sxs-lookup"><span data-stu-id="0ed01-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0ed01-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0ed01-120">Authorization</span></span>  | <span data-ttu-id="0ed01-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0ed01-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0ed01-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0ed01-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="0ed01-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="0ed01-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ed01-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0ed01-126">Request body</span></span>
<span data-ttu-id="0ed01-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="0ed01-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0ed01-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="0ed01-128">Parameter</span></span>    | <span data-ttu-id="0ed01-129">Тип</span><span class="sxs-lookup"><span data-stu-id="0ed01-129">Type</span></span>   |<span data-ttu-id="0ed01-130">Описание</span><span class="sxs-lookup"><span data-stu-id="0ed01-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0ed01-131">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="0ed01-131">valuesOnly</span></span>|<span data-ttu-id="0ed01-132">boolean</span><span class="sxs-lookup"><span data-stu-id="0ed01-132">boolean</span></span>|<span data-ttu-id="0ed01-p104">Необязательный. Учитывает только ячейки со значениями.</span><span class="sxs-lookup"><span data-stu-id="0ed01-p104">Optional. Considers only cells with values as used cells.</span></span>|

## <a name="response"></a><span data-ttu-id="0ed01-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ed01-135">Response</span></span>

<span data-ttu-id="0ed01-136">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/workbookrange.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0ed01-136">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ed01-137">Пример</span><span class="sxs-lookup"><span data-stu-id="0ed01-137">Example</span></span>
<span data-ttu-id="0ed01-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="0ed01-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0ed01-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ed01-139">Request</span></span>
<span data-ttu-id="0ed01-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0ed01-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0ed01-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="0ed01-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "range_usedrange"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/UsedRange
Content-type: application/json
Content-length: 24

{
  "valuesOnly": true
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0ed01-142">C#</span><span class="sxs-lookup"><span data-stu-id="0ed01-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-usedrange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0ed01-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0ed01-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-usedrange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0ed01-144">Цель — C</span><span class="sxs-lookup"><span data-stu-id="0ed01-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-usedrange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0ed01-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ed01-145">Response</span></span>
<span data-ttu-id="0ed01-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0ed01-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Range: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
