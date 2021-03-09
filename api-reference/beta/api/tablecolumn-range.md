---
title: 'TableColumn: Range'
description: Получает объект диапазона, связанный со всем столбцом.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 131cd75e3f9e0183ed2013b824e5963979422f16
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50576367"
---
# <a name="tablecolumn-range"></a><span data-ttu-id="8e858-103">TableColumn: Range</span><span class="sxs-lookup"><span data-stu-id="8e858-103">TableColumn: Range</span></span>

<span data-ttu-id="8e858-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e858-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e858-105">Получает объект диапазона, связанный со всем столбцом.</span><span class="sxs-lookup"><span data-stu-id="8e858-105">Gets the range object associated with the entire column.</span></span>
## <a name="permissions"></a><span data-ttu-id="8e858-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8e858-106">Permissions</span></span>
<span data-ttu-id="8e858-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e858-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e858-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e858-109">Permission type</span></span>      | <span data-ttu-id="8e858-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e858-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e858-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e858-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8e858-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8e858-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8e858-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e858-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e858-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8e858-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8e858-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8e858-115">Application</span></span> | <span data-ttu-id="8e858-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e858-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8e858-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e858-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/Range
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/Range
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/Range
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/Range

```
## <a name="request-headers"></a><span data-ttu-id="8e858-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8e858-118">Request headers</span></span>
| <span data-ttu-id="8e858-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8e858-119">Name</span></span>       | <span data-ttu-id="8e858-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8e858-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8e858-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8e858-121">Authorization</span></span>  | <span data-ttu-id="8e858-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e858-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8e858-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8e858-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="8e858-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="8e858-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e858-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8e858-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="8e858-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e858-128">Response</span></span>

<span data-ttu-id="8e858-129">В случае успеха этот метод возвращает код ответа и `200 OK` [объект workbookRange](../resources/workbookrange.md)в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="8e858-129">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md)) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e858-130">Пример</span><span class="sxs-lookup"><span data-stu-id="8e858-130">Example</span></span>
<span data-ttu-id="8e858-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="8e858-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8e858-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e858-132">Request</span></span>
<span data-ttu-id="8e858-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e858-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8e858-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e858-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tablecolumn_range"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/Range
```
# <a name="c"></a>[<span data-ttu-id="8e858-135">C#</span><span class="sxs-lookup"><span data-stu-id="8e858-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablecolumn-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8e858-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e858-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablecolumn-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8e858-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e858-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablecolumn-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8e858-138">Java</span><span class="sxs-lookup"><span data-stu-id="8e858-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablecolumn-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8e858-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e858-139">Response</span></span>
<span data-ttu-id="8e858-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8e858-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "TableColumn: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


