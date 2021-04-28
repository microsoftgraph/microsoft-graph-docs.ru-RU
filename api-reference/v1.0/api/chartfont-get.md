---
title: Получение объекта ChartFont
description: Получение свойств и связей объекта chartfont.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 4af4903612e08274f6bbcc326de5695509a69610
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052483"
---
# <a name="get-chartfont"></a><span data-ttu-id="9eca8-103">Получение объекта ChartFont</span><span class="sxs-lookup"><span data-stu-id="9eca8-103">Get ChartFont</span></span>

<span data-ttu-id="9eca8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9eca8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9eca8-105">Получение свойств и связей объекта chartfont.</span><span class="sxs-lookup"><span data-stu-id="9eca8-105">Retrieve the properties and relationships of chartfont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9eca8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9eca8-106">Permissions</span></span>
<span data-ttu-id="9eca8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9eca8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9eca8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9eca8-109">Permission type</span></span>      | <span data-ttu-id="9eca8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9eca8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9eca8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9eca8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9eca8-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9eca8-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9eca8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9eca8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9eca8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9eca8-114">Not supported.</span></span>    |
|<span data-ttu-id="9eca8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9eca8-115">Application</span></span> | <span data-ttu-id="9eca8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9eca8-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9eca8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9eca8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/format/font
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/format/font
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/format/font
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/format/font
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/format/font
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/format/font
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9eca8-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9eca8-118">Optional query parameters</span></span>
<span data-ttu-id="9eca8-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9eca8-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9eca8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9eca8-120">Request headers</span></span>
| <span data-ttu-id="9eca8-121">Имя</span><span class="sxs-lookup"><span data-stu-id="9eca8-121">Name</span></span>      |<span data-ttu-id="9eca8-122">Описание</span><span class="sxs-lookup"><span data-stu-id="9eca8-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9eca8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9eca8-123">Authorization</span></span>  | <span data-ttu-id="9eca8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9eca8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9eca8-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9eca8-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="9eca8-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="9eca8-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9eca8-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9eca8-129">Request body</span></span>
<span data-ttu-id="9eca8-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9eca8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9eca8-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="9eca8-131">Response</span></span>

<span data-ttu-id="9eca8-132">В случае успеха этот метод возвращает код отклика и объект `200 OK` [WorkbookChartFont](../resources/chartfont.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9eca8-132">If successful, this method returns a `200 OK` response code and [WorkbookChartFont](../resources/chartfont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9eca8-133">Пример</span><span class="sxs-lookup"><span data-stu-id="9eca8-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9eca8-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="9eca8-134">Request</span></span>
<span data-ttu-id="9eca8-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9eca8-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9eca8-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="9eca8-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chartfont"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/format/font
```
# <a name="c"></a>[<span data-ttu-id="9eca8-137">C#</span><span class="sxs-lookup"><span data-stu-id="9eca8-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chartfont-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9eca8-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9eca8-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chartfont-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9eca8-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9eca8-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chartfont-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9eca8-140">Java</span><span class="sxs-lookup"><span data-stu-id="9eca8-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chartfont-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9eca8-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="9eca8-141">Response</span></span>
<span data-ttu-id="9eca8-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9eca8-142">Here is an example of the response.</span></span> <span data-ttu-id="9eca8-143">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9eca8-143">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartFont"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "bold": true,
  "color": "color-value",
  "italic": true,
  "name": "name-value",
  "size": 99,
  "underline": "underline-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get ChartFont",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
