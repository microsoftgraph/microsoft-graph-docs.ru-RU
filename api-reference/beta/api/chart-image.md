---
title: 'Chart: Image'
description: Отрисовывает диаграмму в виде изображения с кодировкой base64, масштабируя ее в соответствии с указанным размером.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 5ee56b38ca75162a760be54e58dacb6ced6bbc16
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976410"
---
# <a name="chart-image"></a><span data-ttu-id="a092d-103">Chart: Image</span><span class="sxs-lookup"><span data-stu-id="a092d-103">Chart: Image</span></span>

> <span data-ttu-id="a092d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a092d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a092d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a092d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a092d-106">Отрисовывает диаграмму в виде изображения с кодировкой Base64, масштабируя ее в соответствии с указанным размером.</span><span class="sxs-lookup"><span data-stu-id="a092d-106">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>
## <a name="permissions"></a><span data-ttu-id="a092d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a092d-107">Permissions</span></span>
<span data-ttu-id="a092d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a092d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a092d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a092d-110">Permission type</span></span>      | <span data-ttu-id="a092d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a092d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a092d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a092d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a092d-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a092d-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a092d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a092d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a092d-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a092d-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a092d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a092d-116">Application</span></span> | <span data-ttu-id="a092d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a092d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a092d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a092d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts(<name>)/Image(width=0,height=0,fittingMode='fit')

```
## <a name="request-headers"></a><span data-ttu-id="a092d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a092d-119">Request headers</span></span>
| <span data-ttu-id="a092d-120">Имя</span><span class="sxs-lookup"><span data-stu-id="a092d-120">Name</span></span>       | <span data-ttu-id="a092d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a092d-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a092d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a092d-122">Authorization</span></span>  | <span data-ttu-id="a092d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a092d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a092d-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a092d-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="a092d-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="a092d-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a092d-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a092d-128">Request body</span></span>
<span data-ttu-id="a092d-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="a092d-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a092d-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="a092d-130">Parameter</span></span>    | <span data-ttu-id="a092d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a092d-131">Type</span></span>   |<span data-ttu-id="a092d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a092d-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a092d-133">height</span><span class="sxs-lookup"><span data-stu-id="a092d-133">height</span></span>|<span data-ttu-id="a092d-134">number</span><span class="sxs-lookup"><span data-stu-id="a092d-134">number</span></span>|<span data-ttu-id="a092d-p105">Необязательный. Нужная высота создаваемого изображения.</span><span class="sxs-lookup"><span data-stu-id="a092d-p105">Optional. The desired height of the resulting image.</span></span>|
|<span data-ttu-id="a092d-137">width</span><span class="sxs-lookup"><span data-stu-id="a092d-137">width</span></span>|<span data-ttu-id="a092d-138">number</span><span class="sxs-lookup"><span data-stu-id="a092d-138">number</span></span>|<span data-ttu-id="a092d-p106">Необязательный. Нужная ширина создаваемого изображения.</span><span class="sxs-lookup"><span data-stu-id="a092d-p106">Optional. The desired width of the resulting image.</span></span>|
|<span data-ttu-id="a092d-141">fittingMode</span><span class="sxs-lookup"><span data-stu-id="a092d-141">fittingMode</span></span>|<span data-ttu-id="a092d-142">строка</span><span class="sxs-lookup"><span data-stu-id="a092d-142">string</span></span>|<span data-ttu-id="a092d-p107">Необязательный. Метод, используемый для масштабирования диаграммы до указанного размера (если указаны и высота, и ширина).  Возможные значения: `Fit`, `FitAndCenter`, `Fill`.</span><span class="sxs-lookup"><span data-stu-id="a092d-p107">Optional. The method used to scale the chart to the specified to the specified dimensions (if both height and width are set)."  Possible values are: `Fit`, `FitAndCenter`, `Fill`.</span></span>|

## <a name="response"></a><span data-ttu-id="a092d-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="a092d-146">Response</span></span>

<span data-ttu-id="a092d-147">В случае успеха этот метод возвращает код отклика `200 OK` и строку изображения с кодировкой base-64 в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a092d-147">If successful, this method returns `200 OK` response code and base-64 image string in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a092d-148">Пример</span><span class="sxs-lookup"><span data-stu-id="a092d-148">Example</span></span>
<span data-ttu-id="a092d-149">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="a092d-149">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a092d-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="a092d-150">Request</span></span>
<span data-ttu-id="a092d-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a092d-151">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/Image(width=0,height=0,fittingMode='fit')
```

##### <a name="response"></a><span data-ttu-id="a092d-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="a092d-152">Response</span></span>
<span data-ttu-id="a092d-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a092d-153">Here is an example of the response.</span></span> <span data-ttu-id="a092d-154">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="a092d-154">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a092d-155">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a092d-155">All of the properties will be returned from an actual call.</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 3

{
"value" : "base-64 chart image string"
}
```

##### <a name="usage"></a><span data-ttu-id="a092d-156">Применение</span><span class="sxs-lookup"><span data-stu-id="a092d-156">Usage</span></span>

<span data-ttu-id="a092d-157">Вы можете обеспечить отображение строки Base64 в теге изображения HTML: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span><span class="sxs-lookup"><span data-stu-id="a092d-157">You can display the base-64 string inside an HTML image tag: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span></span>

<span data-ttu-id="a092d-158">В случае поведения по умолчанию используйте `Image(width=0,height=0,fittingMode='fit')`.</span><span class="sxs-lookup"><span data-stu-id="a092d-158">For default behavior, use `Image(width=0,height=0,fittingMode='fit')`.</span></span> <span data-ttu-id="a092d-159">Ниже приведен пример изображения диаграммы, возвращаемого с параметрами по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a092d-159">Here is an example of a chart image returned with the default parameters.</span></span>

![Изображение диаграммы Excel с высотой и шириной по умолчанию.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-default.png)

<span data-ttu-id="a092d-161">Если вы хотите настроить отображение этого изображения, укажите высоту, ширину и режим подгонки.</span><span class="sxs-lookup"><span data-stu-id="a092d-161">If you want to customize the display of the image, specify a height, width, and a fitting mode.</span></span> <span data-ttu-id="a092d-162">Ниже показано то же изображение диаграммы, но с такими параметрами: `Image(width=500,height=500,fittingMode='Fill')`.</span><span class="sxs-lookup"><span data-stu-id="a092d-162">Here is what the same chart image looks like if you retrieve it with these parameters: `Image(width=500,height=500,fittingMode='Fill')`.</span></span>

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
