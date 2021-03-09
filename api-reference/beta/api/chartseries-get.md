---
title: Получение объекта ChartSeries
description: Получение свойств и связей объекта chartseries.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 51ce0085e4c873ecf551468b7c1780dbbc1dbf6b
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50574431"
---
# <a name="get-chartseries"></a><span data-ttu-id="d6e23-103">Получение объекта ChartSeries</span><span class="sxs-lookup"><span data-stu-id="d6e23-103">Get ChartSeries</span></span>

<span data-ttu-id="d6e23-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6e23-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6e23-105">Получение свойств и связей объекта chartseries.</span><span class="sxs-lookup"><span data-stu-id="d6e23-105">Retrieve the properties and relationships of chartseries object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d6e23-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d6e23-106">Permissions</span></span>
<span data-ttu-id="d6e23-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6e23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6e23-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d6e23-109">Permission type</span></span>      | <span data-ttu-id="d6e23-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d6e23-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6e23-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d6e23-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d6e23-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d6e23-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d6e23-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d6e23-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6e23-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d6e23-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d6e23-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d6e23-115">Application</span></span> | <span data-ttu-id="d6e23-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6e23-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d6e23-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d6e23-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{undefined}
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/series/{undefined}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d6e23-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d6e23-118">Optional query parameters</span></span>
<span data-ttu-id="d6e23-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d6e23-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d6e23-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d6e23-120">Request headers</span></span>
| <span data-ttu-id="d6e23-121">Имя</span><span class="sxs-lookup"><span data-stu-id="d6e23-121">Name</span></span>      |<span data-ttu-id="d6e23-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d6e23-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d6e23-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d6e23-123">Authorization</span></span>  | <span data-ttu-id="d6e23-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d6e23-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d6e23-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d6e23-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="d6e23-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="d6e23-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6e23-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d6e23-129">Request body</span></span>
<span data-ttu-id="d6e23-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d6e23-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6e23-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6e23-131">Response</span></span>

<span data-ttu-id="d6e23-132">В случае успешной работы этот метод возвращает код отклика и объект `200 OK` [книгиChartSeries](../resources/workbookchartseries.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d6e23-132">If successful, this method returns a `200 OK` response code and [workbookChartSeries](../resources/workbookchartseries.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d6e23-133">Пример</span><span class="sxs-lookup"><span data-stu-id="d6e23-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d6e23-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="d6e23-134">Request</span></span>
<span data-ttu-id="d6e23-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d6e23-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d6e23-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="d6e23-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chartseries"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{undefined}
```
# <a name="c"></a>[<span data-ttu-id="d6e23-137">C#</span><span class="sxs-lookup"><span data-stu-id="d6e23-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chartseries-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d6e23-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d6e23-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chartseries-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d6e23-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d6e23-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chartseries-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d6e23-140">Java</span><span class="sxs-lookup"><span data-stu-id="d6e23-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chartseries-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d6e23-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6e23-141">Response</span></span>
<span data-ttu-id="d6e23-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d6e23-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartSeries"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get ChartSeries",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
