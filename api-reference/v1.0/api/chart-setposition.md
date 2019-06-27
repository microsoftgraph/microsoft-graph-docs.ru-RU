---
title: 'Chart: setPosition'
description: Располагает диаграмму относительно ячеек на листе.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: b3557eb8c6522b27f01949fd6cace5094d5f61d6
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35272613"
---
# <a name="chart-setposition"></a><span data-ttu-id="720cf-103">Chart: setPosition</span><span class="sxs-lookup"><span data-stu-id="720cf-103">Chart: setPosition</span></span>

<span data-ttu-id="720cf-104">Располагает диаграмму относительно ячеек на листе.</span><span class="sxs-lookup"><span data-stu-id="720cf-104">Positions the chart relative to cells on the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="720cf-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="720cf-105">Permissions</span></span>
<span data-ttu-id="720cf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="720cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="720cf-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="720cf-108">Permission type</span></span>      | <span data-ttu-id="720cf-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="720cf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="720cf-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="720cf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="720cf-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="720cf-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="720cf-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="720cf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="720cf-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="720cf-113">Not supported.</span></span>    |
|<span data-ttu-id="720cf-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="720cf-114">Application</span></span> | <span data-ttu-id="720cf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="720cf-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="720cf-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="720cf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/setPosition

```
## <a name="request-headers"></a><span data-ttu-id="720cf-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="720cf-117">Request headers</span></span>
| <span data-ttu-id="720cf-118">Имя</span><span class="sxs-lookup"><span data-stu-id="720cf-118">Name</span></span>       | <span data-ttu-id="720cf-119">Описание</span><span class="sxs-lookup"><span data-stu-id="720cf-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="720cf-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="720cf-120">Authorization</span></span>  | <span data-ttu-id="720cf-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="720cf-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="720cf-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="720cf-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="720cf-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="720cf-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="720cf-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="720cf-126">Request body</span></span>
<span data-ttu-id="720cf-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="720cf-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="720cf-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="720cf-128">Parameter</span></span>    | <span data-ttu-id="720cf-129">Тип</span><span class="sxs-lookup"><span data-stu-id="720cf-129">Type</span></span>   |<span data-ttu-id="720cf-130">Описание</span><span class="sxs-lookup"><span data-stu-id="720cf-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="720cf-131">startCell</span><span class="sxs-lookup"><span data-stu-id="720cf-131">startCell</span></span>|<span data-ttu-id="720cf-132">Json</span><span class="sxs-lookup"><span data-stu-id="720cf-132">Json</span></span>|<span data-ttu-id="720cf-p104">Начальная ячейка. Место, куда будет перемещена диаграмма. Начальная ячейка — это верхняя левая или верхняя правая ячейка (это зависит от того, использует ли пользователь параметры отображения справа налево).</span><span class="sxs-lookup"><span data-stu-id="720cf-p104">The start cell. This is where the chart will be moved to. The start cell is the top-left or top-right cell, depending on the user's right-to-left display settings.</span></span>|
|<span data-ttu-id="720cf-136">endCell</span><span class="sxs-lookup"><span data-stu-id="720cf-136">endCell</span></span>|<span data-ttu-id="720cf-137">Json</span><span class="sxs-lookup"><span data-stu-id="720cf-137">Json</span></span>|<span data-ttu-id="720cf-p105">Необязательный. Конечная ячейка. Если указан этот параметр, значения ширины и высоты диаграммы будут заданы так, чтобы полностью покрыть данную ячейку или диапазон.</span><span class="sxs-lookup"><span data-stu-id="720cf-p105">Optional. The end cell. If specified, the chart's width and height will be set to fully cover up this cell/range.</span></span>|

## <a name="response"></a><span data-ttu-id="720cf-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="720cf-141">Response</span></span>

<span data-ttu-id="720cf-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="720cf-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="720cf-144">Пример</span><span class="sxs-lookup"><span data-stu-id="720cf-144">Example</span></span>
<span data-ttu-id="720cf-145">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="720cf-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="720cf-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="720cf-146">Request</span></span>
<span data-ttu-id="720cf-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="720cf-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_setposition"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/setPosition
Content-type: application/json
Content-length: 66

{
  "startCell": "startCell-value",
  "endCell": "endCell-value"
}
```

##### <a name="response"></a><span data-ttu-id="720cf-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="720cf-148">Response</span></span>
<span data-ttu-id="720cf-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="720cf-149">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="720cf-150">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="720cf-150">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="720cf-151">C#</span><span class="sxs-lookup"><span data-stu-id="720cf-151">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/chart_setposition-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="720cf-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="720cf-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/chart_setposition-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="720cf-153">Цель — C</span><span class="sxs-lookup"><span data-stu-id="720cf-153">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/chart_setposition-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chart: setPosition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/chart-setposition.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/chart-setposition.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/chart-setposition.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
