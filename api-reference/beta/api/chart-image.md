---
title: 'Chart: Image'
description: Отрисовывает диаграмму в виде изображения с кодировкой Base64, масштабируя ее в соответствии с указанным размером.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: e82f0600cb43ba515bfb8bee9ecde90e645ea062
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328156"
---
# <a name="chart-image"></a><span data-ttu-id="16e04-103">Chart: Image</span><span class="sxs-lookup"><span data-stu-id="16e04-103">Chart: Image</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16e04-104">Отрисовывает диаграмму в виде изображения с кодировкой Base64, масштабируя ее в соответствии с указанным размером.</span><span class="sxs-lookup"><span data-stu-id="16e04-104">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>
## <a name="permissions"></a><span data-ttu-id="16e04-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="16e04-105">Permissions</span></span>
<span data-ttu-id="16e04-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16e04-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16e04-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16e04-108">Permission type</span></span>      | <span data-ttu-id="16e04-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="16e04-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16e04-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16e04-110">Delegated (work or school account)</span></span> | <span data-ttu-id="16e04-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="16e04-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="16e04-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16e04-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16e04-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="16e04-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="16e04-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="16e04-114">Application</span></span> | <span data-ttu-id="16e04-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16e04-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="16e04-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16e04-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/Image(width=0,height=0,fittingMode='fit')

```
## <a name="request-headers"></a><span data-ttu-id="16e04-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="16e04-117">Request headers</span></span>
| <span data-ttu-id="16e04-118">Имя</span><span class="sxs-lookup"><span data-stu-id="16e04-118">Name</span></span>       | <span data-ttu-id="16e04-119">Описание</span><span class="sxs-lookup"><span data-stu-id="16e04-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="16e04-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="16e04-120">Authorization</span></span>  | <span data-ttu-id="16e04-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="16e04-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="16e04-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="16e04-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="16e04-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="16e04-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="16e04-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="16e04-126">Request body</span></span>
<span data-ttu-id="16e04-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="16e04-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="16e04-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="16e04-128">Parameter</span></span>    | <span data-ttu-id="16e04-129">Тип</span><span class="sxs-lookup"><span data-stu-id="16e04-129">Type</span></span>   |<span data-ttu-id="16e04-130">Описание</span><span class="sxs-lookup"><span data-stu-id="16e04-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="16e04-131">height</span><span class="sxs-lookup"><span data-stu-id="16e04-131">height</span></span>|<span data-ttu-id="16e04-132">число</span><span class="sxs-lookup"><span data-stu-id="16e04-132">number</span></span>|<span data-ttu-id="16e04-p104">Необязательный. Нужная высота создаваемого изображения.</span><span class="sxs-lookup"><span data-stu-id="16e04-p104">Optional. The desired height of the resulting image.</span></span>|
|<span data-ttu-id="16e04-135">width</span><span class="sxs-lookup"><span data-stu-id="16e04-135">width</span></span>|<span data-ttu-id="16e04-136">number</span><span class="sxs-lookup"><span data-stu-id="16e04-136">number</span></span>|<span data-ttu-id="16e04-p105">Необязательный. Нужная ширина создаваемого изображения.</span><span class="sxs-lookup"><span data-stu-id="16e04-p105">Optional. The desired width of the resulting image.</span></span>|
|<span data-ttu-id="16e04-139">fittingMode</span><span class="sxs-lookup"><span data-stu-id="16e04-139">fittingMode</span></span>|<span data-ttu-id="16e04-140">string</span><span class="sxs-lookup"><span data-stu-id="16e04-140">string</span></span>|<span data-ttu-id="16e04-p106">Необязательный. Метод, используемый для масштабирования диаграммы до указанного размера (если указаны и высота, и ширина).  Возможные значения: `Fit`, `FitAndCenter`, `Fill`.</span><span class="sxs-lookup"><span data-stu-id="16e04-p106">Optional. The method used to scale the chart to the specified to the specified dimensions (if both height and width are set)."  Possible values are: `Fit`, `FitAndCenter`, `Fill`.</span></span>|

## <a name="response"></a><span data-ttu-id="16e04-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="16e04-144">Response</span></span>

<span data-ttu-id="16e04-145">В случае успеха этот метод возвращает код отклика `200 OK` и строку изображения с кодировкой base-64 в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="16e04-145">If successful, this method returns `200 OK` response code and base-64 image string in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16e04-146">Пример</span><span class="sxs-lookup"><span data-stu-id="16e04-146">Example</span></span>
<span data-ttu-id="16e04-147">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="16e04-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="16e04-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="16e04-148">Request</span></span>
<span data-ttu-id="16e04-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="16e04-149">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/Image(width=0,height=0,fittingMode='fit')
```

##### <a name="response"></a><span data-ttu-id="16e04-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="16e04-150">Response</span></span>
<span data-ttu-id="16e04-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="16e04-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call. </span></span><!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 3

{
"value" : "base-64 chart image string"
}
```

##### <a name="usage"></a><span data-ttu-id="16e04-154">Применение</span><span class="sxs-lookup"><span data-stu-id="16e04-154">Usage</span></span>

<span data-ttu-id="16e04-155">Вы можете обеспечить отображение строки Base64 в теге изображения HTML: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span><span class="sxs-lookup"><span data-stu-id="16e04-155">You can display the base-64 string inside an HTML image tag: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span></span>

<span data-ttu-id="16e04-156">В случае поведения по умолчанию используйте `Image(width=0,height=0,fittingMode='fit')`.</span><span class="sxs-lookup"><span data-stu-id="16e04-156">For default behavior, use `Image(width=0,height=0,fittingMode='fit')`.</span></span> <span data-ttu-id="16e04-157">Ниже приведен пример изображения диаграммы, возвращаемого с параметрами по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="16e04-157">Here is an example of a chart image returned with the default parameters.</span></span>

![Изображение диаграммы Excel с высотой и шириной по умолчанию.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-default.png)

<span data-ttu-id="16e04-159">Если вы хотите настроить отображение этого изображения, укажите высоту, ширину и режим подгонки.</span><span class="sxs-lookup"><span data-stu-id="16e04-159">If you want to customize the display of the image, specify a height, width, and a fitting mode.</span></span> <span data-ttu-id="16e04-160">Ниже показано то же изображение диаграммы, но с такими параметрами: `Image(width=500,height=500,fittingMode='Fill')`.</span><span class="sxs-lookup"><span data-stu-id="16e04-160">Here is what the same chart image looks like if you retrieve it with these parameters: `Image(width=500,height=500,fittingMode='Fill')`.</span></span>

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
