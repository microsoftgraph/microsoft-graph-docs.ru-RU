---
title: 'Воркбукчартколлектион: Add'
description: Создает новый объект Воркбукчарт.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 8effe1466bf071e792106a309586a4393628ce6d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35438239"
---
# <a name="workbookchartcollection-add"></a><span data-ttu-id="733cb-103">Воркбукчартколлектион: Add</span><span class="sxs-lookup"><span data-stu-id="733cb-103">workbookChartCollection: add</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="733cb-104">Создает диаграмму.</span><span class="sxs-lookup"><span data-stu-id="733cb-104">Creates a new chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="733cb-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="733cb-105">Permissions</span></span>
<span data-ttu-id="733cb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="733cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="733cb-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="733cb-108">Permission type</span></span>      | <span data-ttu-id="733cb-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="733cb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="733cb-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="733cb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="733cb-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="733cb-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="733cb-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="733cb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="733cb-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="733cb-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="733cb-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="733cb-114">Application</span></span> | <span data-ttu-id="733cb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="733cb-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="733cb-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="733cb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/add

```
## <a name="request-headers"></a><span data-ttu-id="733cb-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="733cb-117">Request headers</span></span>
| <span data-ttu-id="733cb-118">Имя</span><span class="sxs-lookup"><span data-stu-id="733cb-118">Name</span></span>       | <span data-ttu-id="733cb-119">Описание</span><span class="sxs-lookup"><span data-stu-id="733cb-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="733cb-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="733cb-120">Authorization</span></span>  | <span data-ttu-id="733cb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="733cb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="733cb-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="733cb-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="733cb-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="733cb-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="733cb-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="733cb-126">Request body</span></span>
<span data-ttu-id="733cb-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="733cb-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="733cb-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="733cb-128">Parameter</span></span>    | <span data-ttu-id="733cb-129">Тип</span><span class="sxs-lookup"><span data-stu-id="733cb-129">Type</span></span>   |<span data-ttu-id="733cb-130">Описание</span><span class="sxs-lookup"><span data-stu-id="733cb-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="733cb-131">type</span><span class="sxs-lookup"><span data-stu-id="733cb-131">type</span></span>|<span data-ttu-id="733cb-132">string</span><span class="sxs-lookup"><span data-stu-id="733cb-132">string</span></span>|<span data-ttu-id="733cb-133">Представляет тип диаграммы.</span><span class="sxs-lookup"><span data-stu-id="733cb-133">Represents the type of a chart.</span></span>  <span data-ttu-id="733cb-134">Возможные `ColumnClustered`значения:, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers` `LineMarkersStacked` `LineMarkersStacked100`,,, `PieOfPie`,. `etc.`</span><span class="sxs-lookup"><span data-stu-id="733cb-134">The possible values are: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie`, `etc.`.</span></span>|
|<span data-ttu-id="733cb-135">sourceData</span><span class="sxs-lookup"><span data-stu-id="733cb-135">sourceData</span></span>|<span data-ttu-id="733cb-136">Json</span><span class="sxs-lookup"><span data-stu-id="733cb-136">Json</span></span>|<span data-ttu-id="733cb-137">Объект Range, соответствующий исходным данным.</span><span class="sxs-lookup"><span data-stu-id="733cb-137">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="733cb-138">seriesBy</span><span class="sxs-lookup"><span data-stu-id="733cb-138">seriesBy</span></span>|<span data-ttu-id="733cb-139">string</span><span class="sxs-lookup"><span data-stu-id="733cb-139">string</span></span>|<span data-ttu-id="733cb-140">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="733cb-140">Optional.</span></span> <span data-ttu-id="733cb-141">Определяет способ использования столбцов или строк в качестве рядов данных на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="733cb-141">Specifies the way columns or rows are used as data series on the chart.</span></span>  <span data-ttu-id="733cb-142">Допустимые значения: `Auto`, `Columns`, `Rows`.</span><span class="sxs-lookup"><span data-stu-id="733cb-142">The possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="733cb-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="733cb-143">Response</span></span>

<span data-ttu-id="733cb-144">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект [воркбукчарт](../resources/workbookchart.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="733cb-144">If successful, this method returns `200 OK` response code and [workbookChart](../resources/workbookchart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="733cb-145">Пример</span><span class="sxs-lookup"><span data-stu-id="733cb-145">Example</span></span>
<span data-ttu-id="733cb-146">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="733cb-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="733cb-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="733cb-147">Request</span></span>
<span data-ttu-id="733cb-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="733cb-148">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="733cb-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="733cb-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chartcollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/add
Content-type: application/json
Content-length: 94

{
  "type": "ColumnStacked",
  "sourceData": "A1:B1",
  "seriesBy": "Auto"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="733cb-150">C#</span><span class="sxs-lookup"><span data-stu-id="733cb-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chartcollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="733cb-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="733cb-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chartcollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="733cb-152">Цель — C</span><span class="sxs-lookup"><span data-stu-id="733cb-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chartcollection-add-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="733cb-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="733cb-153">Response</span></span>
<span data-ttu-id="733cb-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="733cb-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChart"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
