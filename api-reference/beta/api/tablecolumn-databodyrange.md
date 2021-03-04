---
title: 'TableColumn: DataBodyRange'
description: Получает объект диапазона, связанный с данными столбца.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 4da9f394df7f050d2ecb480639d593630d3ccb9e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440681"
---
# <a name="tablecolumn-databodyrange"></a><span data-ttu-id="dddb2-103">TableColumn: DataBodyRange</span><span class="sxs-lookup"><span data-stu-id="dddb2-103">TableColumn: DataBodyRange</span></span>

<span data-ttu-id="dddb2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dddb2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dddb2-105">Получает объект диапазона, связанный с данными столбца.</span><span class="sxs-lookup"><span data-stu-id="dddb2-105">Gets the range object associated with the data body of the column.</span></span>
## <a name="permissions"></a><span data-ttu-id="dddb2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dddb2-106">Permissions</span></span>
<span data-ttu-id="dddb2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dddb2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dddb2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dddb2-109">Permission type</span></span>      | <span data-ttu-id="dddb2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dddb2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dddb2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dddb2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dddb2-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dddb2-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dddb2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dddb2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dddb2-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dddb2-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dddb2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dddb2-115">Application</span></span> | <span data-ttu-id="dddb2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dddb2-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dddb2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dddb2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/columns/{id|name}/DataBodyRange
GET /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/DataBodyRange

```
## <a name="request-headers"></a><span data-ttu-id="dddb2-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dddb2-118">Request headers</span></span>
| <span data-ttu-id="dddb2-119">Имя</span><span class="sxs-lookup"><span data-stu-id="dddb2-119">Name</span></span>       | <span data-ttu-id="dddb2-120">Описание</span><span class="sxs-lookup"><span data-stu-id="dddb2-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="dddb2-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dddb2-121">Authorization</span></span>  | <span data-ttu-id="dddb2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dddb2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dddb2-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="dddb2-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="dddb2-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="dddb2-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dddb2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dddb2-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="dddb2-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="dddb2-128">Response</span></span>

<span data-ttu-id="dddb2-129">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/workbookrange.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="dddb2-129">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dddb2-130">Пример</span><span class="sxs-lookup"><span data-stu-id="dddb2-130">Example</span></span>
<span data-ttu-id="dddb2-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="dddb2-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="dddb2-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="dddb2-132">Request</span></span>
<span data-ttu-id="dddb2-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dddb2-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dddb2-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="dddb2-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tablecolumn_databodyrange"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/DataBodyRange
```
# <a name="c"></a>[<span data-ttu-id="dddb2-135">C#</span><span class="sxs-lookup"><span data-stu-id="dddb2-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablecolumn-databodyrange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dddb2-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dddb2-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablecolumn-databodyrange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dddb2-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dddb2-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablecolumn-databodyrange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dddb2-138">Java</span><span class="sxs-lookup"><span data-stu-id="dddb2-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablecolumn-databodyrange-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="dddb2-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="dddb2-139">Response</span></span>
<span data-ttu-id="dddb2-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dddb2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "TableColumn: DataBodyRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


