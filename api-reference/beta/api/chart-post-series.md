---
title: Создание объекта ChartSeries
description: С помощью этого API можно создать объект ChartSeries.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 2a528321a9b6cb1ffd40065d28122e44ae4a73a6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47983193"
---
# <a name="create-chartseries"></a><span data-ttu-id="c6157-103">Создание объекта ChartSeries</span><span class="sxs-lookup"><span data-stu-id="c6157-103">Create ChartSeries</span></span>

<span data-ttu-id="c6157-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6157-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6157-105">С помощью этого API можно создать объект ChartSeries.</span><span class="sxs-lookup"><span data-stu-id="c6157-105">Use this API to create a new ChartSeries.</span></span>
## <a name="permissions"></a><span data-ttu-id="c6157-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c6157-106">Permissions</span></span>
<span data-ttu-id="c6157-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6157-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6157-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c6157-109">Permission type</span></span>      | <span data-ttu-id="c6157-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c6157-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6157-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c6157-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c6157-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6157-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c6157-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c6157-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6157-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6157-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c6157-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c6157-115">Application</span></span> | <span data-ttu-id="c6157-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6157-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c6157-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c6157-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/series

```
## <a name="request-headers"></a><span data-ttu-id="c6157-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c6157-118">Request headers</span></span>
| <span data-ttu-id="c6157-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c6157-119">Name</span></span>       | <span data-ttu-id="c6157-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c6157-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c6157-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c6157-121">Authorization</span></span>  | <span data-ttu-id="c6157-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c6157-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c6157-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c6157-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="c6157-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="c6157-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6157-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c6157-127">Request body</span></span>
<span data-ttu-id="c6157-128">В тексте запроса добавьте представление объекта [воркбукчартсериес](../resources/workbookchartseries.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c6157-128">In the request body, supply a JSON representation of [workbookChartSeries](../resources/workbookchartseries.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c6157-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6157-129">Response</span></span>

<span data-ttu-id="c6157-130">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [воркбукчартсериес](../resources/workbookchartseries.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c6157-130">If successful, this method returns `201 Created` response code and [workbookChartSeries](../resources/workbookchartseries.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6157-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c6157-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c6157-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c6157-132">Request</span></span>
<span data-ttu-id="c6157-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c6157-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c6157-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c6157-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_chartseries_from_chart"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```
# <a name="c"></a>[<span data-ttu-id="c6157-135">C#</span><span class="sxs-lookup"><span data-stu-id="c6157-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chartseries-from-chart-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c6157-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c6157-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chartseries-from-chart-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c6157-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c6157-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chartseries-from-chart-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="c6157-138">В тексте запроса добавьте представление объекта [воркбукчартсериес](../resources/workbookchartseries.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c6157-138">In the request body, supply a JSON representation of [workbookChartSeries](../resources/workbookchartseries.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="c6157-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6157-139">Response</span></span>
<span data-ttu-id="c6157-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c6157-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create ChartSeries",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


