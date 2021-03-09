---
title: Обновление объекта ChartLineFormat
description: Обновление свойств объекта chartlineformat.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: f959390fc226dd0b85152585e3c848b002fcd290
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50574477"
---
# <a name="update-chartlineformat"></a><span data-ttu-id="59b09-103">Обновление объекта ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="59b09-103">Update chartlineformat</span></span>

<span data-ttu-id="59b09-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59b09-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59b09-105">Обновление свойств объекта chartlineformat.</span><span class="sxs-lookup"><span data-stu-id="59b09-105">Update the properties of chartlineformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="59b09-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="59b09-106">Permissions</span></span>
<span data-ttu-id="59b09-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59b09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59b09-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="59b09-109">Permission type</span></span>      | <span data-ttu-id="59b09-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="59b09-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59b09-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="59b09-111">Delegated (work or school account)</span></span> | <span data-ttu-id="59b09-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59b09-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="59b09-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="59b09-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59b09-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59b09-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="59b09-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="59b09-115">Application</span></span> | <span data-ttu-id="59b09-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59b09-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="59b09-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="59b09-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/format/line
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/format/line
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/format/line
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/format/line
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/majorgridlines/format/line
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/majorgridlines/format/line
```
## <a name="optional-request-headers"></a><span data-ttu-id="59b09-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="59b09-118">Optional request headers</span></span>
| <span data-ttu-id="59b09-119">Имя</span><span class="sxs-lookup"><span data-stu-id="59b09-119">Name</span></span>       | <span data-ttu-id="59b09-120">Описание</span><span class="sxs-lookup"><span data-stu-id="59b09-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="59b09-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="59b09-121">Authorization</span></span>  | <span data-ttu-id="59b09-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="59b09-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="59b09-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="59b09-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="59b09-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="59b09-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="59b09-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="59b09-127">Request body</span></span>
<span data-ttu-id="59b09-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="59b09-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="59b09-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="59b09-131">Property</span></span>     | <span data-ttu-id="59b09-132">Тип</span><span class="sxs-lookup"><span data-stu-id="59b09-132">Type</span></span>   |<span data-ttu-id="59b09-133">Описание</span><span class="sxs-lookup"><span data-stu-id="59b09-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="59b09-134">color</span><span class="sxs-lookup"><span data-stu-id="59b09-134">color</span></span>|<span data-ttu-id="59b09-135">string</span><span class="sxs-lookup"><span data-stu-id="59b09-135">string</span></span>|<span data-ttu-id="59b09-136">HTML-код цвета, представляющий цвет линий в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="59b09-136">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="response"></a><span data-ttu-id="59b09-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="59b09-137">Response</span></span>

<span data-ttu-id="59b09-138">В случае успеха этот метод возвращает код ответа и обновленный объект `200 OK` [книгиChartLineFormat](../resources/workbookchartlineformat.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="59b09-138">If successful, this method returns a `200 OK` response code and updated [workbookChartLineFormat](../resources/workbookchartlineformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="59b09-139">Пример</span><span class="sxs-lookup"><span data-stu-id="59b09-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="59b09-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="59b09-140">Request</span></span>
<span data-ttu-id="59b09-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="59b09-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="59b09-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="59b09-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_chartlineformat"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/format/line
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```
# <a name="c"></a>[<span data-ttu-id="59b09-143">C#</span><span class="sxs-lookup"><span data-stu-id="59b09-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chartlineformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="59b09-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="59b09-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chartlineformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="59b09-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="59b09-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chartlineformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="59b09-146">Java</span><span class="sxs-lookup"><span data-stu-id="59b09-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-chartlineformat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="59b09-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="59b09-147">Response</span></span>
<span data-ttu-id="59b09-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="59b09-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartLineFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update chartlineformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


