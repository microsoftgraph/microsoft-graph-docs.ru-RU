---
title: Получение объекта TableColumn
description: Получение свойств и связей объекта tablecolumn.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 048e07c2439d007334380fb8de9746c7d2069e50
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36024430"
---
# <a name="get-tablecolumn"></a><span data-ttu-id="f2bec-103">Получение объекта TableColumn</span><span class="sxs-lookup"><span data-stu-id="f2bec-103">Get TableColumn</span></span>

<span data-ttu-id="f2bec-104">Получение свойств и связей объекта tablecolumn.</span><span class="sxs-lookup"><span data-stu-id="f2bec-104">Retrieve the properties and relationships of tablecolumn object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f2bec-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f2bec-105">Permissions</span></span>
<span data-ttu-id="f2bec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2bec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2bec-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f2bec-108">Permission type</span></span>      | <span data-ttu-id="f2bec-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f2bec-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2bec-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f2bec-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f2bec-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f2bec-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f2bec-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f2bec-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2bec-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2bec-113">Not supported.</span></span>    |
|<span data-ttu-id="f2bec-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f2bec-114">Application</span></span> | <span data-ttu-id="f2bec-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2bec-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2bec-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f2bec-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/columns/{id|name}
GET /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f2bec-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f2bec-117">Optional query parameters</span></span>
<span data-ttu-id="f2bec-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f2bec-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f2bec-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f2bec-119">Request headers</span></span>
| <span data-ttu-id="f2bec-120">Имя</span><span class="sxs-lookup"><span data-stu-id="f2bec-120">Name</span></span>      |<span data-ttu-id="f2bec-121">Описание</span><span class="sxs-lookup"><span data-stu-id="f2bec-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f2bec-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f2bec-122">Authorization</span></span>  | <span data-ttu-id="f2bec-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f2bec-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f2bec-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f2bec-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="f2bec-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="f2bec-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2bec-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f2bec-128">Request body</span></span>
<span data-ttu-id="f2bec-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f2bec-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2bec-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2bec-130">Response</span></span>

<span data-ttu-id="f2bec-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [воркбуктаблеколумн](../resources/tablecolumn.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f2bec-131">If successful, this method returns a `200 OK` response code and [WorkbookTableColumn](../resources/tablecolumn.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f2bec-132">Пример</span><span class="sxs-lookup"><span data-stu-id="f2bec-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f2bec-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="f2bec-133">Request</span></span>
<span data-ttu-id="f2bec-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f2bec-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f2bec-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="f2bec-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tablecolumn"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f2bec-136">C#</span><span class="sxs-lookup"><span data-stu-id="f2bec-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tablecolumn-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f2bec-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="f2bec-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tablecolumn-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f2bec-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="f2bec-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tablecolumn-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f2bec-139">Java</span><span class="sxs-lookup"><span data-stu-id="f2bec-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tablecolumn-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f2bec-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2bec-140">Response</span></span>
<span data-ttu-id="f2bec-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f2bec-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableColumn"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get TableColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
