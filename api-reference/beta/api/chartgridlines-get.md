---
title: Получение объекта ChartGridlines
description: Получение свойств и связей объекта chartgridlines.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: af80033c52323023bfdefd35d62f3e6a7820b0ed
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50574547"
---
# <a name="get-chartgridlines"></a><span data-ttu-id="58775-103">Получение объекта ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="58775-103">Get ChartGridlines</span></span>

<span data-ttu-id="58775-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58775-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58775-105">Получение свойств и связей объекта chartgridlines.</span><span class="sxs-lookup"><span data-stu-id="58775-105">Retrieve the properties and relationships of chartgridlines object.</span></span>
## <a name="permissions"></a><span data-ttu-id="58775-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="58775-106">Permissions</span></span>
<span data-ttu-id="58775-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58775-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58775-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="58775-109">Permission type</span></span>      | <span data-ttu-id="58775-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="58775-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="58775-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="58775-111">Delegated (work or school account)</span></span> | <span data-ttu-id="58775-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="58775-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="58775-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="58775-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58775-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="58775-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="58775-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="58775-115">Application</span></span> | <span data-ttu-id="58775-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58775-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="58775-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="58775-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/minorgridlines
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/minorgridlines
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/majorgridlines
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/majorgridlines
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/majorgridlines
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/majorgridlines
```
## <a name="optional-query-parameters"></a><span data-ttu-id="58775-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="58775-118">Optional query parameters</span></span>
<span data-ttu-id="58775-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="58775-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="58775-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="58775-120">Request headers</span></span>
| <span data-ttu-id="58775-121">Имя</span><span class="sxs-lookup"><span data-stu-id="58775-121">Name</span></span>      |<span data-ttu-id="58775-122">Описание</span><span class="sxs-lookup"><span data-stu-id="58775-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="58775-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="58775-123">Authorization</span></span>  | <span data-ttu-id="58775-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="58775-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="58775-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="58775-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="58775-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="58775-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="58775-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="58775-129">Request body</span></span>
<span data-ttu-id="58775-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="58775-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="58775-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="58775-131">Response</span></span>

<span data-ttu-id="58775-132">В случае успешной работы этот метод возвращает код отклика и объект `200 OK` [книгиChartGridlines](../resources/workbookchartgridlines.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="58775-132">If successful, this method returns a `200 OK` response code and [workbookChartGridlines](../resources/workbookchartgridlines.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="58775-133">Пример</span><span class="sxs-lookup"><span data-stu-id="58775-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="58775-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="58775-134">Request</span></span>
<span data-ttu-id="58775-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="58775-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="58775-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="58775-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chartgridlines"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/minorgridlines
```
# <a name="c"></a>[<span data-ttu-id="58775-137">C#</span><span class="sxs-lookup"><span data-stu-id="58775-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chartgridlines-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="58775-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="58775-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chartgridlines-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="58775-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="58775-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chartgridlines-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="58775-140">Java</span><span class="sxs-lookup"><span data-stu-id="58775-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chartgridlines-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="58775-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="58775-141">Response</span></span>
<span data-ttu-id="58775-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="58775-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartGridlines"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 21

{
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get ChartGridlines",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
