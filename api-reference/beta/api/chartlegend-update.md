---
title: Обновление объекта chartlegend
description: Обновление свойств объекта chartlegend.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 03bcd9ce5d5c15f624dd0eaa231f8965137c210e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946632"
---
# <a name="update-chartlegend"></a><span data-ttu-id="85a52-103">Обновление объекта chartlegend</span><span class="sxs-lookup"><span data-stu-id="85a52-103">Update chartlegend</span></span>

> <span data-ttu-id="85a52-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="85a52-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="85a52-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85a52-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="85a52-106">Обновление свойств объекта chartlegend.</span><span class="sxs-lookup"><span data-stu-id="85a52-106">Update the properties of chartlegend object.</span></span>
## <a name="permissions"></a><span data-ttu-id="85a52-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="85a52-107">Permissions</span></span>
<span data-ttu-id="85a52-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85a52-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85a52-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="85a52-110">Permission type</span></span>      | <span data-ttu-id="85a52-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="85a52-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="85a52-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85a52-112">Delegated (work or school account)</span></span> | <span data-ttu-id="85a52-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="85a52-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="85a52-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85a52-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85a52-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="85a52-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="85a52-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="85a52-116">Application</span></span> | <span data-ttu-id="85a52-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85a52-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="85a52-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85a52-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/legend
```
## <a name="optional-request-headers"></a><span data-ttu-id="85a52-119">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="85a52-119">Optional request headers</span></span>
| <span data-ttu-id="85a52-120">Имя</span><span class="sxs-lookup"><span data-stu-id="85a52-120">Name</span></span>       | <span data-ttu-id="85a52-121">Описание</span><span class="sxs-lookup"><span data-stu-id="85a52-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="85a52-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="85a52-122">Authorization</span></span>  | <span data-ttu-id="85a52-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="85a52-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="85a52-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="85a52-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="85a52-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="85a52-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="85a52-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="85a52-128">Request body</span></span>
<span data-ttu-id="85a52-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="85a52-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="85a52-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="85a52-132">Property</span></span>     | <span data-ttu-id="85a52-133">Тип</span><span class="sxs-lookup"><span data-stu-id="85a52-133">Type</span></span>   |<span data-ttu-id="85a52-134">Описание</span><span class="sxs-lookup"><span data-stu-id="85a52-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="85a52-135">overlay</span><span class="sxs-lookup"><span data-stu-id="85a52-135">overlay</span></span>|<span data-ttu-id="85a52-136">boolean</span><span class="sxs-lookup"><span data-stu-id="85a52-136">boolean</span></span>|<span data-ttu-id="85a52-137">Логическое значение, определяющее, должна ли легенда диаграммы пересекаться с основной частью диаграммы.</span><span class="sxs-lookup"><span data-stu-id="85a52-137">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="85a52-138">position</span><span class="sxs-lookup"><span data-stu-id="85a52-138">position</span></span>|<span data-ttu-id="85a52-139">string</span><span class="sxs-lookup"><span data-stu-id="85a52-139">string</span></span>|<span data-ttu-id="85a52-p106">Представляет расположение легенды на диаграмме. Возможные значения: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span><span class="sxs-lookup"><span data-stu-id="85a52-p106">Represents the position of the legend on the chart. Possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="85a52-142">visible</span><span class="sxs-lookup"><span data-stu-id="85a52-142">visible</span></span>|<span data-ttu-id="85a52-143">boolean</span><span class="sxs-lookup"><span data-stu-id="85a52-143">boolean</span></span>|<span data-ttu-id="85a52-144">Логическое значение, представляющее видимость объекта ChartLegend.</span><span class="sxs-lookup"><span data-stu-id="85a52-144">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="response"></a><span data-ttu-id="85a52-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="85a52-145">Response</span></span>

<span data-ttu-id="85a52-146">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [ChartLegend](../resources/chartlegend.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="85a52-146">If successful, this method returns a `200 OK` response code and updated [ChartLegend](../resources/chartlegend.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="85a52-147">Пример</span><span class="sxs-lookup"><span data-stu-id="85a52-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="85a52-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="85a52-148">Request</span></span>
<span data-ttu-id="85a52-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="85a52-149">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="85a52-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="85a52-150">Response</span></span>
<span data-ttu-id="85a52-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="85a52-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update chartlegend",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
