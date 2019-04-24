---
title: Обновление объекта chartlegend
description: Обновление свойств объекта chartlegend.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 83c46208edf769a2c3d3a97d242b874596d3308d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456094"
---
# <a name="update-chartlegend"></a><span data-ttu-id="5cdbe-103">Обновление объекта chartlegend</span><span class="sxs-lookup"><span data-stu-id="5cdbe-103">Update chartlegend</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5cdbe-104">Обновление свойств объекта chartlegend.</span><span class="sxs-lookup"><span data-stu-id="5cdbe-104">Update the properties of chartlegend object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5cdbe-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5cdbe-105">Permissions</span></span>
<span data-ttu-id="5cdbe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5cdbe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5cdbe-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5cdbe-108">Permission type</span></span>      | <span data-ttu-id="5cdbe-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5cdbe-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5cdbe-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5cdbe-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5cdbe-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5cdbe-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5cdbe-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5cdbe-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5cdbe-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5cdbe-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5cdbe-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5cdbe-114">Application</span></span> | <span data-ttu-id="5cdbe-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5cdbe-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5cdbe-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5cdbe-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/legend
```
## <a name="optional-request-headers"></a><span data-ttu-id="5cdbe-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5cdbe-117">Optional request headers</span></span>
| <span data-ttu-id="5cdbe-118">Имя</span><span class="sxs-lookup"><span data-stu-id="5cdbe-118">Name</span></span>       | <span data-ttu-id="5cdbe-119">Описание</span><span class="sxs-lookup"><span data-stu-id="5cdbe-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="5cdbe-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5cdbe-120">Authorization</span></span>  | <span data-ttu-id="5cdbe-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5cdbe-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5cdbe-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5cdbe-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="5cdbe-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="5cdbe-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5cdbe-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5cdbe-126">Request body</span></span>
<span data-ttu-id="5cdbe-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="5cdbe-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5cdbe-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5cdbe-130">Property</span></span>     | <span data-ttu-id="5cdbe-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5cdbe-131">Type</span></span>   |<span data-ttu-id="5cdbe-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5cdbe-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5cdbe-133">overlay</span><span class="sxs-lookup"><span data-stu-id="5cdbe-133">overlay</span></span>|<span data-ttu-id="5cdbe-134">boolean</span><span class="sxs-lookup"><span data-stu-id="5cdbe-134">boolean</span></span>|<span data-ttu-id="5cdbe-135">Логическое значение, определяющее, должна ли легенда диаграммы пересекаться с основной частью диаграммы.</span><span class="sxs-lookup"><span data-stu-id="5cdbe-135">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="5cdbe-136">position</span><span class="sxs-lookup"><span data-stu-id="5cdbe-136">position</span></span>|<span data-ttu-id="5cdbe-137">string</span><span class="sxs-lookup"><span data-stu-id="5cdbe-137">string</span></span>|<span data-ttu-id="5cdbe-p105">Представляет расположение легенды на диаграмме. Возможные значения: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span><span class="sxs-lookup"><span data-stu-id="5cdbe-p105">Represents the position of the legend on the chart. Possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="5cdbe-140">visible</span><span class="sxs-lookup"><span data-stu-id="5cdbe-140">visible</span></span>|<span data-ttu-id="5cdbe-141">boolean</span><span class="sxs-lookup"><span data-stu-id="5cdbe-141">boolean</span></span>|<span data-ttu-id="5cdbe-142">Логическое значение, представляющее видимость объекта ChartLegend.</span><span class="sxs-lookup"><span data-stu-id="5cdbe-142">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="response"></a><span data-ttu-id="5cdbe-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="5cdbe-143">Response</span></span>

<span data-ttu-id="5cdbe-144">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [ChartLegend](../resources/chartlegend.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5cdbe-144">If successful, this method returns a `200 OK` response code and updated [ChartLegend](../resources/chartlegend.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5cdbe-145">Пример</span><span class="sxs-lookup"><span data-stu-id="5cdbe-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5cdbe-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="5cdbe-146">Request</span></span>
<span data-ttu-id="5cdbe-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5cdbe-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartlegend"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/legend
Content-type: application/json
Content-length: 72

{
  "visible": true,
  "position": "position-value",
  "overlay": true
}
```
##### <a name="response"></a><span data-ttu-id="5cdbe-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="5cdbe-148">Response</span></span>
<span data-ttu-id="5cdbe-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5cdbe-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartLegend"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "visible": true,
  "position": "position-value",
  "overlay": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update chartlegend",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chartlegend-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
