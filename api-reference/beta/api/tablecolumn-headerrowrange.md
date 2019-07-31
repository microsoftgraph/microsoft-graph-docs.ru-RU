---
title: 'TableColumn: HeaderRowRange'
description: Получает объект диапазона, связанный со строкой заголовков столбца.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: c8129295be9aabac9e5b626ce43b492e3facb1e0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35982524"
---
# <a name="tablecolumn-headerrowrange"></a><span data-ttu-id="4f83f-103">TableColumn: HeaderRowRange</span><span class="sxs-lookup"><span data-stu-id="4f83f-103">TableColumn: HeaderRowRange</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f83f-104">Получает объект диапазона, связанный со строкой заголовков столбца.</span><span class="sxs-lookup"><span data-stu-id="4f83f-104">Gets the range object associated with the header row of the column.</span></span>
## <a name="permissions"></a><span data-ttu-id="4f83f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4f83f-105">Permissions</span></span>
<span data-ttu-id="4f83f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f83f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f83f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f83f-108">Permission type</span></span>      | <span data-ttu-id="4f83f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f83f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4f83f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f83f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4f83f-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4f83f-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4f83f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f83f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f83f-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4f83f-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4f83f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4f83f-114">Application</span></span> | <span data-ttu-id="4f83f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f83f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4f83f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f83f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/HeaderRowRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/HeaderRowRange

```
## <a name="request-headers"></a><span data-ttu-id="4f83f-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4f83f-117">Request headers</span></span>
| <span data-ttu-id="4f83f-118">Имя</span><span class="sxs-lookup"><span data-stu-id="4f83f-118">Name</span></span>       | <span data-ttu-id="4f83f-119">Описание</span><span class="sxs-lookup"><span data-stu-id="4f83f-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4f83f-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4f83f-120">Authorization</span></span>  | <span data-ttu-id="4f83f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4f83f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4f83f-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4f83f-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="4f83f-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="4f83f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f83f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4f83f-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="4f83f-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f83f-127">Response</span></span>

<span data-ttu-id="4f83f-128">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/workbookrange.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4f83f-128">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f83f-129">Пример</span><span class="sxs-lookup"><span data-stu-id="4f83f-129">Example</span></span>
<span data-ttu-id="4f83f-130">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="4f83f-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4f83f-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f83f-131">Request</span></span>
<span data-ttu-id="4f83f-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4f83f-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4f83f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="4f83f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tablecolumn_headerrowrange"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/HeaderRowRange
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4f83f-134">C#</span><span class="sxs-lookup"><span data-stu-id="4f83f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablecolumn-headerrowrange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4f83f-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="4f83f-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablecolumn-headerrowrange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4f83f-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="4f83f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablecolumn-headerrowrange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4f83f-137">Java</span><span class="sxs-lookup"><span data-stu-id="4f83f-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablecolumn-headerrowrange-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4f83f-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f83f-138">Response</span></span>
<span data-ttu-id="4f83f-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4f83f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "TableColumn: HeaderRowRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
