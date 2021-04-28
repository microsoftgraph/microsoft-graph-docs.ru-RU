---
title: 'Chart: Image'
description: Отрисовывает диаграмму в виде изображения с кодировкой Base64, масштабируя ее в соответствии с указанным размером.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 4f43a2f89a05aebb61ccc7efd60d89b4338b8914
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054597"
---
# <a name="chart-image"></a><span data-ttu-id="22766-103">Chart: Image</span><span class="sxs-lookup"><span data-stu-id="22766-103">Chart: Image</span></span>

<span data-ttu-id="22766-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22766-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="22766-105">Отрисовывает диаграмму в виде изображения с кодировкой Base64, масштабируя ее в соответствии с указанным размером.</span><span class="sxs-lookup"><span data-stu-id="22766-105">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>
## <a name="permissions"></a><span data-ttu-id="22766-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="22766-106">Permissions</span></span>
<span data-ttu-id="22766-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22766-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22766-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="22766-109">Permission type</span></span>      | <span data-ttu-id="22766-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="22766-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="22766-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="22766-111">Delegated (work or school account)</span></span> | <span data-ttu-id="22766-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="22766-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="22766-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="22766-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22766-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22766-114">Not supported.</span></span>    |
|<span data-ttu-id="22766-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="22766-115">Application</span></span> | <span data-ttu-id="22766-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22766-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="22766-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="22766-117">HTTP request</span></span>
<!-- { "blockType": "samples" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/image
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/image
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/image(width=640)
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/image(width=640)
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/image(width=640,height=480)
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/image(width=640,height=480)
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/image(width=640,height=480,fittingMode='fit')
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/image(width=640,height=480,fittingMode='fit')
```
## <a name="request-headers"></a><span data-ttu-id="22766-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="22766-118">Request headers</span></span>
| <span data-ttu-id="22766-119">Имя</span><span class="sxs-lookup"><span data-stu-id="22766-119">Name</span></span>       | <span data-ttu-id="22766-120">Описание</span><span class="sxs-lookup"><span data-stu-id="22766-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="22766-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="22766-121">Authorization</span></span>  | <span data-ttu-id="22766-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="22766-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="22766-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="22766-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="22766-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="22766-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="22766-127">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="22766-127">Path parameters</span></span>
<span data-ttu-id="22766-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="22766-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="22766-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="22766-129">Parameter</span></span>    | <span data-ttu-id="22766-130">Тип</span><span class="sxs-lookup"><span data-stu-id="22766-130">Type</span></span>   |<span data-ttu-id="22766-131">Описание</span><span class="sxs-lookup"><span data-stu-id="22766-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="22766-132">height</span><span class="sxs-lookup"><span data-stu-id="22766-132">height</span></span>|<span data-ttu-id="22766-133">Int32</span><span class="sxs-lookup"><span data-stu-id="22766-133">Int32</span></span>|<span data-ttu-id="22766-134">Нужная высота создаваемого изображения.</span><span class="sxs-lookup"><span data-stu-id="22766-134">The desired height of the resulting image.</span></span> <span data-ttu-id="22766-135">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="22766-135">Optional.</span></span>|
|<span data-ttu-id="22766-136">width</span><span class="sxs-lookup"><span data-stu-id="22766-136">width</span></span>|<span data-ttu-id="22766-137">Int32</span><span class="sxs-lookup"><span data-stu-id="22766-137">Int32</span></span>|<span data-ttu-id="22766-138">Нужная ширина создаваемого изображения.</span><span class="sxs-lookup"><span data-stu-id="22766-138">The desired width of the resulting image.</span></span> <span data-ttu-id="22766-139">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="22766-139">Optional.</span></span>|
|<span data-ttu-id="22766-140">fittingMode</span><span class="sxs-lookup"><span data-stu-id="22766-140">fittingMode</span></span>|<span data-ttu-id="22766-141">string</span><span class="sxs-lookup"><span data-stu-id="22766-141">string</span></span>|<span data-ttu-id="22766-142">Метод, используемый для масштабирования диаграммы до указанных размеров (если заданы как высота, так и ширина)."</span><span class="sxs-lookup"><span data-stu-id="22766-142">The method used to scale the chart to the specified dimensions (if both height and width are set)."</span></span>  <span data-ttu-id="22766-143">Допустимые значения: `Fit`, `FitAndCenter`, `Fill`.</span><span class="sxs-lookup"><span data-stu-id="22766-143">The possible values are: `Fit`, `FitAndCenter`, `Fill`.</span></span>|

## <a name="response"></a><span data-ttu-id="22766-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="22766-144">Response</span></span>

<span data-ttu-id="22766-145">В случае успеха этот метод возвращает код отклика `200 OK` и строку изображения с кодировкой base-64 в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="22766-145">If successful, this method returns `200 OK` response code and base-64 image string in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22766-146">Пример</span><span class="sxs-lookup"><span data-stu-id="22766-146">Example</span></span>
<span data-ttu-id="22766-147">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="22766-147">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="22766-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="22766-148">Request</span></span>
<span data-ttu-id="22766-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="22766-149">Here is an example of the request.</span></span>

<!-- { "blockType": "request" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/image(width=640,height=480,fittingMode='fit')
```

##### <a name="response"></a><span data-ttu-id="22766-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="22766-150">Response</span></span>
<span data-ttu-id="22766-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="22766-151">Here is an example of the response.</span></span> <span data-ttu-id="22766-152">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="22766-152">Note: The response object shown here might be shortened for readability.</span></span>
<!-- { "blockType": "response", "@odata.type": "Edm.String" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json;odata.metadata=minimal;odata.streaming=true

{
"value" : "base-64 chart image string"
}
```

## <a name="usage"></a><span data-ttu-id="22766-153">Применение</span><span class="sxs-lookup"><span data-stu-id="22766-153">Usage</span></span>

<span data-ttu-id="22766-154">Вы можете отображать строку в кодировке Base 64 в HTML-теге изображения: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span><span class="sxs-lookup"><span data-stu-id="22766-154">You can display the base-64 string inside an HTML image tag: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span></span>

<span data-ttu-id="22766-155">В случае поведения по умолчанию используйте `Image(width=0,height=0,fittingMode='fit')`.</span><span class="sxs-lookup"><span data-stu-id="22766-155">For default behavior, use `Image(width=0,height=0,fittingMode='fit')`.</span></span> <span data-ttu-id="22766-156">Ниже приведен пример изображения диаграммы, возвращаемого с параметрами по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="22766-156">Here is an example of a chart image returned with the default parameters.</span></span>

![Изображение диаграммы Excel с высотой и шириной по умолчанию.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-default.png)

<span data-ttu-id="22766-158">Если вы хотите настроить отображение этого изображения, укажите высоту, ширину и режим подгонки.</span><span class="sxs-lookup"><span data-stu-id="22766-158">If you want to customize the display of the image, specify a height, width, and a fitting mode.</span></span> <span data-ttu-id="22766-159">А вот как выглядит то же самое изображение диаграммы, если получить его с этими параметрами: `Image(width=500,height=500,fittingMode='Fill')`.</span><span class="sxs-lookup"><span data-stu-id="22766-159">Here is what the same chart image looks like if you retrieve it with these parameters: `Image(width=500,height=500,fittingMode='Fill')`.</span></span>

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

