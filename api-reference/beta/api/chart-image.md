---
title: 'Chart: Image'
description: Отрисовывает диаграмму в виде изображения с кодировкой Base64, масштабируя ее в соответствии с указанным размером.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 6696ee897a3baf98e0bc3d156771ae23386b2ccc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47983209"
---
# <a name="chart-image"></a><span data-ttu-id="647c2-103">Chart: Image</span><span class="sxs-lookup"><span data-stu-id="647c2-103">Chart: Image</span></span>

<span data-ttu-id="647c2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="647c2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="647c2-105">Отрисовывает диаграмму в виде изображения с кодировкой Base64, масштабируя ее в соответствии с указанным размером.</span><span class="sxs-lookup"><span data-stu-id="647c2-105">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>
## <a name="permissions"></a><span data-ttu-id="647c2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="647c2-106">Permissions</span></span>
<span data-ttu-id="647c2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="647c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="647c2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="647c2-109">Permission type</span></span>      | <span data-ttu-id="647c2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="647c2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="647c2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="647c2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="647c2-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="647c2-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="647c2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="647c2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="647c2-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="647c2-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="647c2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="647c2-115">Application</span></span> | <span data-ttu-id="647c2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="647c2-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="647c2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="647c2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/Image(width=0,height=0,fittingMode='fit')

```
## <a name="request-headers"></a><span data-ttu-id="647c2-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="647c2-118">Request headers</span></span>
| <span data-ttu-id="647c2-119">Имя</span><span class="sxs-lookup"><span data-stu-id="647c2-119">Name</span></span>       | <span data-ttu-id="647c2-120">Описание</span><span class="sxs-lookup"><span data-stu-id="647c2-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="647c2-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="647c2-121">Authorization</span></span>  | <span data-ttu-id="647c2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="647c2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="647c2-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="647c2-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="647c2-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="647c2-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="647c2-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="647c2-127">Request body</span></span>
<span data-ttu-id="647c2-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="647c2-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="647c2-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="647c2-129">Parameter</span></span>    | <span data-ttu-id="647c2-130">Тип</span><span class="sxs-lookup"><span data-stu-id="647c2-130">Type</span></span>   |<span data-ttu-id="647c2-131">Описание</span><span class="sxs-lookup"><span data-stu-id="647c2-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="647c2-132">height</span><span class="sxs-lookup"><span data-stu-id="647c2-132">height</span></span>|<span data-ttu-id="647c2-133">number</span><span class="sxs-lookup"><span data-stu-id="647c2-133">number</span></span>|<span data-ttu-id="647c2-p104">Необязательный. Нужная высота создаваемого изображения.</span><span class="sxs-lookup"><span data-stu-id="647c2-p104">Optional. The desired height of the resulting image.</span></span>|
|<span data-ttu-id="647c2-136">width</span><span class="sxs-lookup"><span data-stu-id="647c2-136">width</span></span>|<span data-ttu-id="647c2-137">number</span><span class="sxs-lookup"><span data-stu-id="647c2-137">number</span></span>|<span data-ttu-id="647c2-p105">Необязательный. Нужная ширина создаваемого изображения.</span><span class="sxs-lookup"><span data-stu-id="647c2-p105">Optional. The desired width of the resulting image.</span></span>|
|<span data-ttu-id="647c2-140">fittingMode</span><span class="sxs-lookup"><span data-stu-id="647c2-140">fittingMode</span></span>|<span data-ttu-id="647c2-141">string</span><span class="sxs-lookup"><span data-stu-id="647c2-141">string</span></span>|<span data-ttu-id="647c2-p106">Необязательный. Метод, используемый для масштабирования диаграммы до указанного размера (если указаны и высота, и ширина).  Возможные значения: `Fit`, `FitAndCenter`, `Fill`.</span><span class="sxs-lookup"><span data-stu-id="647c2-p106">Optional. The method used to scale the chart to the specified to the specified dimensions (if both height and width are set)."  Possible values are: `Fit`, `FitAndCenter`, `Fill`.</span></span>|

## <a name="response"></a><span data-ttu-id="647c2-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="647c2-145">Response</span></span>

<span data-ttu-id="647c2-146">В случае успеха этот метод возвращает код отклика `200 OK` и строку изображения с кодировкой base-64 в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="647c2-146">If successful, this method returns `200 OK` response code and base-64 image string in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="647c2-147">Пример</span><span class="sxs-lookup"><span data-stu-id="647c2-147">Example</span></span>
<span data-ttu-id="647c2-148">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="647c2-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="647c2-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="647c2-149">Request</span></span>
<span data-ttu-id="647c2-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="647c2-150">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/Image(width=0,height=0,fittingMode='fit')
```

##### <a name="response"></a><span data-ttu-id="647c2-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="647c2-151">Response</span></span>
<span data-ttu-id="647c2-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="647c2-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call. </span></span><!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 3

{
"value" : "base-64 chart image string"
}
```

##### <a name="usage"></a><span data-ttu-id="647c2-155">Применение</span><span class="sxs-lookup"><span data-stu-id="647c2-155">Usage</span></span>

<span data-ttu-id="647c2-156">Вы можете отображать строку в кодировке Base 64 в HTML-теге изображения: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span><span class="sxs-lookup"><span data-stu-id="647c2-156">You can display the base-64 string inside an HTML image tag: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span></span>

<span data-ttu-id="647c2-157">В случае поведения по умолчанию используйте `Image(width=0,height=0,fittingMode='fit')`.</span><span class="sxs-lookup"><span data-stu-id="647c2-157">For default behavior, use `Image(width=0,height=0,fittingMode='fit')`.</span></span> <span data-ttu-id="647c2-158">Ниже приведен пример изображения диаграммы, возвращаемого с параметрами по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="647c2-158">Here is an example of a chart image returned with the default parameters.</span></span>

![Изображение диаграммы Excel с высотой и шириной по умолчанию.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-default.png)

<span data-ttu-id="647c2-160">Если вы хотите настроить отображение этого изображения, укажите высоту, ширину и режим подгонки.</span><span class="sxs-lookup"><span data-stu-id="647c2-160">If you want to customize the display of the image, specify a height, width, and a fitting mode.</span></span> <span data-ttu-id="647c2-161">А вот как выглядит то же самое изображение диаграммы, если получить его с этими параметрами: `Image(width=500,height=500,fittingMode='Fill')`.</span><span class="sxs-lookup"><span data-stu-id="647c2-161">Here is what the same chart image looks like if you retrieve it with these parameters: `Image(width=500,height=500,fittingMode='Fill')`.</span></span>

![Изображение диаграммы Excel с высотой и шириной по умолчанию.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-fill.png)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Chart: Image",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


