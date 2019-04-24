---
title: Обновление объекта chartdatalabels
description: Обновление свойств объекта chartdatalabels.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: b7eb067bed747ae2532939e61a9e0dec58ff4655
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456481"
---
# <a name="update-chartdatalabels"></a><span data-ttu-id="0ca8e-103">Обновление объекта chartdatalabels</span><span class="sxs-lookup"><span data-stu-id="0ca8e-103">Update chartdatalabels</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ca8e-104">Обновление свойств объекта chartdatalabels.</span><span class="sxs-lookup"><span data-stu-id="0ca8e-104">Update the properties of chartdatalabels object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0ca8e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0ca8e-105">Permissions</span></span>
<span data-ttu-id="0ca8e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ca8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ca8e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ca8e-108">Permission type</span></span>      | <span data-ttu-id="0ca8e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ca8e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ca8e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ca8e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0ca8e-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ca8e-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0ca8e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ca8e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ca8e-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ca8e-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0ca8e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0ca8e-114">Application</span></span> | <span data-ttu-id="0ca8e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ca8e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ca8e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ca8e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/datalabels
```
## <a name="optional-request-headers"></a><span data-ttu-id="0ca8e-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0ca8e-117">Optional request headers</span></span>
| <span data-ttu-id="0ca8e-118">Имя</span><span class="sxs-lookup"><span data-stu-id="0ca8e-118">Name</span></span>       | <span data-ttu-id="0ca8e-119">Описание</span><span class="sxs-lookup"><span data-stu-id="0ca8e-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0ca8e-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0ca8e-120">Authorization</span></span>  | <span data-ttu-id="0ca8e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0ca8e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0ca8e-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0ca8e-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="0ca8e-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="0ca8e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ca8e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0ca8e-126">Request body</span></span>
<span data-ttu-id="0ca8e-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="0ca8e-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0ca8e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0ca8e-130">Property</span></span>     | <span data-ttu-id="0ca8e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0ca8e-131">Type</span></span>   |<span data-ttu-id="0ca8e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0ca8e-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0ca8e-133">position</span><span class="sxs-lookup"><span data-stu-id="0ca8e-133">position</span></span>|<span data-ttu-id="0ca8e-134">string</span><span class="sxs-lookup"><span data-stu-id="0ca8e-134">string</span></span>|<span data-ttu-id="0ca8e-p105">Значение DataLabelPosition, которое представляет положение метки данных. Возможные значения: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span><span class="sxs-lookup"><span data-stu-id="0ca8e-p105">DataLabelPosition value that represents the position of the data label. Possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="0ca8e-137">разделитель</span><span class="sxs-lookup"><span data-stu-id="0ca8e-137">separator</span></span>|<span data-ttu-id="0ca8e-138">string</span><span class="sxs-lookup"><span data-stu-id="0ca8e-138">string</span></span>|<span data-ttu-id="0ca8e-139">Строка, представляющая разделитель для меток данных на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="0ca8e-139">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="0ca8e-140">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="0ca8e-140">showBubbleSize</span></span>|<span data-ttu-id="0ca8e-141">логический</span><span class="sxs-lookup"><span data-stu-id="0ca8e-141">boolean</span></span>|<span data-ttu-id="0ca8e-142">Логическое значение, которое указывает, отображается ли размер пузырьков с метками данных.</span><span class="sxs-lookup"><span data-stu-id="0ca8e-142">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="0ca8e-143">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="0ca8e-143">showCategoryName</span></span>|<span data-ttu-id="0ca8e-144">логический</span><span class="sxs-lookup"><span data-stu-id="0ca8e-144">boolean</span></span>|<span data-ttu-id="0ca8e-145">Логическое значение, которое указывает, отображается ли имя для категории меток данных.</span><span class="sxs-lookup"><span data-stu-id="0ca8e-145">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="0ca8e-146">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="0ca8e-146">showLegendKey</span></span>|<span data-ttu-id="0ca8e-147">логический</span><span class="sxs-lookup"><span data-stu-id="0ca8e-147">boolean</span></span>|<span data-ttu-id="0ca8e-148">Логическое значение, которое указывает, отображаются ли условные обозначения для меток данных.</span><span class="sxs-lookup"><span data-stu-id="0ca8e-148">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="0ca8e-149">showPercentage</span><span class="sxs-lookup"><span data-stu-id="0ca8e-149">showPercentage</span></span>|<span data-ttu-id="0ca8e-150">логический</span><span class="sxs-lookup"><span data-stu-id="0ca8e-150">boolean</span></span>|<span data-ttu-id="0ca8e-151">Логическое значение, которое указывает, отображается ли процентное соотношение меток данных.</span><span class="sxs-lookup"><span data-stu-id="0ca8e-151">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="0ca8e-152">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="0ca8e-152">showSeriesName</span></span>|<span data-ttu-id="0ca8e-153">логический</span><span class="sxs-lookup"><span data-stu-id="0ca8e-153">boolean</span></span>|<span data-ttu-id="0ca8e-154">Логическое значение, которое указывает, отображается ли имя ряда для меток данных.</span><span class="sxs-lookup"><span data-stu-id="0ca8e-154">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="0ca8e-155">showValue</span><span class="sxs-lookup"><span data-stu-id="0ca8e-155">showValue</span></span>|<span data-ttu-id="0ca8e-156">boolean</span><span class="sxs-lookup"><span data-stu-id="0ca8e-156">boolean</span></span>|<span data-ttu-id="0ca8e-157">Логическое значение, которое указывает, отображается ли значение метки данных.</span><span class="sxs-lookup"><span data-stu-id="0ca8e-157">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="response"></a><span data-ttu-id="0ca8e-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ca8e-158">Response</span></span>

<span data-ttu-id="0ca8e-159">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [ChartDataLabels](../resources/chartdatalabels.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0ca8e-159">If successful, this method returns a `200 OK` response code and updated [ChartDataLabels](../resources/chartdatalabels.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0ca8e-160">Пример</span><span class="sxs-lookup"><span data-stu-id="0ca8e-160">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0ca8e-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ca8e-161">Request</span></span>
<span data-ttu-id="0ca8e-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0ca8e-162">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartdatalabels"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/datalabels
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
##### <a name="response"></a><span data-ttu-id="0ca8e-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ca8e-163">Response</span></span>
<span data-ttu-id="0ca8e-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0ca8e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartDataLabels"
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update chartdatalabels",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chartdatalabels-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
