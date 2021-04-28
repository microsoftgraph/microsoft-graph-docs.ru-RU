---
title: 'ChartCollection: add'
description: Создает диаграмму.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: a2550ba3c86ea7c714bd7eaa6526e2a96ca3e236
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053274"
---
# <a name="chartcollection-add"></a><span data-ttu-id="dd6f0-103">ChartCollection: add</span><span class="sxs-lookup"><span data-stu-id="dd6f0-103">ChartCollection: add</span></span>

<span data-ttu-id="dd6f0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd6f0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dd6f0-105">Создает диаграмму.</span><span class="sxs-lookup"><span data-stu-id="dd6f0-105">Creates a new chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="dd6f0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dd6f0-106">Permissions</span></span>
<span data-ttu-id="dd6f0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd6f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd6f0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd6f0-109">Permission type</span></span>      | <span data-ttu-id="dd6f0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd6f0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd6f0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd6f0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dd6f0-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd6f0-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dd6f0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd6f0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd6f0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd6f0-114">Not supported.</span></span>    |
|<span data-ttu-id="dd6f0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dd6f0-115">Application</span></span> | <span data-ttu-id="dd6f0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd6f0-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd6f0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd6f0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/add
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/add

```
## <a name="request-headers"></a><span data-ttu-id="dd6f0-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dd6f0-118">Request headers</span></span>
| <span data-ttu-id="dd6f0-119">Имя</span><span class="sxs-lookup"><span data-stu-id="dd6f0-119">Name</span></span>       | <span data-ttu-id="dd6f0-120">Описание</span><span class="sxs-lookup"><span data-stu-id="dd6f0-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="dd6f0-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dd6f0-121">Authorization</span></span>  | <span data-ttu-id="dd6f0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd6f0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dd6f0-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="dd6f0-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="dd6f0-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="dd6f0-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd6f0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dd6f0-127">Request body</span></span>
<span data-ttu-id="dd6f0-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="dd6f0-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="dd6f0-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="dd6f0-129">Parameter</span></span>    | <span data-ttu-id="dd6f0-130">Тип</span><span class="sxs-lookup"><span data-stu-id="dd6f0-130">Type</span></span>   |<span data-ttu-id="dd6f0-131">Описание</span><span class="sxs-lookup"><span data-stu-id="dd6f0-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dd6f0-132">type</span><span class="sxs-lookup"><span data-stu-id="dd6f0-132">type</span></span>|<span data-ttu-id="dd6f0-133">string</span><span class="sxs-lookup"><span data-stu-id="dd6f0-133">string</span></span>|<span data-ttu-id="dd6f0-134">Представляет тип диаграммы.</span><span class="sxs-lookup"><span data-stu-id="dd6f0-134">Represents the type of a chart.</span></span>  <span data-ttu-id="dd6f0-135">Возможные значения: `ColumnClustered` , , , , , , , , `ColumnStacked` `ColumnStacked100` `BarClustered` `BarStacked` `BarStacked100` `LineStacked` `LineStacked100` `LineMarkers` `LineMarkersStacked` `LineMarkersStacked100` `PieOfPie` `etc.` .</span><span class="sxs-lookup"><span data-stu-id="dd6f0-135">The possible values are: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie`, `etc.`.</span></span>|
|<span data-ttu-id="dd6f0-136">sourceData</span><span class="sxs-lookup"><span data-stu-id="dd6f0-136">sourceData</span></span>|<span data-ttu-id="dd6f0-137">Json</span><span class="sxs-lookup"><span data-stu-id="dd6f0-137">Json</span></span>|<span data-ttu-id="dd6f0-138">Объект Range, соответствующий исходным данным.</span><span class="sxs-lookup"><span data-stu-id="dd6f0-138">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="dd6f0-139">seriesBy</span><span class="sxs-lookup"><span data-stu-id="dd6f0-139">seriesBy</span></span>|<span data-ttu-id="dd6f0-140">string</span><span class="sxs-lookup"><span data-stu-id="dd6f0-140">string</span></span>|<span data-ttu-id="dd6f0-141">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="dd6f0-141">Optional.</span></span> <span data-ttu-id="dd6f0-142">Определяет способ использования столбцов или строк в качестве рядов данных на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="dd6f0-142">Specifies the way columns or rows are used as data series on the chart.</span></span>  <span data-ttu-id="dd6f0-143">Допустимые значения: `Auto`, `Columns`, `Rows`.</span><span class="sxs-lookup"><span data-stu-id="dd6f0-143">The possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="dd6f0-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd6f0-144">Response</span></span>

<span data-ttu-id="dd6f0-145">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект WorkbookChart](../resources/chart.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="dd6f0-145">If successful, this method returns `200 OK` response code and [WorkbookChart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd6f0-146">Пример</span><span class="sxs-lookup"><span data-stu-id="dd6f0-146">Example</span></span>
<span data-ttu-id="dd6f0-147">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="dd6f0-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="dd6f0-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd6f0-148">Request</span></span>
<span data-ttu-id="dd6f0-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dd6f0-149">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dd6f0-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="dd6f0-150">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="dd6f0-151">C#</span><span class="sxs-lookup"><span data-stu-id="dd6f0-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chartcollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dd6f0-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dd6f0-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chartcollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dd6f0-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dd6f0-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chartcollection-add-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dd6f0-154">Java</span><span class="sxs-lookup"><span data-stu-id="dd6f0-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chartcollection-add-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="dd6f0-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd6f0-155">Response</span></span>
<span data-ttu-id="dd6f0-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dd6f0-156">Here is an example of the response.</span></span> <span data-ttu-id="dd6f0-157">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="dd6f0-157">Note: The response object shown here might be shortened for readability.</span></span>
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

