---
title: Создание объекта ChartSeries
description: С помощью этого API можно создать объект ChartSeries.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 8a30801e31f8940efd318095fe70d6e3a2685e20
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35261973"
---
# <a name="create-chartseries"></a><span data-ttu-id="93afa-103">Создание объекта ChartSeries</span><span class="sxs-lookup"><span data-stu-id="93afa-103">Create ChartSeries</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93afa-104">С помощью этого API можно создать объект ChartSeries.</span><span class="sxs-lookup"><span data-stu-id="93afa-104">Use this API to create a new ChartSeries.</span></span>
## <a name="permissions"></a><span data-ttu-id="93afa-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="93afa-105">Permissions</span></span>
<span data-ttu-id="93afa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93afa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93afa-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="93afa-108">Permission type</span></span>      | <span data-ttu-id="93afa-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="93afa-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="93afa-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="93afa-110">Delegated (work or school account)</span></span> | <span data-ttu-id="93afa-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="93afa-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="93afa-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="93afa-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93afa-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="93afa-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="93afa-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="93afa-114">Application</span></span> | <span data-ttu-id="93afa-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93afa-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="93afa-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="93afa-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/series

```
## <a name="request-headers"></a><span data-ttu-id="93afa-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="93afa-117">Request headers</span></span>
| <span data-ttu-id="93afa-118">Имя</span><span class="sxs-lookup"><span data-stu-id="93afa-118">Name</span></span>       | <span data-ttu-id="93afa-119">Описание</span><span class="sxs-lookup"><span data-stu-id="93afa-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="93afa-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="93afa-120">Authorization</span></span>  | <span data-ttu-id="93afa-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="93afa-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="93afa-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="93afa-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="93afa-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="93afa-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="93afa-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="93afa-126">Request body</span></span>
<span data-ttu-id="93afa-127">В тексте запроса добавьте представление объекта [воркбукчартсериес](../resources/workbookchartseries.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="93afa-127">In the request body, supply a JSON representation of [workbookChartSeries](../resources/workbookchartseries.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="93afa-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="93afa-128">Response</span></span>

<span data-ttu-id="93afa-129">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [воркбукчартсериес](../resources/workbookchartseries.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="93afa-129">If successful, this method returns `201 Created` response code and [workbookChartSeries](../resources/workbookchartseries.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93afa-130">Пример</span><span class="sxs-lookup"><span data-stu-id="93afa-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="93afa-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="93afa-131">Request</span></span>
<span data-ttu-id="93afa-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="93afa-132">Here is an example of the request.</span></span>
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
<span data-ttu-id="93afa-133">В тексте запроса добавьте представление объекта [воркбукчартсериес](../resources/workbookchartseries.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="93afa-133">In the request body, supply a JSON representation of [workbookChartSeries](../resources/workbookchartseries.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="93afa-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="93afa-134">Response</span></span>
<span data-ttu-id="93afa-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="93afa-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="93afa-138">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="93afa-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="93afa-139">C#</span><span class="sxs-lookup"><span data-stu-id="93afa-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_chartseries_from_chart-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="93afa-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="93afa-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_chartseries_from_chart-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="93afa-141">Цель — C</span><span class="sxs-lookup"><span data-stu-id="93afa-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_chartseries_from_chart-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/chart-post-series.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/chart-post-series.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/chart-post-series.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
