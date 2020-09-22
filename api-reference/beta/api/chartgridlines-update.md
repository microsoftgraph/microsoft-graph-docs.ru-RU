---
title: Обновление объекта chartgridlines
description: Обновление свойств объекта chartgridlines.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 1556b66782281db417527c4fe35f5c5c5cb36bd6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47982950"
---
# <a name="update-chartgridlines"></a><span data-ttu-id="9e426-103">Обновление объекта chartgridlines</span><span class="sxs-lookup"><span data-stu-id="9e426-103">Update chartgridlines</span></span>

<span data-ttu-id="9e426-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e426-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e426-105">Обновление свойств объекта chartgridlines.</span><span class="sxs-lookup"><span data-stu-id="9e426-105">Update the properties of chartgridlines object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9e426-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9e426-106">Permissions</span></span>
<span data-ttu-id="9e426-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e426-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e426-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9e426-109">Permission type</span></span>      | <span data-ttu-id="9e426-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9e426-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9e426-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9e426-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9e426-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9e426-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9e426-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9e426-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e426-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9e426-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9e426-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9e426-115">Application</span></span> | <span data-ttu-id="9e426-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e426-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9e426-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9e426-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/minorgridlines
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/majorgridlines
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/majorgridlines
```
## <a name="optional-request-headers"></a><span data-ttu-id="9e426-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9e426-118">Optional request headers</span></span>
| <span data-ttu-id="9e426-119">Имя</span><span class="sxs-lookup"><span data-stu-id="9e426-119">Name</span></span>       | <span data-ttu-id="9e426-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9e426-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="9e426-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9e426-121">Authorization</span></span>  | <span data-ttu-id="9e426-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9e426-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9e426-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9e426-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="9e426-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="9e426-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e426-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9e426-127">Request body</span></span>
<span data-ttu-id="9e426-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="9e426-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9e426-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="9e426-131">Property</span></span>     | <span data-ttu-id="9e426-132">Тип</span><span class="sxs-lookup"><span data-stu-id="9e426-132">Type</span></span>   |<span data-ttu-id="9e426-133">Описание</span><span class="sxs-lookup"><span data-stu-id="9e426-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9e426-134">visible</span><span class="sxs-lookup"><span data-stu-id="9e426-134">visible</span></span>|<span data-ttu-id="9e426-135">boolean</span><span class="sxs-lookup"><span data-stu-id="9e426-135">boolean</span></span>|<span data-ttu-id="9e426-136">Логическое значение, определяющее, отображаются ли линии сетки оси.</span><span class="sxs-lookup"><span data-stu-id="9e426-136">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="response"></a><span data-ttu-id="9e426-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e426-137">Response</span></span>

<span data-ttu-id="9e426-138">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [воркбукчартгридлинес](../resources/workbookchartgridlines.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9e426-138">If successful, this method returns a `200 OK` response code and updated [workbookChartGridlines](../resources/workbookchartgridlines.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9e426-139">Пример</span><span class="sxs-lookup"><span data-stu-id="9e426-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9e426-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="9e426-140">Request</span></span>
<span data-ttu-id="9e426-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9e426-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9e426-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="9e426-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_chartgridlines"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/minorgridlines
Content-type: application/json
Content-length: 21

{
  "visible": true
}
```
# <a name="c"></a>[<span data-ttu-id="9e426-143">C#</span><span class="sxs-lookup"><span data-stu-id="9e426-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chartgridlines-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9e426-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9e426-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chartgridlines-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9e426-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9e426-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chartgridlines-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9e426-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e426-146">Response</span></span>
<span data-ttu-id="9e426-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9e426-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartGridlines"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 21

{
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update chartgridlines",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


