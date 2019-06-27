---
title: 'Chart: setData'
description: Сбрасывает исходные данные для диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: c7f95c83a2eeee77f66dd347b353a585fadbb16f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35261952"
---
# <a name="chart-setdata"></a><span data-ttu-id="608ec-103">Chart: setData</span><span class="sxs-lookup"><span data-stu-id="608ec-103">Chart: setData</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="608ec-104">Сбрасывает исходные данные для диаграммы.</span><span class="sxs-lookup"><span data-stu-id="608ec-104">Resets the source data for the chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="608ec-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="608ec-105">Permissions</span></span>
<span data-ttu-id="608ec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="608ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="608ec-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="608ec-108">Permission type</span></span>      | <span data-ttu-id="608ec-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="608ec-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="608ec-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="608ec-110">Delegated (work or school account)</span></span> | <span data-ttu-id="608ec-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="608ec-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="608ec-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="608ec-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="608ec-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="608ec-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="608ec-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="608ec-114">Application</span></span> | <span data-ttu-id="608ec-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="608ec-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="608ec-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="608ec-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/setData

```
## <a name="request-headers"></a><span data-ttu-id="608ec-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="608ec-117">Request headers</span></span>
| <span data-ttu-id="608ec-118">Имя</span><span class="sxs-lookup"><span data-stu-id="608ec-118">Name</span></span>       | <span data-ttu-id="608ec-119">Описание</span><span class="sxs-lookup"><span data-stu-id="608ec-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="608ec-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="608ec-120">Authorization</span></span>  | <span data-ttu-id="608ec-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="608ec-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="608ec-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="608ec-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="608ec-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="608ec-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="608ec-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="608ec-126">Request body</span></span>
<span data-ttu-id="608ec-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="608ec-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="608ec-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="608ec-128">Parameter</span></span>    | <span data-ttu-id="608ec-129">Тип</span><span class="sxs-lookup"><span data-stu-id="608ec-129">Type</span></span>   |<span data-ttu-id="608ec-130">Описание</span><span class="sxs-lookup"><span data-stu-id="608ec-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="608ec-131">sourceData</span><span class="sxs-lookup"><span data-stu-id="608ec-131">sourceData</span></span>|<span data-ttu-id="608ec-132">string</span><span class="sxs-lookup"><span data-stu-id="608ec-132">string</span></span>|<span data-ttu-id="608ec-133">Объект Range, соответствующий исходным данным.</span><span class="sxs-lookup"><span data-stu-id="608ec-133">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="608ec-134">seriesBy</span><span class="sxs-lookup"><span data-stu-id="608ec-134">seriesBy</span></span>|<span data-ttu-id="608ec-135">string</span><span class="sxs-lookup"><span data-stu-id="608ec-135">string</span></span>|<span data-ttu-id="608ec-p104">Необязательный параметр. Определяет способ использования столбцов или строк в качестве рядов данных на диаграмме. Может иметь одно из следующих значений: Auto (по умолчанию), Rows, Columns.  Возможные значения: `Auto`, `Columns`, `Rows`.</span><span class="sxs-lookup"><span data-stu-id="608ec-p104">Optional. Specifies the way columns or rows are used as data series on the chart. Can be one of the following: Auto (default), Rows, Columns.  Possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="608ec-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="608ec-140">Response</span></span>

<span data-ttu-id="608ec-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="608ec-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="608ec-143">Пример</span><span class="sxs-lookup"><span data-stu-id="608ec-143">Example</span></span>
<span data-ttu-id="608ec-144">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="608ec-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="608ec-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="608ec-145">Request</span></span>
<span data-ttu-id="608ec-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="608ec-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_setdata"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/setData
Content-type: application/json
Content-length: 70

{
  "sourceData": "sourceData-value",
  "seriesBy": "seriesBy-value"
}
```

##### <a name="response"></a><span data-ttu-id="608ec-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="608ec-147">Response</span></span>
<span data-ttu-id="608ec-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="608ec-148">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="608ec-149">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="608ec-149">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="608ec-150">C#</span><span class="sxs-lookup"><span data-stu-id="608ec-150">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/chart_setdata-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="608ec-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="608ec-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/chart_setdata-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="608ec-152">Цель — C</span><span class="sxs-lookup"><span data-stu-id="608ec-152">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/chart_setdata-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Chart: setData",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chart-setdata.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/chart-setdata.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/chart-setdata.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
