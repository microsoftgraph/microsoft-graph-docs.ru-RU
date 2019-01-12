---
title: 'Chart: Image'
description: Отрисовывает диаграмму в виде изображения с кодировкой base64, масштабируя ее в соответствии с указанным размером.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 0f61866885f0798b9e96f80e22a636fb5f619e34
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939723"
---
# <a name="chart-image"></a><span data-ttu-id="c9c84-103">Chart: Image</span><span class="sxs-lookup"><span data-stu-id="c9c84-103">Chart: Image</span></span>

<span data-ttu-id="c9c84-104">Отрисовывает диаграмму в виде изображения с кодировкой Base64, масштабируя ее в соответствии с указанным размером.</span><span class="sxs-lookup"><span data-stu-id="c9c84-104">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>
## <a name="permissions"></a><span data-ttu-id="c9c84-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c9c84-105">Permissions</span></span>
<span data-ttu-id="c9c84-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9c84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9c84-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9c84-108">Permission type</span></span>      | <span data-ttu-id="c9c84-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c9c84-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c9c84-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9c84-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c9c84-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c9c84-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c9c84-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9c84-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9c84-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9c84-113">Not supported.</span></span>    |
|<span data-ttu-id="c9c84-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c9c84-114">Application</span></span> | <span data-ttu-id="c9c84-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9c84-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c9c84-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9c84-116">HTTP request</span></span>
<!-- { "blockType": "samples" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/image
GET /workbook/worksheets/{id|name}/charts/{name}/image(width=640)
GET /workbook/worksheets/{id|name}/charts/{name}/image(width=640,height=480)
GET /workbook/worksheets/{id|name}/charts/{name}/image(width=640,height=480,fittingMode='fit')
```
## <a name="request-headers"></a><span data-ttu-id="c9c84-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c9c84-117">Request headers</span></span>
| <span data-ttu-id="c9c84-118">Имя</span><span class="sxs-lookup"><span data-stu-id="c9c84-118">Name</span></span>       | <span data-ttu-id="c9c84-119">Описание</span><span class="sxs-lookup"><span data-stu-id="c9c84-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c9c84-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c9c84-120">Authorization</span></span>  | <span data-ttu-id="c9c84-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c9c84-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c9c84-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c9c84-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="c9c84-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="c9c84-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="c9c84-126">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="c9c84-126">Path parameters</span></span>
<span data-ttu-id="c9c84-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="c9c84-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c9c84-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="c9c84-128">Parameter</span></span>    | <span data-ttu-id="c9c84-129">Тип</span><span class="sxs-lookup"><span data-stu-id="c9c84-129">Type</span></span>   |<span data-ttu-id="c9c84-130">Описание</span><span class="sxs-lookup"><span data-stu-id="c9c84-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9c84-131">height</span><span class="sxs-lookup"><span data-stu-id="c9c84-131">height</span></span>|<span data-ttu-id="c9c84-132">Int32</span><span class="sxs-lookup"><span data-stu-id="c9c84-132">Int32</span></span>|<span data-ttu-id="c9c84-133">Желаемую высоту изображения.</span><span class="sxs-lookup"><span data-stu-id="c9c84-133">The desired height of the resulting image.</span></span> <span data-ttu-id="c9c84-134">Необязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="c9c84-134">Optional.</span></span>|
|<span data-ttu-id="c9c84-135">width</span><span class="sxs-lookup"><span data-stu-id="c9c84-135">width</span></span>|<span data-ttu-id="c9c84-136">Int32</span><span class="sxs-lookup"><span data-stu-id="c9c84-136">Int32</span></span>|<span data-ttu-id="c9c84-137">Желаемую ширину изображения.</span><span class="sxs-lookup"><span data-stu-id="c9c84-137">The desired width of the resulting image.</span></span> <span data-ttu-id="c9c84-138">Необязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="c9c84-138">Optional.</span></span>|
|<span data-ttu-id="c9c84-139">fittingMode</span><span class="sxs-lookup"><span data-stu-id="c9c84-139">fittingMode</span></span>|<span data-ttu-id="c9c84-140">строка</span><span class="sxs-lookup"><span data-stu-id="c9c84-140">string</span></span>|<span data-ttu-id="c9c84-141">Метод, используемый для масштабирования диаграммы для указанного измерения (если заданы высота и ширина).»</span><span class="sxs-lookup"><span data-stu-id="c9c84-141">The method used to scale the chart to the specified dimensions (if both height and width are set)."</span></span>  <span data-ttu-id="c9c84-142">Возможные значения: `Fit`, `FitAndCenter`, `Fill`.</span><span class="sxs-lookup"><span data-stu-id="c9c84-142">The possible values are: `Fit`, `FitAndCenter`, `Fill`.</span></span>|

## <a name="response"></a><span data-ttu-id="c9c84-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9c84-143">Response</span></span>

<span data-ttu-id="c9c84-144">В случае успеха этот метод возвращает код отклика `200 OK` и строку изображения с кодировкой base-64 в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c9c84-144">If successful, this method returns `200 OK` response code and base-64 image string in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9c84-145">Пример</span><span class="sxs-lookup"><span data-stu-id="c9c84-145">Example</span></span>
<span data-ttu-id="c9c84-146">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="c9c84-146">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="c9c84-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9c84-147">Request</span></span>
<span data-ttu-id="c9c84-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c9c84-148">Here is an example of the request.</span></span>

<!-- { "blockType": "request" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/image(width=640,height=480,fittingMode='fit')
```

##### <a name="response"></a><span data-ttu-id="c9c84-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9c84-149">Response</span></span>
<span data-ttu-id="c9c84-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c9c84-150">Here is an example of the response.</span></span> <span data-ttu-id="c9c84-151">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="c9c84-151">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c9c84-152">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c9c84-152">All of the properties will be returned from an actual call.</span></span>
<!-- { "blockType": "response", "@odata.type": "Edm.String" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json;odata.metadata=minimal;odata.streaming=true

{
"value" : "base-64 chart image string"
}
```

## <a name="usage"></a><span data-ttu-id="c9c84-153">Применение</span><span class="sxs-lookup"><span data-stu-id="c9c84-153">Usage</span></span>

<span data-ttu-id="c9c84-154">Вы можете обеспечить отображение строки Base64 в теге изображения HTML: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span><span class="sxs-lookup"><span data-stu-id="c9c84-154">You can display the base-64 string inside an HTML image tag: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span></span>

<span data-ttu-id="c9c84-155">В случае поведения по умолчанию используйте `Image(width=0,height=0,fittingMode='fit')`.</span><span class="sxs-lookup"><span data-stu-id="c9c84-155">For default behavior, use `Image(width=0,height=0,fittingMode='fit')`.</span></span> <span data-ttu-id="c9c84-156">Ниже приведен пример изображения диаграммы, возвращаемого с параметрами по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="c9c84-156">Here is an example of a chart image returned with the default parameters.</span></span>

![Изображение диаграммы Excel с высотой и шириной по умолчанию.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-default.png)

<span data-ttu-id="c9c84-158">Если вы хотите настроить отображение этого изображения, укажите высоту, ширину и режим подгонки.</span><span class="sxs-lookup"><span data-stu-id="c9c84-158">If you want to customize the display of the image, specify a height, width, and a fitting mode.</span></span> <span data-ttu-id="c9c84-159">Ниже показано то же изображение диаграммы, но с такими параметрами: `Image(width=500,height=500,fittingMode='Fill')`.</span><span class="sxs-lookup"><span data-stu-id="c9c84-159">Here is what the same chart image looks like if you retrieve it with these parameters: `Image(width=500,height=500,fittingMode='Fill')`.</span></span>

![Изображение диаграммы Excel с высотой и шириной по умолчанию.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-fill.png)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chart: Image",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
