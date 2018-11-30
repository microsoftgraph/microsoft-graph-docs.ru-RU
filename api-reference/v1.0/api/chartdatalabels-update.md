---
title: Обновление объекта chartdatalabels
description: Обновление свойств объекта chartdatalabels.
ms.openlocfilehash: d0e7628bc342d83dfd349104105428bb81c4c8f5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025483"
---
# <a name="update-chartdatalabels"></a><span data-ttu-id="4bb8f-103">Обновление объекта chartdatalabels</span><span class="sxs-lookup"><span data-stu-id="4bb8f-103">Update chartdatalabels</span></span>

<span data-ttu-id="4bb8f-104">Обновление свойств объекта chartdatalabels.</span><span class="sxs-lookup"><span data-stu-id="4bb8f-104">Update the properties of chartdatalabels object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4bb8f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4bb8f-105">Permissions</span></span>
<span data-ttu-id="4bb8f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4bb8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4bb8f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4bb8f-108">Permission type</span></span>      | <span data-ttu-id="4bb8f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4bb8f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4bb8f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4bb8f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4bb8f-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4bb8f-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4bb8f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4bb8f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4bb8f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4bb8f-113">Not supported.</span></span>    |
|<span data-ttu-id="4bb8f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4bb8f-114">Application</span></span> | <span data-ttu-id="4bb8f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4bb8f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4bb8f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4bb8f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/dataLabels
```
## <a name="optional-request-headers"></a><span data-ttu-id="4bb8f-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4bb8f-117">Optional request headers</span></span>
| <span data-ttu-id="4bb8f-118">Имя</span><span class="sxs-lookup"><span data-stu-id="4bb8f-118">Name</span></span>       | <span data-ttu-id="4bb8f-119">Описание</span><span class="sxs-lookup"><span data-stu-id="4bb8f-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="4bb8f-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4bb8f-120">Authorization</span></span>  | <span data-ttu-id="4bb8f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4bb8f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4bb8f-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4bb8f-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="4bb8f-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="4bb8f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4bb8f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4bb8f-126">Request body</span></span>
<span data-ttu-id="4bb8f-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="4bb8f-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4bb8f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4bb8f-130">Property</span></span>     | <span data-ttu-id="4bb8f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4bb8f-131">Type</span></span>   |<span data-ttu-id="4bb8f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4bb8f-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4bb8f-133">position</span><span class="sxs-lookup"><span data-stu-id="4bb8f-133">position</span></span>|<span data-ttu-id="4bb8f-134">string</span><span class="sxs-lookup"><span data-stu-id="4bb8f-134">string</span></span>|<span data-ttu-id="4bb8f-135">DataLabelPosition значение, представляющее положение метки данных.</span><span class="sxs-lookup"><span data-stu-id="4bb8f-135">DataLabelPosition value that represents the position of the data label.</span></span> <span data-ttu-id="4bb8f-136">Возможные значения: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span><span class="sxs-lookup"><span data-stu-id="4bb8f-136">The possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="4bb8f-137">разделитель</span><span class="sxs-lookup"><span data-stu-id="4bb8f-137">separator</span></span>|<span data-ttu-id="4bb8f-138">string</span><span class="sxs-lookup"><span data-stu-id="4bb8f-138">string</span></span>|<span data-ttu-id="4bb8f-139">Строка, представляющая разделитель для меток данных на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="4bb8f-139">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="4bb8f-140">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="4bb8f-140">showBubbleSize</span></span>|<span data-ttu-id="4bb8f-141">boolean</span><span class="sxs-lookup"><span data-stu-id="4bb8f-141">boolean</span></span>|<span data-ttu-id="4bb8f-142">Логическое значение, которое указывает, отображается ли размер пузырьков с метками данных.</span><span class="sxs-lookup"><span data-stu-id="4bb8f-142">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="4bb8f-143">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="4bb8f-143">showCategoryName</span></span>|<span data-ttu-id="4bb8f-144">boolean</span><span class="sxs-lookup"><span data-stu-id="4bb8f-144">boolean</span></span>|<span data-ttu-id="4bb8f-145">Логическое значение, которое указывает, отображается ли имя для категории меток данных.</span><span class="sxs-lookup"><span data-stu-id="4bb8f-145">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="4bb8f-146">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="4bb8f-146">showLegendKey</span></span>|<span data-ttu-id="4bb8f-147">boolean</span><span class="sxs-lookup"><span data-stu-id="4bb8f-147">boolean</span></span>|<span data-ttu-id="4bb8f-148">Логическое значение, которое указывает, отображаются ли условные обозначения для меток данных.</span><span class="sxs-lookup"><span data-stu-id="4bb8f-148">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="4bb8f-149">showPercentage</span><span class="sxs-lookup"><span data-stu-id="4bb8f-149">showPercentage</span></span>|<span data-ttu-id="4bb8f-150">boolean</span><span class="sxs-lookup"><span data-stu-id="4bb8f-150">boolean</span></span>|<span data-ttu-id="4bb8f-151">Логическое значение, которое указывает, отображается ли процентное соотношение меток данных.</span><span class="sxs-lookup"><span data-stu-id="4bb8f-151">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="4bb8f-152">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="4bb8f-152">showSeriesName</span></span>|<span data-ttu-id="4bb8f-153">boolean</span><span class="sxs-lookup"><span data-stu-id="4bb8f-153">boolean</span></span>|<span data-ttu-id="4bb8f-154">Логическое значение, которое указывает, отображается ли имя ряда для меток данных.</span><span class="sxs-lookup"><span data-stu-id="4bb8f-154">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="4bb8f-155">showValue</span><span class="sxs-lookup"><span data-stu-id="4bb8f-155">showValue</span></span>|<span data-ttu-id="4bb8f-156">boolean</span><span class="sxs-lookup"><span data-stu-id="4bb8f-156">boolean</span></span>|<span data-ttu-id="4bb8f-157">Логическое значение, которое указывает, отображается ли значение метки данных.</span><span class="sxs-lookup"><span data-stu-id="4bb8f-157">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="response"></a><span data-ttu-id="4bb8f-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="4bb8f-158">Response</span></span>

<span data-ttu-id="4bb8f-159">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленный объект [WorkbookChartDataLabels](../resources/chartdatalabels.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4bb8f-159">If successful, this method returns a `200 OK` response code and updated [WorkbookChartDataLabels](../resources/chartdatalabels.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4bb8f-160">Пример</span><span class="sxs-lookup"><span data-stu-id="4bb8f-160">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4bb8f-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="4bb8f-161">Request</span></span>
<span data-ttu-id="4bb8f-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4bb8f-162">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="4bb8f-163">Ответ</span><span class="sxs-lookup"><span data-stu-id="4bb8f-163">Response</span></span>
<span data-ttu-id="4bb8f-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="4bb8f-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartdatalabels",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->