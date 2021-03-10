---
title: 'Table: TotalRowRange'
description: Получает объект диапазона, связанный со строкой итогов таблицы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 141d52f9a23eea2d2bca7ae73c366a200e918e55
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50575534"
---
# <a name="table-totalrowrange"></a><span data-ttu-id="485df-103">Table: TotalRowRange</span><span class="sxs-lookup"><span data-stu-id="485df-103">Table: TotalRowRange</span></span>

<span data-ttu-id="485df-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="485df-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="485df-105">Получает объект диапазона, связанный со строкой итогов таблицы.</span><span class="sxs-lookup"><span data-stu-id="485df-105">Gets the range object associated with totals row of the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="485df-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="485df-106">Permissions</span></span>
<span data-ttu-id="485df-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="485df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="485df-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="485df-109">Permission type</span></span>      | <span data-ttu-id="485df-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="485df-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="485df-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="485df-111">Delegated (work or school account)</span></span> | <span data-ttu-id="485df-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="485df-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="485df-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="485df-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="485df-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="485df-114">Not supported.</span></span>    |
|<span data-ttu-id="485df-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="485df-115">Application</span></span> | <span data-ttu-id="485df-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="485df-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="485df-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="485df-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/tables/{id|name}/totalRowRange
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/totalRowRange
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/totalRowRange
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/totalRowRange

```
## <a name="request-headers"></a><span data-ttu-id="485df-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="485df-118">Request headers</span></span>
| <span data-ttu-id="485df-119">Имя</span><span class="sxs-lookup"><span data-stu-id="485df-119">Name</span></span>       | <span data-ttu-id="485df-120">Описание</span><span class="sxs-lookup"><span data-stu-id="485df-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="485df-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="485df-121">Authorization</span></span>  | <span data-ttu-id="485df-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="485df-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="485df-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="485df-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="485df-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="485df-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="485df-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="485df-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="485df-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="485df-128">Response</span></span>

<span data-ttu-id="485df-129">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="485df-129">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="485df-130">Пример</span><span class="sxs-lookup"><span data-stu-id="485df-130">Example</span></span>
<span data-ttu-id="485df-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="485df-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="485df-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="485df-132">Request</span></span>
<span data-ttu-id="485df-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="485df-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="485df-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="485df-134">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "table_totalrowrange",
  "idempotent": true
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/totalRowRange
```
# <a name="c"></a>[<span data-ttu-id="485df-135">C#</span><span class="sxs-lookup"><span data-stu-id="485df-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/table-totalrowrange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="485df-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="485df-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/table-totalrowrange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="485df-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="485df-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/table-totalrowrange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="485df-138">Java</span><span class="sxs-lookup"><span data-stu-id="485df-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/table-totalrowrange-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="485df-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="485df-139">Response</span></span>
<span data-ttu-id="485df-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="485df-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Table: TotalRowRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

