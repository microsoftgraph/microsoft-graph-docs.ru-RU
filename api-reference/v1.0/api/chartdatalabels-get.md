---
title: Получение объекта ChartDataLabels
description: Получение свойств и связей объекта chartdatalabels.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 8ef4ba28dcb1421c714015639bfb36643902cd17
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36003625"
---
# <a name="get-chartdatalabels"></a><span data-ttu-id="9f1c5-103">Получение объекта ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="9f1c5-103">Get ChartDataLabels</span></span>

<span data-ttu-id="9f1c5-104">Получение свойств и связей объекта chartdatalabels.</span><span class="sxs-lookup"><span data-stu-id="9f1c5-104">Retrieve the properties and relationships of chartdatalabels object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9f1c5-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9f1c5-105">Permissions</span></span>
<span data-ttu-id="9f1c5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f1c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f1c5-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f1c5-108">Permission type</span></span>      | <span data-ttu-id="9f1c5-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f1c5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f1c5-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f1c5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9f1c5-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9f1c5-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9f1c5-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f1c5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f1c5-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f1c5-113">Not supported.</span></span>    |
|<span data-ttu-id="9f1c5-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9f1c5-114">Application</span></span> | <span data-ttu-id="9f1c5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f1c5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f1c5-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f1c5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/dataLabels
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9f1c5-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9f1c5-117">Optional query parameters</span></span>
<span data-ttu-id="9f1c5-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9f1c5-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9f1c5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9f1c5-119">Request headers</span></span>
| <span data-ttu-id="9f1c5-120">Имя</span><span class="sxs-lookup"><span data-stu-id="9f1c5-120">Name</span></span>      |<span data-ttu-id="9f1c5-121">Описание</span><span class="sxs-lookup"><span data-stu-id="9f1c5-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9f1c5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9f1c5-122">Authorization</span></span>  | <span data-ttu-id="9f1c5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f1c5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9f1c5-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9f1c5-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="9f1c5-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="9f1c5-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f1c5-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9f1c5-128">Request body</span></span>
<span data-ttu-id="9f1c5-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9f1c5-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f1c5-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f1c5-130">Response</span></span>

<span data-ttu-id="9f1c5-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [воркбукчартдаталабелс](../resources/chartdatalabels.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9f1c5-131">If successful, this method returns a `200 OK` response code and [WorkbookChartDataLabels](../resources/chartdatalabels.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9f1c5-132">Пример</span><span class="sxs-lookup"><span data-stu-id="9f1c5-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9f1c5-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f1c5-133">Request</span></span>
<span data-ttu-id="9f1c5-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f1c5-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9f1c5-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="9f1c5-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chartdatalabels"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/dataLabels
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9f1c5-136">C#</span><span class="sxs-lookup"><span data-stu-id="9f1c5-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chartdatalabels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9f1c5-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="9f1c5-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chartdatalabels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9f1c5-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="9f1c5-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chartdatalabels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9f1c5-139">Java</span><span class="sxs-lookup"><span data-stu-id="9f1c5-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chartdatalabels-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9f1c5-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f1c5-140">Response</span></span>
<span data-ttu-id="9f1c5-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9f1c5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartDataLabels"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "position": "position-value",
  "showValue": true,
  "showSeriesName": true,
  "showCategoryName": true,
  "showLegendKey": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get ChartDataLabels",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
