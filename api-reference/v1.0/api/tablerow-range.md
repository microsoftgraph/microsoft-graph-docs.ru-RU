---
title: 'TableRow: Range'
description: Возвращает объект диапазона, связанный со всей строкой.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: eec63b5377afe21dfcdff10e4c25b1c1075b3910
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35894221"
---
# <a name="tablerow-range"></a><span data-ttu-id="706d6-103">TableRow: Range</span><span class="sxs-lookup"><span data-stu-id="706d6-103">TableRow: Range</span></span>

<span data-ttu-id="706d6-104">Возвращает объект диапазона, связанный со всей строкой.</span><span class="sxs-lookup"><span data-stu-id="706d6-104">Returns the range object associated with the entire row.</span></span>
## <a name="permissions"></a><span data-ttu-id="706d6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="706d6-105">Permissions</span></span>
<span data-ttu-id="706d6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="706d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="706d6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="706d6-108">Permission type</span></span>      | <span data-ttu-id="706d6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="706d6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="706d6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="706d6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="706d6-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="706d6-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="706d6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="706d6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="706d6-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="706d6-113">Not supported.</span></span>    |
|<span data-ttu-id="706d6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="706d6-114">Application</span></span> | <span data-ttu-id="706d6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="706d6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="706d6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="706d6-116">HTTP request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="706d6-117">HTTP</span><span class="sxs-lookup"><span data-stu-id="706d6-117">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/rows/{index}/range
GET /workbook/worksheets/{id|name}/tables/{id|name}/rows/{index}/range

```
## <a name="request-headers"></a><span data-ttu-id="706d6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="706d6-118">Request headers</span></span>
| <span data-ttu-id="706d6-119">Имя</span><span class="sxs-lookup"><span data-stu-id="706d6-119">Name</span></span>       | <span data-ttu-id="706d6-120">Описание</span><span class="sxs-lookup"><span data-stu-id="706d6-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="706d6-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="706d6-121">Authorization</span></span>  | <span data-ttu-id="706d6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="706d6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="706d6-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="706d6-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="706d6-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="706d6-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="706d6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="706d6-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="706d6-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="706d6-128">Response</span></span>

<span data-ttu-id="706d6-129">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="706d6-129">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="706d6-130">Пример</span><span class="sxs-lookup"><span data-stu-id="706d6-130">Example</span></span>
<span data-ttu-id="706d6-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="706d6-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="706d6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="706d6-132">Request</span></span>
<span data-ttu-id="706d6-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="706d6-133">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "tablerow_range"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}/range
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="706d6-134">C#</span><span class="sxs-lookup"><span data-stu-id="706d6-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablerow-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="706d6-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="706d6-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablerow-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="706d6-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="706d6-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablerow-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="706d6-137">Java</span><span class="sxs-lookup"><span data-stu-id="706d6-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablerow-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="706d6-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="706d6-138">Response</span></span>
<span data-ttu-id="706d6-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="706d6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "TableRow: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
