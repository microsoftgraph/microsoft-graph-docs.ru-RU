---
title: 'ChartCollection: add'
description: Создает диаграмму.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 39fd7852ad57b9f618da9d7d8608fb5f09521179
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48059889"
---
# <a name="chartcollection-add"></a><span data-ttu-id="3e373-103">ChartCollection: add</span><span class="sxs-lookup"><span data-stu-id="3e373-103">ChartCollection: add</span></span>

<span data-ttu-id="3e373-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e373-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3e373-105">Создает диаграмму.</span><span class="sxs-lookup"><span data-stu-id="3e373-105">Creates a new chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="3e373-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3e373-106">Permissions</span></span>
<span data-ttu-id="3e373-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e373-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e373-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3e373-109">Permission type</span></span>      | <span data-ttu-id="3e373-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3e373-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e373-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3e373-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3e373-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3e373-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3e373-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3e373-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e373-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e373-114">Not supported.</span></span>    |
|<span data-ttu-id="3e373-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3e373-115">Application</span></span> | <span data-ttu-id="3e373-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e373-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e373-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3e373-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/add

```
## <a name="request-headers"></a><span data-ttu-id="3e373-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3e373-118">Request headers</span></span>
| <span data-ttu-id="3e373-119">Имя</span><span class="sxs-lookup"><span data-stu-id="3e373-119">Name</span></span>       | <span data-ttu-id="3e373-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3e373-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3e373-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3e373-121">Authorization</span></span>  | <span data-ttu-id="3e373-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3e373-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3e373-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3e373-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="3e373-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="3e373-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e373-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3e373-127">Request body</span></span>
<span data-ttu-id="3e373-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="3e373-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3e373-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="3e373-129">Parameter</span></span>    | <span data-ttu-id="3e373-130">Тип</span><span class="sxs-lookup"><span data-stu-id="3e373-130">Type</span></span>   |<span data-ttu-id="3e373-131">Описание</span><span class="sxs-lookup"><span data-stu-id="3e373-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3e373-132">type</span><span class="sxs-lookup"><span data-stu-id="3e373-132">type</span></span>|<span data-ttu-id="3e373-133">string</span><span class="sxs-lookup"><span data-stu-id="3e373-133">string</span></span>|<span data-ttu-id="3e373-134">Представляет тип диаграммы.</span><span class="sxs-lookup"><span data-stu-id="3e373-134">Represents the type of a chart.</span></span>  <span data-ttu-id="3e373-135">Возможные значения: `ColumnClustered` , `ColumnStacked` ,,, `ColumnStacked100` `BarClustered` `BarStacked` , `BarStacked100` , `LineStacked` , `LineStacked100` , `LineMarkers` `LineMarkersStacked` `LineMarkersStacked100` `PieOfPie` `etc.` ,,,,.</span><span class="sxs-lookup"><span data-stu-id="3e373-135">The possible values are: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie`, `etc.`.</span></span>|
|<span data-ttu-id="3e373-136">sourceData</span><span class="sxs-lookup"><span data-stu-id="3e373-136">sourceData</span></span>|<span data-ttu-id="3e373-137">Json</span><span class="sxs-lookup"><span data-stu-id="3e373-137">Json</span></span>|<span data-ttu-id="3e373-138">Объект Range, соответствующий исходным данным.</span><span class="sxs-lookup"><span data-stu-id="3e373-138">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="3e373-139">seriesBy</span><span class="sxs-lookup"><span data-stu-id="3e373-139">seriesBy</span></span>|<span data-ttu-id="3e373-140">string</span><span class="sxs-lookup"><span data-stu-id="3e373-140">string</span></span>|<span data-ttu-id="3e373-141">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="3e373-141">Optional.</span></span> <span data-ttu-id="3e373-142">Определяет способ использования столбцов или строк в качестве рядов данных на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="3e373-142">Specifies the way columns or rows are used as data series on the chart.</span></span>  <span data-ttu-id="3e373-143">Допустимые значения: `Auto`, `Columns`, `Rows`.</span><span class="sxs-lookup"><span data-stu-id="3e373-143">The possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="3e373-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e373-144">Response</span></span>

<span data-ttu-id="3e373-145">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [воркбукчарт](../resources/chart.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3e373-145">If successful, this method returns `200 OK` response code and [WorkbookChart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e373-146">Пример</span><span class="sxs-lookup"><span data-stu-id="3e373-146">Example</span></span>
<span data-ttu-id="3e373-147">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="3e373-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3e373-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e373-148">Request</span></span>
<span data-ttu-id="3e373-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3e373-149">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3e373-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="3e373-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chartcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/add
Content-type: application/json
Content-length: 94

{
  "type": "ColumnStacked",
  "sourceData": "A1:B1",
  "seriesBy": "Auto"
}
```
# <a name="c"></a>[<span data-ttu-id="3e373-151">C#</span><span class="sxs-lookup"><span data-stu-id="3e373-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chartcollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3e373-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3e373-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chartcollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3e373-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3e373-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chartcollection-add-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3e373-154">Java</span><span class="sxs-lookup"><span data-stu-id="3e373-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chartcollection-add-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3e373-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e373-155">Response</span></span>
<span data-ttu-id="3e373-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3e373-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "ChartCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

