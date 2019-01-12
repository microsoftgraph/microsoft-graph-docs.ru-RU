---
title: 'ChartCollection: add'
description: Создает диаграмму.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 19ab5936b563fc491e08923d257d334d9932af98
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936580"
---
# <a name="chartcollection-add"></a><span data-ttu-id="29d70-103">ChartCollection: add</span><span class="sxs-lookup"><span data-stu-id="29d70-103">ChartCollection: add</span></span>

> <span data-ttu-id="29d70-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="29d70-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="29d70-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29d70-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="29d70-106">Создает диаграмму.</span><span class="sxs-lookup"><span data-stu-id="29d70-106">Creates a new chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="29d70-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="29d70-107">Permissions</span></span>
<span data-ttu-id="29d70-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29d70-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29d70-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="29d70-110">Permission type</span></span>      | <span data-ttu-id="29d70-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="29d70-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="29d70-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="29d70-112">Delegated (work or school account)</span></span> | <span data-ttu-id="29d70-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="29d70-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="29d70-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="29d70-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29d70-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="29d70-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="29d70-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="29d70-116">Application</span></span> | <span data-ttu-id="29d70-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29d70-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="29d70-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="29d70-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/add

```
## <a name="request-headers"></a><span data-ttu-id="29d70-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="29d70-119">Request headers</span></span>
| <span data-ttu-id="29d70-120">Имя</span><span class="sxs-lookup"><span data-stu-id="29d70-120">Name</span></span>       | <span data-ttu-id="29d70-121">Описание</span><span class="sxs-lookup"><span data-stu-id="29d70-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="29d70-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="29d70-122">Authorization</span></span>  | <span data-ttu-id="29d70-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="29d70-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="29d70-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="29d70-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="29d70-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="29d70-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="29d70-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="29d70-128">Request body</span></span>
<span data-ttu-id="29d70-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="29d70-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="29d70-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="29d70-130">Parameter</span></span>    | <span data-ttu-id="29d70-131">Тип</span><span class="sxs-lookup"><span data-stu-id="29d70-131">Type</span></span>   |<span data-ttu-id="29d70-132">Описание</span><span class="sxs-lookup"><span data-stu-id="29d70-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="29d70-133">type</span><span class="sxs-lookup"><span data-stu-id="29d70-133">type</span></span>|<span data-ttu-id="29d70-134">строка</span><span class="sxs-lookup"><span data-stu-id="29d70-134">string</span></span>|<span data-ttu-id="29d70-p105">Представляет тип диаграммы.  Возможные значения: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie`, `etc.`.</span><span class="sxs-lookup"><span data-stu-id="29d70-p105">Represents the type of a chart.  Possible values are: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie`, `etc.`.</span></span>|
|<span data-ttu-id="29d70-137">sourceData</span><span class="sxs-lookup"><span data-stu-id="29d70-137">sourceData</span></span>|<span data-ttu-id="29d70-138">строка</span><span class="sxs-lookup"><span data-stu-id="29d70-138">string</span></span>|<span data-ttu-id="29d70-139">Объект Range, соответствующий исходным данным.</span><span class="sxs-lookup"><span data-stu-id="29d70-139">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="29d70-140">seriesBy</span><span class="sxs-lookup"><span data-stu-id="29d70-140">seriesBy</span></span>|<span data-ttu-id="29d70-141">строка</span><span class="sxs-lookup"><span data-stu-id="29d70-141">string</span></span>|<span data-ttu-id="29d70-p106">Необязательный параметр. Определяет способ использования столбцов или строк в качестве рядов данных на диаграмме.  Возможные значения: `Auto`, `Columns`, `Rows`.</span><span class="sxs-lookup"><span data-stu-id="29d70-p106">Optional. Specifies the way columns or rows are used as data series on the chart.  Possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="29d70-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="29d70-145">Response</span></span>

<span data-ttu-id="29d70-146">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Chart](../resources/chart.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="29d70-146">If successful, this method returns `200 OK` response code and [Chart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29d70-147">Пример</span><span class="sxs-lookup"><span data-stu-id="29d70-147">Example</span></span>
<span data-ttu-id="29d70-148">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="29d70-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="29d70-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="29d70-149">Request</span></span>
<span data-ttu-id="29d70-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="29d70-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartcollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/add
Content-type: application/json
Content-length: 94

{
  "type": "ColumnStacked",
  "sourceData": "A1:B1",
  "seriesBy": "Auto"
}
```

##### <a name="response"></a><span data-ttu-id="29d70-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="29d70-151">Response</span></span>
<span data-ttu-id="29d70-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="29d70-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chart"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
