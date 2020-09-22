---
title: Получение объекта ChartLegend
description: Получение свойств и связей объекта chartlegend.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 727150f41bd9218ec65e19d4a529caa63dd9eb26
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47982943"
---
# <a name="get-chartlegend"></a><span data-ttu-id="d88b1-103">Получение объекта ChartLegend</span><span class="sxs-lookup"><span data-stu-id="d88b1-103">Get ChartLegend</span></span>

<span data-ttu-id="d88b1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d88b1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d88b1-105">Получение свойств и связей объекта chartlegend.</span><span class="sxs-lookup"><span data-stu-id="d88b1-105">Retrieve the properties and relationships of chartlegend object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d88b1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d88b1-106">Permissions</span></span>
<span data-ttu-id="d88b1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d88b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d88b1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d88b1-109">Permission type</span></span>      | <span data-ttu-id="d88b1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d88b1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d88b1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d88b1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d88b1-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d88b1-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d88b1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d88b1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d88b1-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d88b1-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d88b1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d88b1-115">Application</span></span> | <span data-ttu-id="d88b1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d88b1-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d88b1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d88b1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/legend
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d88b1-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d88b1-118">Optional query parameters</span></span>
<span data-ttu-id="d88b1-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d88b1-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d88b1-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d88b1-120">Request headers</span></span>
| <span data-ttu-id="d88b1-121">Имя</span><span class="sxs-lookup"><span data-stu-id="d88b1-121">Name</span></span>      |<span data-ttu-id="d88b1-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d88b1-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d88b1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d88b1-123">Authorization</span></span>  | <span data-ttu-id="d88b1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d88b1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d88b1-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d88b1-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="d88b1-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="d88b1-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d88b1-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d88b1-129">Request body</span></span>
<span data-ttu-id="d88b1-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d88b1-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d88b1-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="d88b1-131">Response</span></span>

<span data-ttu-id="d88b1-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [воркбукчартлеженд](../resources/workbookchartlegend.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d88b1-132">If successful, this method returns a `200 OK` response code and [workbookChartLegend](../resources/workbookchartlegend.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d88b1-133">Пример</span><span class="sxs-lookup"><span data-stu-id="d88b1-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d88b1-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="d88b1-134">Request</span></span>
<span data-ttu-id="d88b1-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d88b1-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d88b1-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="d88b1-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chartlegend"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/legend
```
# <a name="c"></a>[<span data-ttu-id="d88b1-137">C#</span><span class="sxs-lookup"><span data-stu-id="d88b1-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chartlegend-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d88b1-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d88b1-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chartlegend-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d88b1-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d88b1-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chartlegend-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d88b1-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="d88b1-140">Response</span></span>
<span data-ttu-id="d88b1-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d88b1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartLegend"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "visible": true,
  "position": "position-value",
  "overlay": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get ChartLegend",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


