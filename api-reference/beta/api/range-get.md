---
title: Получение объекта Range
description: Получение свойств и связей объекта диапазона.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: a251c19b5582478c85db3971c276c8b7204e9c57
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35978464"
---
# <a name="get-range"></a><span data-ttu-id="84514-103">Получение объекта Range</span><span class="sxs-lookup"><span data-stu-id="84514-103">Get Range</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84514-104">Получение свойств и связей объекта диапазона.</span><span class="sxs-lookup"><span data-stu-id="84514-104">Retrieve the properties and relationships of range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="84514-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="84514-105">Permissions</span></span>
<span data-ttu-id="84514-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84514-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84514-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="84514-108">Permission type</span></span>      | <span data-ttu-id="84514-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="84514-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="84514-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="84514-110">Delegated (work or school account)</span></span> | <span data-ttu-id="84514-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84514-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="84514-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="84514-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84514-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84514-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="84514-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="84514-114">Application</span></span> | <span data-ttu-id="84514-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84514-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="84514-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84514-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/range(address='<address>')
GET /workbook/tables/{id|name}/columns/{id|name}/range
```
## <a name="optional-query-parameters"></a><span data-ttu-id="84514-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="84514-117">Optional query parameters</span></span>
<span data-ttu-id="84514-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="84514-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="84514-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="84514-119">Request headers</span></span>
| <span data-ttu-id="84514-120">Имя</span><span class="sxs-lookup"><span data-stu-id="84514-120">Name</span></span>      |<span data-ttu-id="84514-121">Описание</span><span class="sxs-lookup"><span data-stu-id="84514-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="84514-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="84514-122">Authorization</span></span>  | <span data-ttu-id="84514-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="84514-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="84514-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="84514-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="84514-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="84514-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="84514-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="84514-128">Request body</span></span>
<span data-ttu-id="84514-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="84514-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84514-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="84514-130">Response</span></span>

<span data-ttu-id="84514-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [workbookRange](../resources/workbookrange.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="84514-131">If successful, this method returns a `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="84514-132">Пример</span><span class="sxs-lookup"><span data-stu-id="84514-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="84514-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="84514-133">Request</span></span>
<span data-ttu-id="84514-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="84514-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="84514-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="84514-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_range"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="84514-136">C#</span><span class="sxs-lookup"><span data-stu-id="84514-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="84514-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="84514-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="84514-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="84514-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="84514-139">Java</span><span class="sxs-lookup"><span data-stu-id="84514-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="84514-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="84514-140">Response</span></span>
<span data-ttu-id="84514-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="84514-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Get Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
