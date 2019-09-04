---
title: Получение объекта RangeBorder
description: Получение свойств и связей объекта rangeborder.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: a0164f98f74981c5b4504fca2a90c162badd4a7e
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36725411"
---
# <a name="get-rangeborder"></a><span data-ttu-id="84947-103">Получение объекта RangeBorder</span><span class="sxs-lookup"><span data-stu-id="84947-103">Get RangeBorder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84947-104">Получение свойств и связей объекта rangeborder.</span><span class="sxs-lookup"><span data-stu-id="84947-104">Retrieve the properties and relationships of rangeborder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="84947-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="84947-105">Permissions</span></span>
<span data-ttu-id="84947-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84947-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84947-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="84947-108">Permission type</span></span>      | <span data-ttu-id="84947-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="84947-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="84947-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="84947-110">Delegated (work or school account)</span></span> | <span data-ttu-id="84947-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84947-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="84947-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="84947-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84947-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84947-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="84947-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="84947-114">Application</span></span> | <span data-ttu-id="84947-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84947-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="84947-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84947-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/format/borders(<sideIndex>)
GET /workbook/worksheets/{id|name}/range(address='<address>')/format/borders(<sideIndex>)
GET /workbook/tables/{id|name}/columns/{id|name}/range/format/borders(<sideIndex>)
```
## <a name="optional-query-parameters"></a><span data-ttu-id="84947-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="84947-117">Optional query parameters</span></span>
<span data-ttu-id="84947-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="84947-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="84947-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="84947-119">Request headers</span></span>
| <span data-ttu-id="84947-120">Имя</span><span class="sxs-lookup"><span data-stu-id="84947-120">Name</span></span>      |<span data-ttu-id="84947-121">Описание</span><span class="sxs-lookup"><span data-stu-id="84947-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="84947-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="84947-122">Authorization</span></span>  | <span data-ttu-id="84947-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="84947-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="84947-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="84947-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="84947-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="84947-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="84947-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="84947-128">Request body</span></span>
<span data-ttu-id="84947-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="84947-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84947-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="84947-130">Response</span></span>

<span data-ttu-id="84947-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [воркбукранжебордер](../resources/workbookrangeborder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="84947-131">If successful, this method returns a `200 OK` response code and [workbookRangeBorder](../resources/workbookrangeborder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="84947-132">Пример</span><span class="sxs-lookup"><span data-stu-id="84947-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="84947-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="84947-133">Request</span></span>
<span data-ttu-id="84947-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="84947-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="84947-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="84947-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_rangeborder"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/format/borders/{sideIndex}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="84947-136">C#</span><span class="sxs-lookup"><span data-stu-id="84947-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-rangeborder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="84947-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="84947-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-rangeborder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="84947-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="84947-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-rangeborder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="84947-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="84947-139">Response</span></span>
<span data-ttu-id="84947-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="84947-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeBorder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get RangeBorder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
