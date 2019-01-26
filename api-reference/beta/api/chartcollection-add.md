---
title: 'ChartCollection: add'
description: Создает диаграмму.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: f552e4d8f0c8dc9f1257baf02ebe7a449c98a348
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572117"
---
# <a name="chartcollection-add"></a><span data-ttu-id="bbc48-103">ChartCollection: add</span><span class="sxs-lookup"><span data-stu-id="bbc48-103">ChartCollection: add</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bbc48-104">Создает диаграмму.</span><span class="sxs-lookup"><span data-stu-id="bbc48-104">Creates a new chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="bbc48-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bbc48-105">Permissions</span></span>
<span data-ttu-id="bbc48-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bbc48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bbc48-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bbc48-108">Permission type</span></span>      | <span data-ttu-id="bbc48-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bbc48-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bbc48-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bbc48-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bbc48-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bbc48-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bbc48-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bbc48-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bbc48-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bbc48-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bbc48-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bbc48-114">Application</span></span> | <span data-ttu-id="bbc48-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bbc48-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bbc48-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bbc48-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/add

```
## <a name="request-headers"></a><span data-ttu-id="bbc48-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bbc48-117">Request headers</span></span>
| <span data-ttu-id="bbc48-118">Имя</span><span class="sxs-lookup"><span data-stu-id="bbc48-118">Name</span></span>       | <span data-ttu-id="bbc48-119">Описание</span><span class="sxs-lookup"><span data-stu-id="bbc48-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bbc48-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bbc48-120">Authorization</span></span>  | <span data-ttu-id="bbc48-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bbc48-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bbc48-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="bbc48-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="bbc48-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="bbc48-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bbc48-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bbc48-126">Request body</span></span>
<span data-ttu-id="bbc48-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="bbc48-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="bbc48-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="bbc48-128">Parameter</span></span>    | <span data-ttu-id="bbc48-129">Тип</span><span class="sxs-lookup"><span data-stu-id="bbc48-129">Type</span></span>   |<span data-ttu-id="bbc48-130">Описание</span><span class="sxs-lookup"><span data-stu-id="bbc48-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bbc48-131">type</span><span class="sxs-lookup"><span data-stu-id="bbc48-131">type</span></span>|<span data-ttu-id="bbc48-132">строка</span><span class="sxs-lookup"><span data-stu-id="bbc48-132">string</span></span>|<span data-ttu-id="bbc48-133">Представляет тип диаграммы.</span><span class="sxs-lookup"><span data-stu-id="bbc48-133">Represents the type of a chart.</span></span>  <span data-ttu-id="bbc48-134">Возможные значения: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie`, `etc.`.</span><span class="sxs-lookup"><span data-stu-id="bbc48-134">The possible values are: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie`, `etc.`.</span></span>|
|<span data-ttu-id="bbc48-135">sourceData</span><span class="sxs-lookup"><span data-stu-id="bbc48-135">sourceData</span></span>|<span data-ttu-id="bbc48-136">Json</span><span class="sxs-lookup"><span data-stu-id="bbc48-136">Json</span></span>|<span data-ttu-id="bbc48-137">Объект Range, соответствующий исходным данным.</span><span class="sxs-lookup"><span data-stu-id="bbc48-137">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="bbc48-138">seriesBy</span><span class="sxs-lookup"><span data-stu-id="bbc48-138">seriesBy</span></span>|<span data-ttu-id="bbc48-139">string</span><span class="sxs-lookup"><span data-stu-id="bbc48-139">string</span></span>|<span data-ttu-id="bbc48-140">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="bbc48-140">Optional.</span></span> <span data-ttu-id="bbc48-141">Указывает, что способ столбцы или строки используются в качестве рядов данных на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="bbc48-141">Specifies the way columns or rows are used as data series on the chart.</span></span>  <span data-ttu-id="bbc48-142">Возможные значения: `Auto`, `Columns`, `Rows`.</span><span class="sxs-lookup"><span data-stu-id="bbc48-142">The possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="bbc48-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="bbc48-143">Response</span></span>

<span data-ttu-id="bbc48-144">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [WorkbookChart](../resources/chart.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="bbc48-144">If successful, this method returns `200 OK` response code and [WorkbookChart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bbc48-145">Пример</span><span class="sxs-lookup"><span data-stu-id="bbc48-145">Example</span></span>
<span data-ttu-id="bbc48-146">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="bbc48-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="bbc48-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="bbc48-147">Request</span></span>
<span data-ttu-id="bbc48-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bbc48-148">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="bbc48-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="bbc48-149">Response</span></span>
<span data-ttu-id="bbc48-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="bbc48-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/chartcollection-add.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
