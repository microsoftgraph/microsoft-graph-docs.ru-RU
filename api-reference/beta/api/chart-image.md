---
title: 'Chart: Image'
description: Отрисовывает диаграмму в виде изображения с кодировкой Base64, масштабируя ее в соответствии с указанным размером.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 997948cbae8b8df135c01da20bf3b508c95eed97
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047520"
---
# <a name="chart-image"></a><span data-ttu-id="62c49-103">Chart: Image</span><span class="sxs-lookup"><span data-stu-id="62c49-103">Chart: Image</span></span>

<span data-ttu-id="62c49-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62c49-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62c49-105">Отрисовывает диаграмму в виде изображения с кодировкой Base64, масштабируя ее в соответствии с указанным размером.</span><span class="sxs-lookup"><span data-stu-id="62c49-105">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>
## <a name="permissions"></a><span data-ttu-id="62c49-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="62c49-106">Permissions</span></span>
<span data-ttu-id="62c49-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62c49-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62c49-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="62c49-109">Permission type</span></span>      | <span data-ttu-id="62c49-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="62c49-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="62c49-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="62c49-111">Delegated (work or school account)</span></span> | <span data-ttu-id="62c49-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="62c49-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="62c49-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="62c49-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62c49-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="62c49-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="62c49-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="62c49-115">Application</span></span> | <span data-ttu-id="62c49-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62c49-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="62c49-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="62c49-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/Image(width=0,height=0,fittingMode='fit')
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/Image(width=0,height=0,fittingMode='fit')

```
## <a name="request-headers"></a><span data-ttu-id="62c49-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="62c49-118">Request headers</span></span>
| <span data-ttu-id="62c49-119">Имя</span><span class="sxs-lookup"><span data-stu-id="62c49-119">Name</span></span>       | <span data-ttu-id="62c49-120">Описание</span><span class="sxs-lookup"><span data-stu-id="62c49-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="62c49-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="62c49-121">Authorization</span></span>  | <span data-ttu-id="62c49-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="62c49-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="62c49-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="62c49-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="62c49-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="62c49-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="62c49-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="62c49-127">Request body</span></span>
<span data-ttu-id="62c49-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="62c49-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="62c49-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="62c49-129">Parameter</span></span>    | <span data-ttu-id="62c49-130">Тип</span><span class="sxs-lookup"><span data-stu-id="62c49-130">Type</span></span>   |<span data-ttu-id="62c49-131">Описание</span><span class="sxs-lookup"><span data-stu-id="62c49-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="62c49-132">height</span><span class="sxs-lookup"><span data-stu-id="62c49-132">height</span></span>|<span data-ttu-id="62c49-133">number</span><span class="sxs-lookup"><span data-stu-id="62c49-133">number</span></span>|<span data-ttu-id="62c49-p104">Необязательный. Нужная высота создаваемого изображения.</span><span class="sxs-lookup"><span data-stu-id="62c49-p104">Optional. The desired height of the resulting image.</span></span>|
|<span data-ttu-id="62c49-136">width</span><span class="sxs-lookup"><span data-stu-id="62c49-136">width</span></span>|<span data-ttu-id="62c49-137">number</span><span class="sxs-lookup"><span data-stu-id="62c49-137">number</span></span>|<span data-ttu-id="62c49-p105">Необязательный. Нужная ширина создаваемого изображения.</span><span class="sxs-lookup"><span data-stu-id="62c49-p105">Optional. The desired width of the resulting image.</span></span>|
|<span data-ttu-id="62c49-140">fittingMode</span><span class="sxs-lookup"><span data-stu-id="62c49-140">fittingMode</span></span>|<span data-ttu-id="62c49-141">string</span><span class="sxs-lookup"><span data-stu-id="62c49-141">string</span></span>|<span data-ttu-id="62c49-p106">Необязательный. Метод, используемый для масштабирования диаграммы до указанного размера (если указаны и высота, и ширина).  Возможные значения: `Fit`, `FitAndCenter`, `Fill`.</span><span class="sxs-lookup"><span data-stu-id="62c49-p106">Optional. The method used to scale the chart to the specified to the specified dimensions (if both height and width are set)."  Possible values are: `Fit`, `FitAndCenter`, `Fill`.</span></span>|

## <a name="response"></a><span data-ttu-id="62c49-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="62c49-145">Response</span></span>

<span data-ttu-id="62c49-146">В случае успеха этот метод возвращает код отклика `200 OK` и строку изображения с кодировкой base-64 в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="62c49-146">If successful, this method returns `200 OK` response code and base-64 image string in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62c49-147">Пример</span><span class="sxs-lookup"><span data-stu-id="62c49-147">Example</span></span>
<span data-ttu-id="62c49-148">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="62c49-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="62c49-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="62c49-149">Request</span></span>
<span data-ttu-id="62c49-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="62c49-150">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/Image(width=0,height=0,fittingMode='fit')
```

##### <a name="response"></a><span data-ttu-id="62c49-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="62c49-151">Response</span></span>
<span data-ttu-id="62c49-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="62c49-152">Here is an example of the response.</span></span> <span data-ttu-id="62c49-153">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="62c49-153">Note: The response object shown here might be shortened for readability.</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 3

{
"value" : "base-64 chart image string"
}
```

##### <a name="usage"></a><span data-ttu-id="62c49-154">Применение</span><span class="sxs-lookup"><span data-stu-id="62c49-154">Usage</span></span>

<span data-ttu-id="62c49-155">Вы можете отображать строку в кодировке Base 64 в HTML-теге изображения: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span><span class="sxs-lookup"><span data-stu-id="62c49-155">You can display the base-64 string inside an HTML image tag: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span></span>

<span data-ttu-id="62c49-156">В случае поведения по умолчанию используйте `Image(width=0,height=0,fittingMode='fit')`.</span><span class="sxs-lookup"><span data-stu-id="62c49-156">For default behavior, use `Image(width=0,height=0,fittingMode='fit')`.</span></span> <span data-ttu-id="62c49-157">Ниже приведен пример изображения диаграммы, возвращаемого с параметрами по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="62c49-157">Here is an example of a chart image returned with the default parameters.</span></span>

![Изображение диаграммы Excel с высотой и шириной по умолчанию.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-default.png)

<span data-ttu-id="62c49-159">Если вы хотите настроить отображение этого изображения, укажите высоту, ширину и режим подгонки.</span><span class="sxs-lookup"><span data-stu-id="62c49-159">If you want to customize the display of the image, specify a height, width, and a fitting mode.</span></span> <span data-ttu-id="62c49-160">А вот как выглядит то же самое изображение диаграммы, если получить его с этими параметрами: `Image(width=500,height=500,fittingMode='Fill')`.</span><span class="sxs-lookup"><span data-stu-id="62c49-160">Here is what the same chart image looks like if you retrieve it with these parameters: `Image(width=500,height=500,fittingMode='Fill')`.</span></span>

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


