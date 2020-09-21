---
title: Обновление Воркбукчартаксиститле
description: Обновление свойств объекта воркбукчартаксиститле.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: bf71ff93ed5ed3a539ce34a59c9f6ffff6ed378a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47983090"
---
# <a name="update-workbookchartaxistitle"></a><span data-ttu-id="0726d-103">Обновление Воркбукчартаксиститле</span><span class="sxs-lookup"><span data-stu-id="0726d-103">Update workbookChartAxisTitle</span></span>

<span data-ttu-id="0726d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0726d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0726d-105">Обновление свойств объекта Воркбукчартаксиститле.</span><span class="sxs-lookup"><span data-stu-id="0726d-105">Update the properties of workbookChartAxisTitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0726d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0726d-106">Permissions</span></span>
<span data-ttu-id="0726d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0726d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0726d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0726d-109">Permission type</span></span>      | <span data-ttu-id="0726d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0726d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0726d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0726d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0726d-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0726d-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0726d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0726d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0726d-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0726d-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0726d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0726d-115">Application</span></span> | <span data-ttu-id="0726d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0726d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0726d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0726d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/title
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/title
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="0726d-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0726d-118">Optional request headers</span></span>
| <span data-ttu-id="0726d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0726d-119">Name</span></span>       | <span data-ttu-id="0726d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0726d-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0726d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0726d-121">Authorization</span></span>  | <span data-ttu-id="0726d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0726d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0726d-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0726d-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="0726d-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="0726d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0726d-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0726d-127">Request body</span></span>
<span data-ttu-id="0726d-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="0726d-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0726d-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="0726d-131">Property</span></span>     | <span data-ttu-id="0726d-132">Тип</span><span class="sxs-lookup"><span data-stu-id="0726d-132">Type</span></span>   |<span data-ttu-id="0726d-133">Описание</span><span class="sxs-lookup"><span data-stu-id="0726d-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0726d-134">text</span><span class="sxs-lookup"><span data-stu-id="0726d-134">text</span></span>|<span data-ttu-id="0726d-135">string</span><span class="sxs-lookup"><span data-stu-id="0726d-135">string</span></span>|<span data-ttu-id="0726d-136">Обозначает название оси.</span><span class="sxs-lookup"><span data-stu-id="0726d-136">Represents the axis title.</span></span>|
|<span data-ttu-id="0726d-137">visible</span><span class="sxs-lookup"><span data-stu-id="0726d-137">visible</span></span>|<span data-ttu-id="0726d-138">boolean</span><span class="sxs-lookup"><span data-stu-id="0726d-138">boolean</span></span>|<span data-ttu-id="0726d-139">Логическое значение, которое определяет видимость названия оси.</span><span class="sxs-lookup"><span data-stu-id="0726d-139">A boolean that specifies the visibility of an axis title.</span></span>|

## <a name="response"></a><span data-ttu-id="0726d-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="0726d-140">Response</span></span>

<span data-ttu-id="0726d-141">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [воркбукчартаксиститле](../resources/workbookchartaxistitle.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0726d-141">If successful, this method returns a `200 OK` response code and updated [workbookChartAxisTitle](../resources/workbookchartaxistitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0726d-142">Пример</span><span class="sxs-lookup"><span data-stu-id="0726d-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0726d-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="0726d-143">Request</span></span>
<span data-ttu-id="0726d-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0726d-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0726d-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="0726d-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_chartaxistitle"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/title
Content-type: application/json
Content-length: 45

{
  "text": "text-value",
  "visible": true
}
```
# <a name="c"></a>[<span data-ttu-id="0726d-146">C#</span><span class="sxs-lookup"><span data-stu-id="0726d-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chartaxistitle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0726d-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0726d-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chartaxistitle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0726d-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0726d-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chartaxistitle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0726d-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="0726d-149">Response</span></span>
<span data-ttu-id="0726d-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0726d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartAxisTitle"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "text": "text-value",
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update chartaxistitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


