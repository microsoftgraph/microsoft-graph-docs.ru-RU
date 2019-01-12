---
title: Обновление объекта chartdatalabels
description: Обновление свойств объекта chartdatalabels.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: f61113f8cd0617d6d8eb3f3191112d74e55f27cb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985440"
---
# <a name="update-chartdatalabels"></a><span data-ttu-id="fe2c2-103">Обновление объекта chartdatalabels</span><span class="sxs-lookup"><span data-stu-id="fe2c2-103">Update chartdatalabels</span></span>

> <span data-ttu-id="fe2c2-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fe2c2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fe2c2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe2c2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fe2c2-106">Обновление свойств объекта chartdatalabels.</span><span class="sxs-lookup"><span data-stu-id="fe2c2-106">Update the properties of chartdatalabels object.</span></span>
## <a name="permissions"></a><span data-ttu-id="fe2c2-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fe2c2-107">Permissions</span></span>
<span data-ttu-id="fe2c2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe2c2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe2c2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fe2c2-110">Permission type</span></span>      | <span data-ttu-id="fe2c2-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fe2c2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe2c2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fe2c2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fe2c2-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fe2c2-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fe2c2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fe2c2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe2c2-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fe2c2-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fe2c2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fe2c2-116">Application</span></span> | <span data-ttu-id="fe2c2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe2c2-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe2c2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fe2c2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/datalabels
```
## <a name="optional-request-headers"></a><span data-ttu-id="fe2c2-119">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fe2c2-119">Optional request headers</span></span>
| <span data-ttu-id="fe2c2-120">Имя</span><span class="sxs-lookup"><span data-stu-id="fe2c2-120">Name</span></span>       | <span data-ttu-id="fe2c2-121">Описание</span><span class="sxs-lookup"><span data-stu-id="fe2c2-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="fe2c2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fe2c2-122">Authorization</span></span>  | <span data-ttu-id="fe2c2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fe2c2-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fe2c2-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="fe2c2-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="fe2c2-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="fe2c2-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe2c2-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fe2c2-128">Request body</span></span>
<span data-ttu-id="fe2c2-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="fe2c2-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="fe2c2-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="fe2c2-132">Property</span></span>     | <span data-ttu-id="fe2c2-133">Тип</span><span class="sxs-lookup"><span data-stu-id="fe2c2-133">Type</span></span>   |<span data-ttu-id="fe2c2-134">Описание</span><span class="sxs-lookup"><span data-stu-id="fe2c2-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fe2c2-135">position</span><span class="sxs-lookup"><span data-stu-id="fe2c2-135">position</span></span>|<span data-ttu-id="fe2c2-136">строка</span><span class="sxs-lookup"><span data-stu-id="fe2c2-136">string</span></span>|<span data-ttu-id="fe2c2-p106">Значение DataLabelPosition, которое представляет положение метки данных. Возможные значения: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span><span class="sxs-lookup"><span data-stu-id="fe2c2-p106">DataLabelPosition value that represents the position of the data label. Possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="fe2c2-139">разделитель</span><span class="sxs-lookup"><span data-stu-id="fe2c2-139">separator</span></span>|<span data-ttu-id="fe2c2-140">строка</span><span class="sxs-lookup"><span data-stu-id="fe2c2-140">string</span></span>|<span data-ttu-id="fe2c2-141">Строка, представляющая разделитель для меток данных на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="fe2c2-141">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="fe2c2-142">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="fe2c2-142">showBubbleSize</span></span>|<span data-ttu-id="fe2c2-143">boolean</span><span class="sxs-lookup"><span data-stu-id="fe2c2-143">boolean</span></span>|<span data-ttu-id="fe2c2-144">Логическое значение, которое указывает, отображается ли размер пузырьков с метками данных.</span><span class="sxs-lookup"><span data-stu-id="fe2c2-144">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="fe2c2-145">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="fe2c2-145">showCategoryName</span></span>|<span data-ttu-id="fe2c2-146">boolean</span><span class="sxs-lookup"><span data-stu-id="fe2c2-146">boolean</span></span>|<span data-ttu-id="fe2c2-147">Логическое значение, которое указывает, отображается ли имя для категории меток данных.</span><span class="sxs-lookup"><span data-stu-id="fe2c2-147">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="fe2c2-148">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="fe2c2-148">showLegendKey</span></span>|<span data-ttu-id="fe2c2-149">boolean</span><span class="sxs-lookup"><span data-stu-id="fe2c2-149">boolean</span></span>|<span data-ttu-id="fe2c2-150">Логическое значение, которое указывает, отображаются ли условные обозначения для меток данных.</span><span class="sxs-lookup"><span data-stu-id="fe2c2-150">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="fe2c2-151">showPercentage</span><span class="sxs-lookup"><span data-stu-id="fe2c2-151">showPercentage</span></span>|<span data-ttu-id="fe2c2-152">boolean</span><span class="sxs-lookup"><span data-stu-id="fe2c2-152">boolean</span></span>|<span data-ttu-id="fe2c2-153">Логическое значение, которое указывает, отображается ли процентное соотношение меток данных.</span><span class="sxs-lookup"><span data-stu-id="fe2c2-153">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="fe2c2-154">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="fe2c2-154">showSeriesName</span></span>|<span data-ttu-id="fe2c2-155">boolean</span><span class="sxs-lookup"><span data-stu-id="fe2c2-155">boolean</span></span>|<span data-ttu-id="fe2c2-156">Логическое значение, которое указывает, отображается ли имя ряда для меток данных.</span><span class="sxs-lookup"><span data-stu-id="fe2c2-156">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="fe2c2-157">showValue</span><span class="sxs-lookup"><span data-stu-id="fe2c2-157">showValue</span></span>|<span data-ttu-id="fe2c2-158">boolean</span><span class="sxs-lookup"><span data-stu-id="fe2c2-158">boolean</span></span>|<span data-ttu-id="fe2c2-159">Логическое значение, которое указывает, отображается ли значение метки данных.</span><span class="sxs-lookup"><span data-stu-id="fe2c2-159">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="response"></a><span data-ttu-id="fe2c2-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe2c2-160">Response</span></span>

<span data-ttu-id="fe2c2-161">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [ChartDataLabels](../resources/chartdatalabels.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fe2c2-161">If successful, this method returns a `200 OK` response code and updated [ChartDataLabels](../resources/chartdatalabels.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fe2c2-162">Пример</span><span class="sxs-lookup"><span data-stu-id="fe2c2-162">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fe2c2-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="fe2c2-163">Request</span></span>
<span data-ttu-id="fe2c2-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fe2c2-164">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="fe2c2-165">Ответ</span><span class="sxs-lookup"><span data-stu-id="fe2c2-165">Response</span></span>
<span data-ttu-id="fe2c2-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fe2c2-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update chartdatalabels",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
