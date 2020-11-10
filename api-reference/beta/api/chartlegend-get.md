---
title: Получение объекта ChartLegend
description: Получение свойств и связей объекта chartlegend.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 29ef946c579eca517976176a5efcf8f764028bcb
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48958661"
---
# <a name="get-chartlegend"></a><span data-ttu-id="f85e2-103">Получение объекта ChartLegend</span><span class="sxs-lookup"><span data-stu-id="f85e2-103">Get ChartLegend</span></span>

<span data-ttu-id="f85e2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f85e2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f85e2-105">Получение свойств и связей объекта chartlegend.</span><span class="sxs-lookup"><span data-stu-id="f85e2-105">Retrieve the properties and relationships of chartlegend object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f85e2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f85e2-106">Permissions</span></span>
<span data-ttu-id="f85e2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f85e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f85e2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f85e2-109">Permission type</span></span>      | <span data-ttu-id="f85e2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f85e2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f85e2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f85e2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f85e2-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f85e2-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f85e2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f85e2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f85e2-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f85e2-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f85e2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f85e2-115">Application</span></span> | <span data-ttu-id="f85e2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f85e2-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f85e2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f85e2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/legend
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f85e2-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f85e2-118">Optional query parameters</span></span>
<span data-ttu-id="f85e2-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f85e2-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f85e2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f85e2-120">Request headers</span></span>
| <span data-ttu-id="f85e2-121">Имя</span><span class="sxs-lookup"><span data-stu-id="f85e2-121">Name</span></span>      |<span data-ttu-id="f85e2-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f85e2-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f85e2-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f85e2-123">Authorization</span></span>  | <span data-ttu-id="f85e2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f85e2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f85e2-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f85e2-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="f85e2-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="f85e2-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f85e2-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f85e2-129">Request body</span></span>
<span data-ttu-id="f85e2-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f85e2-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f85e2-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="f85e2-131">Response</span></span>

<span data-ttu-id="f85e2-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [воркбукчартлеженд](../resources/workbookchartlegend.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f85e2-132">If successful, this method returns a `200 OK` response code and [workbookChartLegend](../resources/workbookchartlegend.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f85e2-133">Пример</span><span class="sxs-lookup"><span data-stu-id="f85e2-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f85e2-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="f85e2-134">Request</span></span>
<span data-ttu-id="f85e2-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f85e2-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f85e2-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="f85e2-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chartlegend"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/legend
```
# <a name="c"></a>[<span data-ttu-id="f85e2-137">C#</span><span class="sxs-lookup"><span data-stu-id="f85e2-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chartlegend-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f85e2-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f85e2-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chartlegend-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f85e2-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f85e2-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chartlegend-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f85e2-140">Java</span><span class="sxs-lookup"><span data-stu-id="f85e2-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chartlegend-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f85e2-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="f85e2-141">Response</span></span>
<span data-ttu-id="f85e2-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f85e2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
