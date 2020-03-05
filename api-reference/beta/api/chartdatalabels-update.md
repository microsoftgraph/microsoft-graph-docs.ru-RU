---
title: Обновление Воркбукчартдаталабелс
description: Обновление свойств объекта воркбукчартдаталабелс.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 7682c29203e057b23f19259422c61c4264c1f3d4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42439501"
---
# <a name="update-workbookchartdatalabels"></a><span data-ttu-id="f2c21-103">Обновление Воркбукчартдаталабелс</span><span class="sxs-lookup"><span data-stu-id="f2c21-103">Update workbookChartDataLabels</span></span>

<span data-ttu-id="f2c21-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f2c21-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2c21-105">Обновление свойств объекта chartdatalabels.</span><span class="sxs-lookup"><span data-stu-id="f2c21-105">Update the properties of chartdatalabels object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f2c21-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f2c21-106">Permissions</span></span>
<span data-ttu-id="f2c21-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2c21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2c21-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f2c21-109">Permission type</span></span>      | <span data-ttu-id="f2c21-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f2c21-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2c21-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f2c21-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f2c21-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f2c21-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f2c21-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f2c21-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2c21-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f2c21-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f2c21-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f2c21-115">Application</span></span> | <span data-ttu-id="f2c21-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2c21-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2c21-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f2c21-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/datalabels
```
## <a name="optional-request-headers"></a><span data-ttu-id="f2c21-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f2c21-118">Optional request headers</span></span>
| <span data-ttu-id="f2c21-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f2c21-119">Name</span></span>       | <span data-ttu-id="f2c21-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f2c21-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f2c21-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f2c21-121">Authorization</span></span>  | <span data-ttu-id="f2c21-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f2c21-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f2c21-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f2c21-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="f2c21-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="f2c21-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2c21-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f2c21-127">Request body</span></span>
<span data-ttu-id="f2c21-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="f2c21-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f2c21-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="f2c21-131">Property</span></span>     | <span data-ttu-id="f2c21-132">Тип</span><span class="sxs-lookup"><span data-stu-id="f2c21-132">Type</span></span>   |<span data-ttu-id="f2c21-133">Описание</span><span class="sxs-lookup"><span data-stu-id="f2c21-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f2c21-134">position</span><span class="sxs-lookup"><span data-stu-id="f2c21-134">position</span></span>|<span data-ttu-id="f2c21-135">string</span><span class="sxs-lookup"><span data-stu-id="f2c21-135">string</span></span>|<span data-ttu-id="f2c21-p105">Значение DataLabelPosition, которое представляет положение метки данных. Возможные значения: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span><span class="sxs-lookup"><span data-stu-id="f2c21-p105">DataLabelPosition value that represents the position of the data label. Possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="f2c21-138">разделитель</span><span class="sxs-lookup"><span data-stu-id="f2c21-138">separator</span></span>|<span data-ttu-id="f2c21-139">string</span><span class="sxs-lookup"><span data-stu-id="f2c21-139">string</span></span>|<span data-ttu-id="f2c21-140">Строка, представляющая разделитель для меток данных на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="f2c21-140">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="f2c21-141">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="f2c21-141">showBubbleSize</span></span>|<span data-ttu-id="f2c21-142">boolean</span><span class="sxs-lookup"><span data-stu-id="f2c21-142">boolean</span></span>|<span data-ttu-id="f2c21-143">Логическое значение, которое указывает, отображается ли размер пузырьков с метками данных.</span><span class="sxs-lookup"><span data-stu-id="f2c21-143">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="f2c21-144">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="f2c21-144">showCategoryName</span></span>|<span data-ttu-id="f2c21-145">boolean</span><span class="sxs-lookup"><span data-stu-id="f2c21-145">boolean</span></span>|<span data-ttu-id="f2c21-146">Логическое значение, которое указывает, отображается ли имя для категории меток данных.</span><span class="sxs-lookup"><span data-stu-id="f2c21-146">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="f2c21-147">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="f2c21-147">showLegendKey</span></span>|<span data-ttu-id="f2c21-148">boolean</span><span class="sxs-lookup"><span data-stu-id="f2c21-148">boolean</span></span>|<span data-ttu-id="f2c21-149">Логическое значение, которое указывает, отображаются ли условные обозначения для меток данных.</span><span class="sxs-lookup"><span data-stu-id="f2c21-149">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="f2c21-150">showPercentage</span><span class="sxs-lookup"><span data-stu-id="f2c21-150">showPercentage</span></span>|<span data-ttu-id="f2c21-151">boolean</span><span class="sxs-lookup"><span data-stu-id="f2c21-151">boolean</span></span>|<span data-ttu-id="f2c21-152">Логическое значение, которое указывает, отображается ли процентное соотношение меток данных.</span><span class="sxs-lookup"><span data-stu-id="f2c21-152">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="f2c21-153">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="f2c21-153">showSeriesName</span></span>|<span data-ttu-id="f2c21-154">boolean</span><span class="sxs-lookup"><span data-stu-id="f2c21-154">boolean</span></span>|<span data-ttu-id="f2c21-155">Логическое значение, которое указывает, отображается ли имя ряда для меток данных.</span><span class="sxs-lookup"><span data-stu-id="f2c21-155">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="f2c21-156">showValue</span><span class="sxs-lookup"><span data-stu-id="f2c21-156">showValue</span></span>|<span data-ttu-id="f2c21-157">boolean</span><span class="sxs-lookup"><span data-stu-id="f2c21-157">boolean</span></span>|<span data-ttu-id="f2c21-158">Логическое значение, которое указывает, отображается ли значение метки данных.</span><span class="sxs-lookup"><span data-stu-id="f2c21-158">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="response"></a><span data-ttu-id="f2c21-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2c21-159">Response</span></span>

<span data-ttu-id="f2c21-160">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [воркбукчартдаталабелс](../resources/workbookchartdatalabels.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f2c21-160">If successful, this method returns a `200 OK` response code and updated [workbookChartDataLabels](../resources/workbookchartdatalabels.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f2c21-161">Пример</span><span class="sxs-lookup"><span data-stu-id="f2c21-161">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f2c21-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="f2c21-162">Request</span></span>
<span data-ttu-id="f2c21-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f2c21-163">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f2c21-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="f2c21-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_chartdatalabels"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/datalabels
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
# <a name="c"></a>[<span data-ttu-id="f2c21-165">C#</span><span class="sxs-lookup"><span data-stu-id="f2c21-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chartdatalabels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f2c21-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f2c21-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chartdatalabels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f2c21-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f2c21-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chartdatalabels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f2c21-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2c21-168">Response</span></span>
<span data-ttu-id="f2c21-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f2c21-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update chartdatalabels",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
