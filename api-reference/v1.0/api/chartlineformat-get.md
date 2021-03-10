---
title: Получение объекта ChartLineFormat
description: Получение свойств и связей объекта chartlineformat.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 7cd60485547e88a936456498d88019d86625c05d
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50577802"
---
# <a name="get-chartlineformat"></a><span data-ttu-id="bcbce-103">Получение объекта ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="bcbce-103">Get ChartLineFormat</span></span>

<span data-ttu-id="bcbce-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bcbce-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bcbce-105">Получение свойств и связей объекта chartlineformat.</span><span class="sxs-lookup"><span data-stu-id="bcbce-105">Retrieve the properties and relationships of chartlineformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="bcbce-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bcbce-106">Permissions</span></span>
<span data-ttu-id="bcbce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bcbce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bcbce-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bcbce-109">Permission type</span></span>      | <span data-ttu-id="bcbce-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bcbce-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bcbce-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bcbce-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bcbce-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bcbce-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bcbce-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bcbce-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bcbce-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bcbce-114">Not supported.</span></span>    |
|<span data-ttu-id="bcbce-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bcbce-115">Application</span></span> | <span data-ttu-id="bcbce-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bcbce-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bcbce-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bcbce-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/format/line
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/format/line
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/format/line
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/format/line
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/majorgridlines/format/line
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/majorgridlines/format/line
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bcbce-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bcbce-118">Optional query parameters</span></span>
<span data-ttu-id="bcbce-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bcbce-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bcbce-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bcbce-120">Request headers</span></span>
| <span data-ttu-id="bcbce-121">Имя</span><span class="sxs-lookup"><span data-stu-id="bcbce-121">Name</span></span>      |<span data-ttu-id="bcbce-122">Описание</span><span class="sxs-lookup"><span data-stu-id="bcbce-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bcbce-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bcbce-123">Authorization</span></span>  | <span data-ttu-id="bcbce-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bcbce-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bcbce-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="bcbce-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="bcbce-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="bcbce-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bcbce-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bcbce-129">Request body</span></span>
<span data-ttu-id="bcbce-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bcbce-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bcbce-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="bcbce-131">Response</span></span>

<span data-ttu-id="bcbce-132">В случае успешной работы этот метод возвращает код ответа и объект `200 OK` [WorkbookChartLineFormat](../resources/chartlineformat.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="bcbce-132">If successful, this method returns a `200 OK` response code and [WorkbookChartLineFormat](../resources/chartlineformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bcbce-133">Пример</span><span class="sxs-lookup"><span data-stu-id="bcbce-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bcbce-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="bcbce-134">Request</span></span>
<span data-ttu-id="bcbce-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bcbce-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bcbce-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="bcbce-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chartlineformat"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/format/line
```
# <a name="c"></a>[<span data-ttu-id="bcbce-137">C#</span><span class="sxs-lookup"><span data-stu-id="bcbce-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chartlineformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bcbce-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bcbce-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chartlineformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bcbce-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bcbce-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chartlineformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bcbce-140">Java</span><span class="sxs-lookup"><span data-stu-id="bcbce-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chartlineformat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="bcbce-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="bcbce-141">Response</span></span>
<span data-ttu-id="bcbce-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bcbce-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartLineFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get ChartLineFormat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
