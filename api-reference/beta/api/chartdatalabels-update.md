---
title: Обновление Воркбукчартдаталабелс
description: Обновление свойств объекта воркбукчартдаталабелс.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 1d139360f68e5468c327802693fc277949b5879e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35438246"
---
# <a name="update-workbookchartdatalabels"></a><span data-ttu-id="d9b8e-103">Обновление Воркбукчартдаталабелс</span><span class="sxs-lookup"><span data-stu-id="d9b8e-103">Update workbookChartDataLabels</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9b8e-104">Обновление свойств объекта chartdatalabels.</span><span class="sxs-lookup"><span data-stu-id="d9b8e-104">Update the properties of chartdatalabels object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d9b8e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d9b8e-105">Permissions</span></span>
<span data-ttu-id="d9b8e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9b8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9b8e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d9b8e-108">Permission type</span></span>      | <span data-ttu-id="d9b8e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d9b8e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9b8e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d9b8e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d9b8e-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d9b8e-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d9b8e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d9b8e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9b8e-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d9b8e-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d9b8e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d9b8e-114">Application</span></span> | <span data-ttu-id="d9b8e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9b8e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9b8e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d9b8e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/datalabels
```
## <a name="optional-request-headers"></a><span data-ttu-id="d9b8e-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d9b8e-117">Optional request headers</span></span>
| <span data-ttu-id="d9b8e-118">Имя</span><span class="sxs-lookup"><span data-stu-id="d9b8e-118">Name</span></span>       | <span data-ttu-id="d9b8e-119">Описание</span><span class="sxs-lookup"><span data-stu-id="d9b8e-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d9b8e-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d9b8e-120">Authorization</span></span>  | <span data-ttu-id="d9b8e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d9b8e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d9b8e-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d9b8e-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="d9b8e-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="d9b8e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9b8e-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d9b8e-126">Request body</span></span>
<span data-ttu-id="d9b8e-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="d9b8e-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d9b8e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d9b8e-130">Property</span></span>     | <span data-ttu-id="d9b8e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d9b8e-131">Type</span></span>   |<span data-ttu-id="d9b8e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d9b8e-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d9b8e-133">position</span><span class="sxs-lookup"><span data-stu-id="d9b8e-133">position</span></span>|<span data-ttu-id="d9b8e-134">string</span><span class="sxs-lookup"><span data-stu-id="d9b8e-134">string</span></span>|<span data-ttu-id="d9b8e-p105">Значение DataLabelPosition, которое представляет положение метки данных. Возможные значения: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span><span class="sxs-lookup"><span data-stu-id="d9b8e-p105">DataLabelPosition value that represents the position of the data label. Possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="d9b8e-137">разделитель</span><span class="sxs-lookup"><span data-stu-id="d9b8e-137">separator</span></span>|<span data-ttu-id="d9b8e-138">string</span><span class="sxs-lookup"><span data-stu-id="d9b8e-138">string</span></span>|<span data-ttu-id="d9b8e-139">Строка, представляющая разделитель для меток данных на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="d9b8e-139">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="d9b8e-140">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="d9b8e-140">showBubbleSize</span></span>|<span data-ttu-id="d9b8e-141">boolean</span><span class="sxs-lookup"><span data-stu-id="d9b8e-141">boolean</span></span>|<span data-ttu-id="d9b8e-142">Логическое значение, которое указывает, отображается ли размер пузырьков с метками данных.</span><span class="sxs-lookup"><span data-stu-id="d9b8e-142">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="d9b8e-143">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="d9b8e-143">showCategoryName</span></span>|<span data-ttu-id="d9b8e-144">boolean</span><span class="sxs-lookup"><span data-stu-id="d9b8e-144">boolean</span></span>|<span data-ttu-id="d9b8e-145">Логическое значение, которое указывает, отображается ли имя для категории меток данных.</span><span class="sxs-lookup"><span data-stu-id="d9b8e-145">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="d9b8e-146">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="d9b8e-146">showLegendKey</span></span>|<span data-ttu-id="d9b8e-147">boolean</span><span class="sxs-lookup"><span data-stu-id="d9b8e-147">boolean</span></span>|<span data-ttu-id="d9b8e-148">Логическое значение, которое указывает, отображаются ли условные обозначения для меток данных.</span><span class="sxs-lookup"><span data-stu-id="d9b8e-148">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="d9b8e-149">showPercentage</span><span class="sxs-lookup"><span data-stu-id="d9b8e-149">showPercentage</span></span>|<span data-ttu-id="d9b8e-150">boolean</span><span class="sxs-lookup"><span data-stu-id="d9b8e-150">boolean</span></span>|<span data-ttu-id="d9b8e-151">Логическое значение, которое указывает, отображается ли процентное соотношение меток данных.</span><span class="sxs-lookup"><span data-stu-id="d9b8e-151">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="d9b8e-152">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="d9b8e-152">showSeriesName</span></span>|<span data-ttu-id="d9b8e-153">boolean</span><span class="sxs-lookup"><span data-stu-id="d9b8e-153">boolean</span></span>|<span data-ttu-id="d9b8e-154">Логическое значение, которое указывает, отображается ли имя ряда для меток данных.</span><span class="sxs-lookup"><span data-stu-id="d9b8e-154">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="d9b8e-155">showValue</span><span class="sxs-lookup"><span data-stu-id="d9b8e-155">showValue</span></span>|<span data-ttu-id="d9b8e-156">boolean</span><span class="sxs-lookup"><span data-stu-id="d9b8e-156">boolean</span></span>|<span data-ttu-id="d9b8e-157">Логическое значение, которое указывает, отображается ли значение метки данных.</span><span class="sxs-lookup"><span data-stu-id="d9b8e-157">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="response"></a><span data-ttu-id="d9b8e-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9b8e-158">Response</span></span>

<span data-ttu-id="d9b8e-159">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [воркбукчартдаталабелс](../resources/workbookchartdatalabels.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d9b8e-159">If successful, this method returns a `200 OK` response code and updated [workbookChartDataLabels](../resources/workbookchartdatalabels.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d9b8e-160">Пример</span><span class="sxs-lookup"><span data-stu-id="d9b8e-160">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d9b8e-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="d9b8e-161">Request</span></span>
<span data-ttu-id="d9b8e-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d9b8e-162">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d9b8e-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="d9b8e-163">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="d9b8e-164">C#</span><span class="sxs-lookup"><span data-stu-id="d9b8e-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chartdatalabels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d9b8e-165">Javascript</span><span class="sxs-lookup"><span data-stu-id="d9b8e-165">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chartdatalabels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d9b8e-166">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d9b8e-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chartdatalabels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d9b8e-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9b8e-167">Response</span></span>
<span data-ttu-id="d9b8e-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d9b8e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
