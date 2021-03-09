---
title: 'workbookTable: диапазон'
description: Получает объект диапазона, связанный со всей таблицей.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 6ba01f948a6b21dc2b53c52682f92f428bb2df95
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50576528"
---
# <a name="workbooktable-range"></a><span data-ttu-id="aa48b-103">workbookTable: диапазон</span><span class="sxs-lookup"><span data-stu-id="aa48b-103">workbookTable: range</span></span>

<span data-ttu-id="aa48b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa48b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa48b-105">Получает объект диапазона, связанный со всей таблицей.</span><span class="sxs-lookup"><span data-stu-id="aa48b-105">Gets the range object associated with the entire table.</span></span>
## <a name="permissions"></a><span data-ttu-id="aa48b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aa48b-106">Permissions</span></span>
<span data-ttu-id="aa48b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa48b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa48b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aa48b-109">Permission type</span></span>      | <span data-ttu-id="aa48b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aa48b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa48b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aa48b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="aa48b-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aa48b-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="aa48b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aa48b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa48b-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aa48b-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="aa48b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aa48b-115">Application</span></span> | <span data-ttu-id="aa48b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa48b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="aa48b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aa48b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/tables/{id|name}/Range
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/Range
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/Range
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/Range

```
## <a name="request-headers"></a><span data-ttu-id="aa48b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aa48b-118">Request headers</span></span>
| <span data-ttu-id="aa48b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="aa48b-119">Name</span></span>       | <span data-ttu-id="aa48b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="aa48b-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="aa48b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aa48b-121">Authorization</span></span>  | <span data-ttu-id="aa48b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aa48b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="aa48b-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="aa48b-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="aa48b-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="aa48b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa48b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aa48b-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="aa48b-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa48b-128">Response</span></span>

<span data-ttu-id="aa48b-129">В случае успешной работы этот метод возвращает код отклика и `200 OK` объект [workbookRange](../resources/workbookrange.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="aa48b-129">If successful, this method returns a `200 OK` response code and a [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa48b-130">Пример</span><span class="sxs-lookup"><span data-stu-id="aa48b-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="aa48b-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="aa48b-131">Request</span></span>
<span data-ttu-id="aa48b-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aa48b-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="aa48b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="aa48b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "table_range"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/Range
```
# <a name="c"></a>[<span data-ttu-id="aa48b-134">C#</span><span class="sxs-lookup"><span data-stu-id="aa48b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/table-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aa48b-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aa48b-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/table-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aa48b-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aa48b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/table-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aa48b-137">Java</span><span class="sxs-lookup"><span data-stu-id="aa48b-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/table-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="aa48b-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa48b-138">Response</span></span>
<span data-ttu-id="aa48b-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="aa48b-139">The following is an example of the response.</span></span> 

><span data-ttu-id="aa48b-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aa48b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Table: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


