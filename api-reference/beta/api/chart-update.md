---
title: Обновление диаграммы
description: Обновление свойств объекта диаграммы.
author: lumine2008
ms.openlocfilehash: 086d4a2ea0ce823ace141df0d5576af732bf8c0f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328184"
---
# <a name="update-chart"></a><span data-ttu-id="273bc-103">Обновление диаграммы</span><span class="sxs-lookup"><span data-stu-id="273bc-103">Update chart</span></span>

> <span data-ttu-id="273bc-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="273bc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="273bc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="273bc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="273bc-106">Обновление свойств объекта диаграммы.</span><span class="sxs-lookup"><span data-stu-id="273bc-106">Update the properties of chart object.</span></span>
## <a name="permissions"></a><span data-ttu-id="273bc-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="273bc-107">Permissions</span></span>
<span data-ttu-id="273bc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="273bc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="273bc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="273bc-110">Permission type</span></span>      | <span data-ttu-id="273bc-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="273bc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="273bc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="273bc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="273bc-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="273bc-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="273bc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="273bc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="273bc-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="273bc-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="273bc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="273bc-116">Application</span></span> | <span data-ttu-id="273bc-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="273bc-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="273bc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="273bc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)
```
## <a name="optional-request-headers"></a><span data-ttu-id="273bc-119">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="273bc-119">Optional request headers</span></span>
| <span data-ttu-id="273bc-120">Имя</span><span class="sxs-lookup"><span data-stu-id="273bc-120">Name</span></span>       | <span data-ttu-id="273bc-121">Описание</span><span class="sxs-lookup"><span data-stu-id="273bc-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="273bc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="273bc-122">Authorization</span></span>  | <span data-ttu-id="273bc-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="273bc-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="273bc-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="273bc-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="273bc-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="273bc-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="273bc-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="273bc-128">Request body</span></span>
<span data-ttu-id="273bc-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="273bc-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="273bc-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="273bc-132">Property</span></span>     | <span data-ttu-id="273bc-133">Тип</span><span class="sxs-lookup"><span data-stu-id="273bc-133">Type</span></span>   |<span data-ttu-id="273bc-134">Описание</span><span class="sxs-lookup"><span data-stu-id="273bc-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="273bc-135">height</span><span class="sxs-lookup"><span data-stu-id="273bc-135">height</span></span>|<span data-ttu-id="273bc-136">double</span><span class="sxs-lookup"><span data-stu-id="273bc-136">double</span></span>|<span data-ttu-id="273bc-137">Обозначает высоту объекта диаграммы (в пунктах).</span><span class="sxs-lookup"><span data-stu-id="273bc-137">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="273bc-138">left</span><span class="sxs-lookup"><span data-stu-id="273bc-138">left</span></span>|<span data-ttu-id="273bc-139">double</span><span class="sxs-lookup"><span data-stu-id="273bc-139">double</span></span>|<span data-ttu-id="273bc-140">Расстояние в пунктах от левого края диаграммы до начала листа.</span><span class="sxs-lookup"><span data-stu-id="273bc-140">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="273bc-141">name</span><span class="sxs-lookup"><span data-stu-id="273bc-141">name</span></span>|<span data-ttu-id="273bc-142">строка</span><span class="sxs-lookup"><span data-stu-id="273bc-142">string</span></span>|<span data-ttu-id="273bc-143">Обозначает имя объекта диаграммы.</span><span class="sxs-lookup"><span data-stu-id="273bc-143">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="273bc-144">top</span><span class="sxs-lookup"><span data-stu-id="273bc-144">top</span></span>|<span data-ttu-id="273bc-145">double</span><span class="sxs-lookup"><span data-stu-id="273bc-145">double</span></span>|<span data-ttu-id="273bc-146">Представляет расстояние в пунктах от верхнего края объекта до верхнего края первой строки (на листе) или до верхнего края области диаграммы (на диаграмме).</span><span class="sxs-lookup"><span data-stu-id="273bc-146">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="273bc-147">width</span><span class="sxs-lookup"><span data-stu-id="273bc-147">width</span></span>|<span data-ttu-id="273bc-148">double</span><span class="sxs-lookup"><span data-stu-id="273bc-148">double</span></span>|<span data-ttu-id="273bc-149">Представляет ширину объекта диаграммы (в пунктах).</span><span class="sxs-lookup"><span data-stu-id="273bc-149">Represents the width, in points, of the chart object.</span></span>|

## <a name="response"></a><span data-ttu-id="273bc-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="273bc-150">Response</span></span>

<span data-ttu-id="273bc-151">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [Chart](../resources/chart.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="273bc-151">If successful, this method returns a `200 OK` response code and updated [Chart](../resources/chart.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="273bc-152">Пример</span><span class="sxs-lookup"><span data-stu-id="273bc-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="273bc-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="273bc-153">Request</span></span>
<span data-ttu-id="273bc-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="273bc-154">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="273bc-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="273bc-155">Response</span></span>
<span data-ttu-id="273bc-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="273bc-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Update chart",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->