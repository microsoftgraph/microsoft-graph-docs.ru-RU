---
title: Обновление объекта chartdatalabels
description: Обновление свойств объекта chartdatalabels.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4ad66f2cbf4d78c1fd3570d9e98184370b0ef075
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35272522"
---
# <a name="update-chartdatalabels"></a><span data-ttu-id="10d16-103">Обновление объекта chartdatalabels</span><span class="sxs-lookup"><span data-stu-id="10d16-103">Update chartdatalabels</span></span>

<span data-ttu-id="10d16-104">Обновление свойств объекта chartdatalabels.</span><span class="sxs-lookup"><span data-stu-id="10d16-104">Update the properties of chartdatalabels object.</span></span>
## <a name="permissions"></a><span data-ttu-id="10d16-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="10d16-105">Permissions</span></span>
<span data-ttu-id="10d16-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10d16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10d16-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10d16-108">Permission type</span></span>      | <span data-ttu-id="10d16-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="10d16-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="10d16-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10d16-110">Delegated (work or school account)</span></span> | <span data-ttu-id="10d16-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="10d16-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="10d16-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10d16-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10d16-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10d16-113">Not supported.</span></span>    |
|<span data-ttu-id="10d16-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="10d16-114">Application</span></span> | <span data-ttu-id="10d16-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10d16-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="10d16-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10d16-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/dataLabels
```
## <a name="optional-request-headers"></a><span data-ttu-id="10d16-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10d16-117">Optional request headers</span></span>
| <span data-ttu-id="10d16-118">Имя</span><span class="sxs-lookup"><span data-stu-id="10d16-118">Name</span></span>       | <span data-ttu-id="10d16-119">Описание</span><span class="sxs-lookup"><span data-stu-id="10d16-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="10d16-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="10d16-120">Authorization</span></span>  | <span data-ttu-id="10d16-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10d16-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="10d16-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="10d16-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="10d16-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="10d16-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="10d16-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="10d16-126">Request body</span></span>
<span data-ttu-id="10d16-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="10d16-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="10d16-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="10d16-130">Property</span></span>     | <span data-ttu-id="10d16-131">Тип</span><span class="sxs-lookup"><span data-stu-id="10d16-131">Type</span></span>   |<span data-ttu-id="10d16-132">Описание</span><span class="sxs-lookup"><span data-stu-id="10d16-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="10d16-133">position</span><span class="sxs-lookup"><span data-stu-id="10d16-133">position</span></span>|<span data-ttu-id="10d16-134">string</span><span class="sxs-lookup"><span data-stu-id="10d16-134">string</span></span>|<span data-ttu-id="10d16-135">Значение DataLabelPosition, которое представляет положение метки данных.</span><span class="sxs-lookup"><span data-stu-id="10d16-135">DataLabelPosition value that represents the position of the data label.</span></span> <span data-ttu-id="10d16-136">`None`Возможные значения:, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`,. `Callout`</span><span class="sxs-lookup"><span data-stu-id="10d16-136">The possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="10d16-137">separator</span><span class="sxs-lookup"><span data-stu-id="10d16-137">separator</span></span>|<span data-ttu-id="10d16-138">string</span><span class="sxs-lookup"><span data-stu-id="10d16-138">string</span></span>|<span data-ttu-id="10d16-139">Строка, представляющая разделитель для меток данных на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="10d16-139">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="10d16-140">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="10d16-140">showBubbleSize</span></span>|<span data-ttu-id="10d16-141">boolean</span><span class="sxs-lookup"><span data-stu-id="10d16-141">boolean</span></span>|<span data-ttu-id="10d16-142">Логическое значение, которое указывает, отображается ли размер пузырьков с метками данных.</span><span class="sxs-lookup"><span data-stu-id="10d16-142">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="10d16-143">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="10d16-143">showCategoryName</span></span>|<span data-ttu-id="10d16-144">boolean</span><span class="sxs-lookup"><span data-stu-id="10d16-144">boolean</span></span>|<span data-ttu-id="10d16-145">Логическое значение, которое указывает, отображается ли имя для категории меток данных.</span><span class="sxs-lookup"><span data-stu-id="10d16-145">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="10d16-146">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="10d16-146">showLegendKey</span></span>|<span data-ttu-id="10d16-147">boolean</span><span class="sxs-lookup"><span data-stu-id="10d16-147">boolean</span></span>|<span data-ttu-id="10d16-148">Логическое значение, которое указывает, отображаются ли условные обозначения для меток данных.</span><span class="sxs-lookup"><span data-stu-id="10d16-148">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="10d16-149">showPercentage</span><span class="sxs-lookup"><span data-stu-id="10d16-149">showPercentage</span></span>|<span data-ttu-id="10d16-150">boolean</span><span class="sxs-lookup"><span data-stu-id="10d16-150">boolean</span></span>|<span data-ttu-id="10d16-151">Логическое значение, которое указывает, отображается ли процентное соотношение меток данных.</span><span class="sxs-lookup"><span data-stu-id="10d16-151">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="10d16-152">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="10d16-152">showSeriesName</span></span>|<span data-ttu-id="10d16-153">boolean</span><span class="sxs-lookup"><span data-stu-id="10d16-153">boolean</span></span>|<span data-ttu-id="10d16-154">Логическое значение, которое указывает, отображается ли имя ряда для меток данных.</span><span class="sxs-lookup"><span data-stu-id="10d16-154">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="10d16-155">showValue</span><span class="sxs-lookup"><span data-stu-id="10d16-155">showValue</span></span>|<span data-ttu-id="10d16-156">boolean</span><span class="sxs-lookup"><span data-stu-id="10d16-156">boolean</span></span>|<span data-ttu-id="10d16-157">Логическое значение, которое указывает, отображается ли значение метки данных.</span><span class="sxs-lookup"><span data-stu-id="10d16-157">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="response"></a><span data-ttu-id="10d16-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="10d16-158">Response</span></span>

<span data-ttu-id="10d16-159">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [воркбукчартдаталабелс](../resources/chartdatalabels.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="10d16-159">If successful, this method returns a `200 OK` response code and updated [WorkbookChartDataLabels](../resources/chartdatalabels.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="10d16-160">Пример</span><span class="sxs-lookup"><span data-stu-id="10d16-160">Example</span></span>
##### <a name="request"></a><span data-ttu-id="10d16-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="10d16-161">Request</span></span>
<span data-ttu-id="10d16-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10d16-162">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartdatalabels"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/dataLabels
Content-type: application/json
Content-length: 134

{
  "position": "position-value",
  "showValue": true,
  "showSeriesName": true,
  "showCategoryName": true,
  "showLegendKey": true
}
```
##### <a name="response"></a><span data-ttu-id="10d16-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="10d16-163">Response</span></span>
<span data-ttu-id="10d16-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="10d16-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartDataLabels"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "position": "position-value",
  "showValue": true,
  "showSeriesName": true,
  "showCategoryName": true,
  "showLegendKey": true
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="10d16-167">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="10d16-167">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="10d16-168">C#</span><span class="sxs-lookup"><span data-stu-id="10d16-168">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_chartdatalabels-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="10d16-169">Javascript</span><span class="sxs-lookup"><span data-stu-id="10d16-169">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_chartdatalabels-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="10d16-170">Цель — C</span><span class="sxs-lookup"><span data-stu-id="10d16-170">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_chartdatalabels-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartdatalabels",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/chartdatalabels-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/chartdatalabels-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/chartdatalabels-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
