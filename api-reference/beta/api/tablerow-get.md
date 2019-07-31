---
title: Получение объекта TableRow
description: Получение свойств и связей объекта tablerow.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 3ea0c7d70b7e248f96a8507854fc11a02a60635f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35982475"
---
# <a name="get-tablerow"></a><span data-ttu-id="f1d38-103">Получение объекта TableRow</span><span class="sxs-lookup"><span data-stu-id="f1d38-103">Get TableRow</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1d38-104">Получение свойств и связей объекта tablerow.</span><span class="sxs-lookup"><span data-stu-id="f1d38-104">Retrieve the properties and relationships of tablerow object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f1d38-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f1d38-105">Permissions</span></span>
<span data-ttu-id="f1d38-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1d38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1d38-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f1d38-108">Permission type</span></span>      | <span data-ttu-id="f1d38-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f1d38-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1d38-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f1d38-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f1d38-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f1d38-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f1d38-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f1d38-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1d38-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f1d38-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f1d38-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f1d38-114">Application</span></span> | <span data-ttu-id="f1d38-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1d38-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1d38-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f1d38-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/rows/{index}
GET /workbook/worksheets/{id|name}/tables/{id|name}/rows/{index}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f1d38-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f1d38-117">Optional query parameters</span></span>
<span data-ttu-id="f1d38-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f1d38-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f1d38-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f1d38-119">Request headers</span></span>
| <span data-ttu-id="f1d38-120">Имя</span><span class="sxs-lookup"><span data-stu-id="f1d38-120">Name</span></span>      |<span data-ttu-id="f1d38-121">Описание</span><span class="sxs-lookup"><span data-stu-id="f1d38-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f1d38-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f1d38-122">Authorization</span></span>  | <span data-ttu-id="f1d38-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f1d38-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f1d38-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f1d38-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="f1d38-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="f1d38-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1d38-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f1d38-128">Request body</span></span>
<span data-ttu-id="f1d38-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f1d38-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1d38-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1d38-130">Response</span></span>

<span data-ttu-id="f1d38-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [воркбуктаблеров](../resources/workbooktablerow.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f1d38-131">If successful, this method returns a `200 OK` response code and [workbookTableRow](../resources/workbooktablerow.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f1d38-132">Пример</span><span class="sxs-lookup"><span data-stu-id="f1d38-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f1d38-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="f1d38-133">Request</span></span>
<span data-ttu-id="f1d38-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f1d38-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f1d38-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="f1d38-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tablerow"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f1d38-136">C#</span><span class="sxs-lookup"><span data-stu-id="f1d38-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tablerow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f1d38-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="f1d38-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tablerow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f1d38-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="f1d38-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tablerow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f1d38-139">Java</span><span class="sxs-lookup"><span data-stu-id="f1d38-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tablerow-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f1d38-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1d38-140">Response</span></span>
<span data-ttu-id="f1d38-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f1d38-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableRow"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get TableRow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
