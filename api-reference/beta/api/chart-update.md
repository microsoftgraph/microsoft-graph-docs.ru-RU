---
title: Обновление диаграммы
description: Обновление свойств объекта диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 2d1377a0a8c19538ea1c0c19483512736e129559
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516387"
---
# <a name="update-chart"></a><span data-ttu-id="e7eb9-103">Обновление диаграммы</span><span class="sxs-lookup"><span data-stu-id="e7eb9-103">Update chart</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7eb9-104">Обновление свойств объекта диаграммы.</span><span class="sxs-lookup"><span data-stu-id="e7eb9-104">Update the properties of chart object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e7eb9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e7eb9-105">Permissions</span></span>
<span data-ttu-id="e7eb9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7eb9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7eb9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e7eb9-108">Permission type</span></span>      | <span data-ttu-id="e7eb9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e7eb9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7eb9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e7eb9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e7eb9-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e7eb9-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e7eb9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e7eb9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7eb9-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e7eb9-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e7eb9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e7eb9-114">Application</span></span> | <span data-ttu-id="e7eb9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7eb9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e7eb9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e7eb9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)
```
## <a name="optional-request-headers"></a><span data-ttu-id="e7eb9-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e7eb9-117">Optional request headers</span></span>
| <span data-ttu-id="e7eb9-118">Имя</span><span class="sxs-lookup"><span data-stu-id="e7eb9-118">Name</span></span>       | <span data-ttu-id="e7eb9-119">Описание</span><span class="sxs-lookup"><span data-stu-id="e7eb9-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e7eb9-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e7eb9-120">Authorization</span></span>  | <span data-ttu-id="e7eb9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e7eb9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e7eb9-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e7eb9-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="e7eb9-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="e7eb9-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7eb9-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e7eb9-126">Request body</span></span>
<span data-ttu-id="e7eb9-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="e7eb9-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e7eb9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e7eb9-130">Property</span></span>     | <span data-ttu-id="e7eb9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e7eb9-131">Type</span></span>   |<span data-ttu-id="e7eb9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e7eb9-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e7eb9-133">height</span><span class="sxs-lookup"><span data-stu-id="e7eb9-133">height</span></span>|<span data-ttu-id="e7eb9-134">double</span><span class="sxs-lookup"><span data-stu-id="e7eb9-134">double</span></span>|<span data-ttu-id="e7eb9-135">Обозначает высоту объекта диаграммы (в пунктах).</span><span class="sxs-lookup"><span data-stu-id="e7eb9-135">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="e7eb9-136">left</span><span class="sxs-lookup"><span data-stu-id="e7eb9-136">left</span></span>|<span data-ttu-id="e7eb9-137">double</span><span class="sxs-lookup"><span data-stu-id="e7eb9-137">double</span></span>|<span data-ttu-id="e7eb9-138">Расстояние в пунктах от левого края диаграммы до начала листа.</span><span class="sxs-lookup"><span data-stu-id="e7eb9-138">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="e7eb9-139">name</span><span class="sxs-lookup"><span data-stu-id="e7eb9-139">name</span></span>|<span data-ttu-id="e7eb9-140">строка</span><span class="sxs-lookup"><span data-stu-id="e7eb9-140">string</span></span>|<span data-ttu-id="e7eb9-141">Обозначает имя объекта диаграммы.</span><span class="sxs-lookup"><span data-stu-id="e7eb9-141">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="e7eb9-142">top</span><span class="sxs-lookup"><span data-stu-id="e7eb9-142">top</span></span>|<span data-ttu-id="e7eb9-143">double</span><span class="sxs-lookup"><span data-stu-id="e7eb9-143">double</span></span>|<span data-ttu-id="e7eb9-144">Представляет расстояние в пунктах от верхнего края объекта до верхнего края первой строки (на листе) или до верхнего края области диаграммы (на диаграмме).</span><span class="sxs-lookup"><span data-stu-id="e7eb9-144">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="e7eb9-145">width</span><span class="sxs-lookup"><span data-stu-id="e7eb9-145">width</span></span>|<span data-ttu-id="e7eb9-146">double</span><span class="sxs-lookup"><span data-stu-id="e7eb9-146">double</span></span>|<span data-ttu-id="e7eb9-147">Представляет ширину объекта диаграммы (в пунктах).</span><span class="sxs-lookup"><span data-stu-id="e7eb9-147">Represents the width, in points, of the chart object.</span></span>|

## <a name="response"></a><span data-ttu-id="e7eb9-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7eb9-148">Response</span></span>

<span data-ttu-id="e7eb9-149">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [Chart](../resources/chart.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e7eb9-149">If successful, this method returns a `200 OK` response code and updated [Chart](../resources/chart.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e7eb9-150">Пример</span><span class="sxs-lookup"><span data-stu-id="e7eb9-150">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e7eb9-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="e7eb9-151">Request</span></span>
<span data-ttu-id="e7eb9-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e7eb9-152">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chart"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)
Content-type: application/json
Content-length: 52

{
  "height": 99,
  "left": 99
}
```
##### <a name="response"></a><span data-ttu-id="e7eb9-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="e7eb9-153">Response</span></span>
<span data-ttu-id="e7eb9-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="e7eb9-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update chart",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chart-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
