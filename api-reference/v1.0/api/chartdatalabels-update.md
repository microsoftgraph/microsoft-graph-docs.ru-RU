---
title: Обновление объекта chartdatalabels
description: Обновление свойств объекта chartdatalabels.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: cbd519c302c64c78dfbca81ad50d1c142d5e5e92
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874552"
---
# <a name="update-chartdatalabels"></a><span data-ttu-id="a6f22-103">Обновление объекта chartdatalabels</span><span class="sxs-lookup"><span data-stu-id="a6f22-103">Update chartdatalabels</span></span>

<span data-ttu-id="a6f22-104">Обновление свойств объекта chartdatalabels.</span><span class="sxs-lookup"><span data-stu-id="a6f22-104">Update the properties of chartdatalabels object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a6f22-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a6f22-105">Permissions</span></span>
<span data-ttu-id="a6f22-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6f22-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6f22-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a6f22-108">Permission type</span></span>      | <span data-ttu-id="a6f22-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a6f22-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6f22-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a6f22-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a6f22-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a6f22-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a6f22-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a6f22-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6f22-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6f22-113">Not supported.</span></span>    |
|<span data-ttu-id="a6f22-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a6f22-114">Application</span></span> | <span data-ttu-id="a6f22-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6f22-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6f22-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a6f22-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/dataLabels
```
## <a name="optional-request-headers"></a><span data-ttu-id="a6f22-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a6f22-117">Optional request headers</span></span>
| <span data-ttu-id="a6f22-118">Имя</span><span class="sxs-lookup"><span data-stu-id="a6f22-118">Name</span></span>       | <span data-ttu-id="a6f22-119">Описание</span><span class="sxs-lookup"><span data-stu-id="a6f22-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="a6f22-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a6f22-120">Authorization</span></span>  | <span data-ttu-id="a6f22-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a6f22-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a6f22-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a6f22-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="a6f22-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="a6f22-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6f22-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a6f22-126">Request body</span></span>
<span data-ttu-id="a6f22-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="a6f22-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a6f22-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a6f22-130">Property</span></span>     | <span data-ttu-id="a6f22-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a6f22-131">Type</span></span>   |<span data-ttu-id="a6f22-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a6f22-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a6f22-133">position</span><span class="sxs-lookup"><span data-stu-id="a6f22-133">position</span></span>|<span data-ttu-id="a6f22-134">string</span><span class="sxs-lookup"><span data-stu-id="a6f22-134">string</span></span>|<span data-ttu-id="a6f22-135">DataLabelPosition значение, представляющее положение метки данных.</span><span class="sxs-lookup"><span data-stu-id="a6f22-135">DataLabelPosition value that represents the position of the data label.</span></span> <span data-ttu-id="a6f22-136">Возможные значения: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span><span class="sxs-lookup"><span data-stu-id="a6f22-136">The possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="a6f22-137">разделитель</span><span class="sxs-lookup"><span data-stu-id="a6f22-137">separator</span></span>|<span data-ttu-id="a6f22-138">string</span><span class="sxs-lookup"><span data-stu-id="a6f22-138">string</span></span>|<span data-ttu-id="a6f22-139">Строка, представляющая разделитель для меток данных на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="a6f22-139">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="a6f22-140">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="a6f22-140">showBubbleSize</span></span>|<span data-ttu-id="a6f22-141">boolean</span><span class="sxs-lookup"><span data-stu-id="a6f22-141">boolean</span></span>|<span data-ttu-id="a6f22-142">Логическое значение, которое указывает, отображается ли размер пузырьков с метками данных.</span><span class="sxs-lookup"><span data-stu-id="a6f22-142">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="a6f22-143">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="a6f22-143">showCategoryName</span></span>|<span data-ttu-id="a6f22-144">boolean</span><span class="sxs-lookup"><span data-stu-id="a6f22-144">boolean</span></span>|<span data-ttu-id="a6f22-145">Логическое значение, которое указывает, отображается ли имя для категории меток данных.</span><span class="sxs-lookup"><span data-stu-id="a6f22-145">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="a6f22-146">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="a6f22-146">showLegendKey</span></span>|<span data-ttu-id="a6f22-147">boolean</span><span class="sxs-lookup"><span data-stu-id="a6f22-147">boolean</span></span>|<span data-ttu-id="a6f22-148">Логическое значение, которое указывает, отображаются ли условные обозначения для меток данных.</span><span class="sxs-lookup"><span data-stu-id="a6f22-148">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="a6f22-149">showPercentage</span><span class="sxs-lookup"><span data-stu-id="a6f22-149">showPercentage</span></span>|<span data-ttu-id="a6f22-150">boolean</span><span class="sxs-lookup"><span data-stu-id="a6f22-150">boolean</span></span>|<span data-ttu-id="a6f22-151">Логическое значение, которое указывает, отображается ли процентное соотношение меток данных.</span><span class="sxs-lookup"><span data-stu-id="a6f22-151">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="a6f22-152">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="a6f22-152">showSeriesName</span></span>|<span data-ttu-id="a6f22-153">boolean</span><span class="sxs-lookup"><span data-stu-id="a6f22-153">boolean</span></span>|<span data-ttu-id="a6f22-154">Логическое значение, которое указывает, отображается ли имя ряда для меток данных.</span><span class="sxs-lookup"><span data-stu-id="a6f22-154">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="a6f22-155">showValue</span><span class="sxs-lookup"><span data-stu-id="a6f22-155">showValue</span></span>|<span data-ttu-id="a6f22-156">boolean</span><span class="sxs-lookup"><span data-stu-id="a6f22-156">boolean</span></span>|<span data-ttu-id="a6f22-157">Логическое значение, которое указывает, отображается ли значение метки данных.</span><span class="sxs-lookup"><span data-stu-id="a6f22-157">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="response"></a><span data-ttu-id="a6f22-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6f22-158">Response</span></span>

<span data-ttu-id="a6f22-159">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленный объект [WorkbookChartDataLabels](../resources/chartdatalabels.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a6f22-159">If successful, this method returns a `200 OK` response code and updated [WorkbookChartDataLabels](../resources/chartdatalabels.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a6f22-160">Пример</span><span class="sxs-lookup"><span data-stu-id="a6f22-160">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a6f22-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="a6f22-161">Request</span></span>
<span data-ttu-id="a6f22-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a6f22-162">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="a6f22-163">Ответ</span><span class="sxs-lookup"><span data-stu-id="a6f22-163">Response</span></span>
<span data-ttu-id="a6f22-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a6f22-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
