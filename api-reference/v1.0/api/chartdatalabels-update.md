---
title: Обновление объекта chartdatalabels
description: Обновление свойств объекта chartdatalabels.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: a3e0b4ca77e9fac770d12b14978412bcfd9d8689
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051559"
---
# <a name="update-chartdatalabels"></a><span data-ttu-id="b3b44-103">Обновление объекта chartdatalabels</span><span class="sxs-lookup"><span data-stu-id="b3b44-103">Update chartdatalabels</span></span>

<span data-ttu-id="b3b44-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3b44-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b3b44-105">Обновление свойств объекта chartdatalabels.</span><span class="sxs-lookup"><span data-stu-id="b3b44-105">Update the properties of chartdatalabels object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b3b44-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b3b44-106">Permissions</span></span>
<span data-ttu-id="b3b44-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3b44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3b44-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b3b44-109">Permission type</span></span>      | <span data-ttu-id="b3b44-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b3b44-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b3b44-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b3b44-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b3b44-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b3b44-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b3b44-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b3b44-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3b44-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3b44-114">Not supported.</span></span>    |
|<span data-ttu-id="b3b44-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b3b44-115">Application</span></span> | <span data-ttu-id="b3b44-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3b44-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3b44-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b3b44-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/dataLabels
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/dataLabels
```
## <a name="optional-request-headers"></a><span data-ttu-id="b3b44-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b3b44-118">Optional request headers</span></span>
| <span data-ttu-id="b3b44-119">Имя</span><span class="sxs-lookup"><span data-stu-id="b3b44-119">Name</span></span>       | <span data-ttu-id="b3b44-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b3b44-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="b3b44-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b3b44-121">Authorization</span></span>  | <span data-ttu-id="b3b44-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b3b44-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b3b44-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b3b44-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="b3b44-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="b3b44-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3b44-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b3b44-127">Request body</span></span>
<span data-ttu-id="b3b44-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="b3b44-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b3b44-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="b3b44-131">Property</span></span>     | <span data-ttu-id="b3b44-132">Тип</span><span class="sxs-lookup"><span data-stu-id="b3b44-132">Type</span></span>   |<span data-ttu-id="b3b44-133">Описание</span><span class="sxs-lookup"><span data-stu-id="b3b44-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b3b44-134">position</span><span class="sxs-lookup"><span data-stu-id="b3b44-134">position</span></span>|<span data-ttu-id="b3b44-135">string</span><span class="sxs-lookup"><span data-stu-id="b3b44-135">string</span></span>|<span data-ttu-id="b3b44-136">Значение DataLabelPosition, которое представляет положение метки данных.</span><span class="sxs-lookup"><span data-stu-id="b3b44-136">DataLabelPosition value that represents the position of the data label.</span></span> <span data-ttu-id="b3b44-137">Возможные значения: `None` `Center` , , , , , , `InsideEnd` , `InsideBase` `OutsideEnd` `Left` `Right` `Top` `Bottom` `BestFit` `Callout` .</span><span class="sxs-lookup"><span data-stu-id="b3b44-137">The possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="b3b44-138">separator</span><span class="sxs-lookup"><span data-stu-id="b3b44-138">separator</span></span>|<span data-ttu-id="b3b44-139">string</span><span class="sxs-lookup"><span data-stu-id="b3b44-139">string</span></span>|<span data-ttu-id="b3b44-140">Строка, представляющая разделитель для меток данных на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="b3b44-140">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="b3b44-141">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="b3b44-141">showBubbleSize</span></span>|<span data-ttu-id="b3b44-142">boolean</span><span class="sxs-lookup"><span data-stu-id="b3b44-142">boolean</span></span>|<span data-ttu-id="b3b44-143">Логическое значение, которое указывает, отображается ли размер пузырьков с метками данных.</span><span class="sxs-lookup"><span data-stu-id="b3b44-143">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="b3b44-144">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="b3b44-144">showCategoryName</span></span>|<span data-ttu-id="b3b44-145">boolean</span><span class="sxs-lookup"><span data-stu-id="b3b44-145">boolean</span></span>|<span data-ttu-id="b3b44-146">Логическое значение, которое указывает, отображается ли имя для категории меток данных.</span><span class="sxs-lookup"><span data-stu-id="b3b44-146">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="b3b44-147">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="b3b44-147">showLegendKey</span></span>|<span data-ttu-id="b3b44-148">boolean</span><span class="sxs-lookup"><span data-stu-id="b3b44-148">boolean</span></span>|<span data-ttu-id="b3b44-149">Логическое значение, которое указывает, отображаются ли условные обозначения для меток данных.</span><span class="sxs-lookup"><span data-stu-id="b3b44-149">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="b3b44-150">showPercentage</span><span class="sxs-lookup"><span data-stu-id="b3b44-150">showPercentage</span></span>|<span data-ttu-id="b3b44-151">boolean</span><span class="sxs-lookup"><span data-stu-id="b3b44-151">boolean</span></span>|<span data-ttu-id="b3b44-152">Логическое значение, которое указывает, отображается ли процентное соотношение меток данных.</span><span class="sxs-lookup"><span data-stu-id="b3b44-152">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="b3b44-153">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="b3b44-153">showSeriesName</span></span>|<span data-ttu-id="b3b44-154">boolean</span><span class="sxs-lookup"><span data-stu-id="b3b44-154">boolean</span></span>|<span data-ttu-id="b3b44-155">Логическое значение, которое указывает, отображается ли имя ряда для меток данных.</span><span class="sxs-lookup"><span data-stu-id="b3b44-155">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="b3b44-156">showValue</span><span class="sxs-lookup"><span data-stu-id="b3b44-156">showValue</span></span>|<span data-ttu-id="b3b44-157">boolean</span><span class="sxs-lookup"><span data-stu-id="b3b44-157">boolean</span></span>|<span data-ttu-id="b3b44-158">Логическое значение, которое указывает, отображается ли значение метки данных.</span><span class="sxs-lookup"><span data-stu-id="b3b44-158">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="response"></a><span data-ttu-id="b3b44-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3b44-159">Response</span></span>

<span data-ttu-id="b3b44-160">В случае успеха этот метод возвращает код ответа и обновленный объект `200 OK` [WorkbookChartDataLabels](../resources/chartdatalabels.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b3b44-160">If successful, this method returns a `200 OK` response code and updated [WorkbookChartDataLabels](../resources/chartdatalabels.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b3b44-161">Пример</span><span class="sxs-lookup"><span data-stu-id="b3b44-161">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b3b44-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3b44-162">Request</span></span>
<span data-ttu-id="b3b44-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b3b44-163">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b3b44-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="b3b44-164">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b3b44-165">C#</span><span class="sxs-lookup"><span data-stu-id="b3b44-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chartdatalabels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b3b44-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b3b44-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chartdatalabels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b3b44-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b3b44-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chartdatalabels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b3b44-168">Java</span><span class="sxs-lookup"><span data-stu-id="b3b44-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-chartdatalabels-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b3b44-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3b44-169">Response</span></span>
<span data-ttu-id="b3b44-170">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b3b44-170">Here is an example of the response.</span></span> <span data-ttu-id="b3b44-171">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b3b44-171">Note: The response object shown here might be shortened for readability.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->

