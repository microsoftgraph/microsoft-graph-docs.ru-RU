---
title: Получение объекта Table
description: Получение свойств и связей объекта таблицы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: a97433f824c299467da3b7f476c96a06d21790f7
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36729205"
---
# <a name="get-table"></a><span data-ttu-id="24574-103">Получение объекта Table</span><span class="sxs-lookup"><span data-stu-id="24574-103">Get Table</span></span>

<span data-ttu-id="24574-104">Получение свойств и связей объекта таблицы.</span><span class="sxs-lookup"><span data-stu-id="24574-104">Retrieve the properties and relationships of table object.</span></span>
## <a name="permissions"></a><span data-ttu-id="24574-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="24574-105">Permissions</span></span>
<span data-ttu-id="24574-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24574-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24574-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="24574-108">Permission type</span></span>      | <span data-ttu-id="24574-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="24574-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="24574-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="24574-110">Delegated (work or school account)</span></span> | <span data-ttu-id="24574-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="24574-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="24574-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="24574-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24574-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24574-113">Not supported.</span></span>    |
|<span data-ttu-id="24574-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="24574-114">Application</span></span> | <span data-ttu-id="24574-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24574-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="24574-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="24574-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}
GET /workbook/worksheets/{id|name}/tables/{id|name}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="24574-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="24574-117">Optional query parameters</span></span>
<span data-ttu-id="24574-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="24574-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="24574-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="24574-119">Request headers</span></span>
| <span data-ttu-id="24574-120">Имя</span><span class="sxs-lookup"><span data-stu-id="24574-120">Name</span></span>      |<span data-ttu-id="24574-121">Описание</span><span class="sxs-lookup"><span data-stu-id="24574-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="24574-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="24574-122">Authorization</span></span>  | <span data-ttu-id="24574-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="24574-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="24574-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="24574-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="24574-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="24574-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="24574-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="24574-128">Request body</span></span>
<span data-ttu-id="24574-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="24574-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24574-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="24574-130">Response</span></span>

<span data-ttu-id="24574-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [воркбуктабле](../resources/table.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="24574-131">If successful, this method returns a `200 OK` response code and [WorkbookTable](../resources/table.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="24574-132">Пример</span><span class="sxs-lookup"><span data-stu-id="24574-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="24574-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="24574-133">Request</span></span>
<span data-ttu-id="24574-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="24574-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="24574-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="24574-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_table"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="24574-136">C#</span><span class="sxs-lookup"><span data-stu-id="24574-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-table-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="24574-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="24574-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-table-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="24574-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="24574-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-table-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="24574-139">Java</span><span class="sxs-lookup"><span data-stu-id="24574-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-table-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="24574-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="24574-140">Response</span></span>
<span data-ttu-id="24574-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="24574-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTable"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 109

{
  "id": "99",
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get Table",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
