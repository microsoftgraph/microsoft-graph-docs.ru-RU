---
title: 'Range: LastColumn'
description: .
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: cdf03dec9d69ddc2d4c4d934de7a375f772f49e2
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36412217"
---
# <a name="range-lastcolumn"></a><span data-ttu-id="35f6a-103">Range: LastColumn</span><span class="sxs-lookup"><span data-stu-id="35f6a-103">Range: LastColumn</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35f6a-p101">Возвращает последний столбец в диапазоне. Например, последний столбец диапазона B2:D5 — D2:D5.</span><span class="sxs-lookup"><span data-stu-id="35f6a-p101">Gets the last column within the range. For example, the last column of "B2:D5" is "D2:D5".</span></span>
## <a name="permissions"></a><span data-ttu-id="35f6a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="35f6a-106">Permissions</span></span>
<span data-ttu-id="35f6a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35f6a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35f6a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="35f6a-109">Permission type</span></span>      | <span data-ttu-id="35f6a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="35f6a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="35f6a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="35f6a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="35f6a-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="35f6a-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="35f6a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="35f6a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35f6a-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="35f6a-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="35f6a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="35f6a-115">Application</span></span> | <span data-ttu-id="35f6a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35f6a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="35f6a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="35f6a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/LastColumn
GET /workbook/worksheets/{id|name}/range(address='<address>')/LastColumn
GET /workbook/tables/{id|name}/columns/{id|name}/range/LastColumn

```
## <a name="request-headers"></a><span data-ttu-id="35f6a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="35f6a-118">Request headers</span></span>
| <span data-ttu-id="35f6a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="35f6a-119">Name</span></span>       | <span data-ttu-id="35f6a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="35f6a-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="35f6a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="35f6a-121">Authorization</span></span>  | <span data-ttu-id="35f6a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="35f6a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="35f6a-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="35f6a-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="35f6a-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="35f6a-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="35f6a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="35f6a-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="35f6a-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="35f6a-128">Response</span></span>

<span data-ttu-id="35f6a-129">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/workbookrange.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="35f6a-129">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35f6a-130">Пример</span><span class="sxs-lookup"><span data-stu-id="35f6a-130">Example</span></span>
<span data-ttu-id="35f6a-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="35f6a-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="35f6a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="35f6a-132">Request</span></span>
<span data-ttu-id="35f6a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="35f6a-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="35f6a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="35f6a-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "range_lastcolumn"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/LastColumn
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="35f6a-135">C#</span><span class="sxs-lookup"><span data-stu-id="35f6a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-lastcolumn-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="35f6a-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="35f6a-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-lastcolumn-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="35f6a-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="35f6a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-lastcolumn-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="35f6a-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="35f6a-138">Response</span></span>
<span data-ttu-id="35f6a-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="35f6a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: LastColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
