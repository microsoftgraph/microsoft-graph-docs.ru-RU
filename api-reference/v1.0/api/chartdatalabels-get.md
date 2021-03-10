---
title: Получение объекта ChartDataLabels
description: Получение свойств и связей объекта chartdatalabels.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 98f03a652c0b7920de81a4487a1652a9e5dec3b3
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50578461"
---
# <a name="get-chartdatalabels"></a><span data-ttu-id="e833d-103">Получение объекта ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="e833d-103">Get ChartDataLabels</span></span>

<span data-ttu-id="e833d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e833d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e833d-105">Получение свойств и связей объекта chartdatalabels.</span><span class="sxs-lookup"><span data-stu-id="e833d-105">Retrieve the properties and relationships of chartdatalabels object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e833d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e833d-106">Permissions</span></span>
<span data-ttu-id="e833d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e833d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e833d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e833d-109">Permission type</span></span>      | <span data-ttu-id="e833d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e833d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e833d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e833d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e833d-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e833d-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e833d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e833d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e833d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e833d-114">Not supported.</span></span>    |
|<span data-ttu-id="e833d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e833d-115">Application</span></span> | <span data-ttu-id="e833d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e833d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e833d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e833d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/dataLabels
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/dataLabels
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e833d-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e833d-118">Optional query parameters</span></span>
<span data-ttu-id="e833d-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e833d-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e833d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e833d-120">Request headers</span></span>
| <span data-ttu-id="e833d-121">Имя</span><span class="sxs-lookup"><span data-stu-id="e833d-121">Name</span></span>      |<span data-ttu-id="e833d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e833d-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e833d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e833d-123">Authorization</span></span>  | <span data-ttu-id="e833d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e833d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e833d-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e833d-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="e833d-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="e833d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e833d-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e833d-129">Request body</span></span>
<span data-ttu-id="e833d-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e833d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e833d-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="e833d-131">Response</span></span>

<span data-ttu-id="e833d-132">В случае успешной работы этот метод возвращает код отклика и объект `200 OK` [WorkbookChartDataLabels](../resources/chartdatalabels.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e833d-132">If successful, this method returns a `200 OK` response code and [WorkbookChartDataLabels](../resources/chartdatalabels.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e833d-133">Пример</span><span class="sxs-lookup"><span data-stu-id="e833d-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e833d-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e833d-134">Request</span></span>
<span data-ttu-id="e833d-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e833d-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e833d-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="e833d-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chartdatalabels"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/dataLabels
```
# <a name="c"></a>[<span data-ttu-id="e833d-137">C#</span><span class="sxs-lookup"><span data-stu-id="e833d-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chartdatalabels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e833d-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e833d-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chartdatalabels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e833d-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e833d-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chartdatalabels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e833d-140">Java</span><span class="sxs-lookup"><span data-stu-id="e833d-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chartdatalabels-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e833d-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="e833d-141">Response</span></span>
<span data-ttu-id="e833d-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e833d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
