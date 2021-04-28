---
title: Создание объекта ChartSeries
description: С помощью этого API можно создать объект ChartSeries.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 9468a415a02409a17862cec4486eee8156973e1b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053288"
---
# <a name="create-chartseries"></a><span data-ttu-id="d3f77-103">Создание объекта ChartSeries</span><span class="sxs-lookup"><span data-stu-id="d3f77-103">Create ChartSeries</span></span>

<span data-ttu-id="d3f77-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3f77-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d3f77-105">С помощью этого API можно создать объект ChartSeries.</span><span class="sxs-lookup"><span data-stu-id="d3f77-105">Use this API to create a new ChartSeries.</span></span>
## <a name="permissions"></a><span data-ttu-id="d3f77-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d3f77-106">Permissions</span></span>
<span data-ttu-id="d3f77-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3f77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3f77-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d3f77-109">Permission type</span></span>      | <span data-ttu-id="d3f77-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d3f77-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d3f77-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d3f77-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d3f77-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d3f77-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d3f77-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d3f77-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3f77-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3f77-114">Not supported.</span></span>    |
|<span data-ttu-id="d3f77-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d3f77-115">Application</span></span> | <span data-ttu-id="d3f77-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3f77-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d3f77-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d3f77-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/series

```
## <a name="request-headers"></a><span data-ttu-id="d3f77-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d3f77-118">Request headers</span></span>
| <span data-ttu-id="d3f77-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d3f77-119">Name</span></span>       | <span data-ttu-id="d3f77-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d3f77-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d3f77-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d3f77-121">Authorization</span></span>  | <span data-ttu-id="d3f77-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d3f77-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d3f77-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d3f77-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="d3f77-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="d3f77-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3f77-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d3f77-127">Request body</span></span>
<span data-ttu-id="d3f77-128">В корпусе запроса поставляем JSON-представление объекта [WorkbookChartSeries.](../resources/chartseries.md)</span><span class="sxs-lookup"><span data-stu-id="d3f77-128">In the request body, supply a JSON representation of [WorkbookChartSeries](../resources/chartseries.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d3f77-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3f77-129">Response</span></span>

<span data-ttu-id="d3f77-130">В случае успеха этот метод возвращает код ответа и `201 Created` [объект WorkbookChartSeries](../resources/chartseries.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d3f77-130">If successful, this method returns `201 Created` response code and [WorkbookChartSeries](../resources/chartseries.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3f77-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d3f77-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d3f77-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d3f77-132">Request</span></span>
<span data-ttu-id="d3f77-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d3f77-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d3f77-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="d3f77-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_chartseries_from_chart"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```
# <a name="c"></a>[<span data-ttu-id="d3f77-135">C#</span><span class="sxs-lookup"><span data-stu-id="d3f77-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chartseries-from-chart-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d3f77-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d3f77-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chartseries-from-chart-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d3f77-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d3f77-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chartseries-from-chart-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d3f77-138">Java</span><span class="sxs-lookup"><span data-stu-id="d3f77-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-chartseries-from-chart-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="d3f77-139">В корпусе запроса поставляем JSON-представление объекта [WorkbookChartSeries.](../resources/chartseries.md)</span><span class="sxs-lookup"><span data-stu-id="d3f77-139">In the request body, supply a JSON representation of [WorkbookChartSeries](../resources/chartseries.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="d3f77-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3f77-140">Response</span></span>
<span data-ttu-id="d3f77-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d3f77-141">Here is an example of the response.</span></span> <span data-ttu-id="d3f77-142">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d3f77-142">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartSeries"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create ChartSeries",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

