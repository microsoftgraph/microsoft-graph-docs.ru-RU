---
title: Обновление объекта chartlegend
description: Обновление свойств объекта chartlegend.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: bdd765cebe86015bdd01ef42c9db829a89c7749f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930259"
---
# <a name="update-chartlegend"></a><span data-ttu-id="4b80f-103">Обновление объекта chartlegend</span><span class="sxs-lookup"><span data-stu-id="4b80f-103">Update chartlegend</span></span>

<span data-ttu-id="4b80f-104">Обновление свойств объекта chartlegend.</span><span class="sxs-lookup"><span data-stu-id="4b80f-104">Update the properties of chartlegend object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4b80f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4b80f-105">Permissions</span></span>
<span data-ttu-id="4b80f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b80f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b80f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b80f-108">Permission type</span></span>      | <span data-ttu-id="4b80f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b80f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b80f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b80f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4b80f-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4b80f-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4b80f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b80f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b80f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b80f-113">Not supported.</span></span>    |
|<span data-ttu-id="4b80f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4b80f-114">Application</span></span> | <span data-ttu-id="4b80f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b80f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b80f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b80f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/legend
```
## <a name="optional-request-headers"></a><span data-ttu-id="4b80f-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4b80f-117">Optional request headers</span></span>
| <span data-ttu-id="4b80f-118">Имя</span><span class="sxs-lookup"><span data-stu-id="4b80f-118">Name</span></span>       | <span data-ttu-id="4b80f-119">Описание</span><span class="sxs-lookup"><span data-stu-id="4b80f-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="4b80f-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4b80f-120">Authorization</span></span>  | <span data-ttu-id="4b80f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b80f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4b80f-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4b80f-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="4b80f-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="4b80f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b80f-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4b80f-126">Request body</span></span>
<span data-ttu-id="4b80f-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="4b80f-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4b80f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b80f-130">Property</span></span>     | <span data-ttu-id="4b80f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4b80f-131">Type</span></span>   |<span data-ttu-id="4b80f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4b80f-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4b80f-133">overlay</span><span class="sxs-lookup"><span data-stu-id="4b80f-133">overlay</span></span>|<span data-ttu-id="4b80f-134">boolean</span><span class="sxs-lookup"><span data-stu-id="4b80f-134">boolean</span></span>|<span data-ttu-id="4b80f-135">Логическое значение, определяющее, должна ли легенда диаграммы пересекаться с основной частью диаграммы.</span><span class="sxs-lookup"><span data-stu-id="4b80f-135">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="4b80f-136">position</span><span class="sxs-lookup"><span data-stu-id="4b80f-136">position</span></span>|<span data-ttu-id="4b80f-137">строка</span><span class="sxs-lookup"><span data-stu-id="4b80f-137">string</span></span>|<span data-ttu-id="4b80f-138">Представляет положение легенды диаграммы.</span><span class="sxs-lookup"><span data-stu-id="4b80f-138">Represents the position of the legend on the chart.</span></span> <span data-ttu-id="4b80f-139">Возможные значения: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span><span class="sxs-lookup"><span data-stu-id="4b80f-139">The possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="4b80f-140">visible</span><span class="sxs-lookup"><span data-stu-id="4b80f-140">visible</span></span>|<span data-ttu-id="4b80f-141">boolean</span><span class="sxs-lookup"><span data-stu-id="4b80f-141">boolean</span></span>|<span data-ttu-id="4b80f-142">Логическое значение, представляющее видимость объекта ChartLegend.</span><span class="sxs-lookup"><span data-stu-id="4b80f-142">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="response"></a><span data-ttu-id="4b80f-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b80f-143">Response</span></span>

<span data-ttu-id="4b80f-144">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленный объект [WorkbookChartLegend](../resources/chartlegend.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4b80f-144">If successful, this method returns a `200 OK` response code and updated [WorkbookChartLegend](../resources/chartlegend.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4b80f-145">Пример</span><span class="sxs-lookup"><span data-stu-id="4b80f-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4b80f-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b80f-146">Request</span></span>
<span data-ttu-id="4b80f-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b80f-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartlegend"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/legend
Content-type: application/json
Content-length: 72

{
  "visible": true,
  "position": "position-value",
  "overlay": true
}
```
##### <a name="response"></a><span data-ttu-id="4b80f-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="4b80f-148">Response</span></span>
<span data-ttu-id="4b80f-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4b80f-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartLegend"
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
<!-- {
  "type": "#page.annotation",
  "description": "Update chartlegend",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
