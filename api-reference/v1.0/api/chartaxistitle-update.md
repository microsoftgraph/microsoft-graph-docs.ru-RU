---
title: Обновление объекта chartaxistitle
description: Обновление свойств объекта chartaxistitle.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 4a8624031ce1acb51485729d6d5b79bdccd06637
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48059903"
---
# <a name="update-chartaxistitle"></a><span data-ttu-id="e2afd-103">Обновление объекта chartaxistitle</span><span class="sxs-lookup"><span data-stu-id="e2afd-103">Update chartaxistitle</span></span>

<span data-ttu-id="e2afd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2afd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e2afd-105">Обновление свойств объекта chartaxistitle.</span><span class="sxs-lookup"><span data-stu-id="e2afd-105">Update the properties of chartaxistitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e2afd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e2afd-106">Permissions</span></span>
<span data-ttu-id="e2afd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2afd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2afd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e2afd-109">Permission type</span></span>      | <span data-ttu-id="e2afd-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e2afd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2afd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e2afd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e2afd-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e2afd-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e2afd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e2afd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2afd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2afd-114">Not supported.</span></span>    |
|<span data-ttu-id="e2afd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e2afd-115">Application</span></span> | <span data-ttu-id="e2afd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2afd-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2afd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e2afd-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/title
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/title
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="e2afd-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e2afd-118">Optional request headers</span></span>
| <span data-ttu-id="e2afd-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e2afd-119">Name</span></span>       | <span data-ttu-id="e2afd-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e2afd-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e2afd-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e2afd-121">Authorization</span></span>  | <span data-ttu-id="e2afd-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e2afd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e2afd-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e2afd-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="e2afd-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="e2afd-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2afd-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e2afd-127">Request body</span></span>
<span data-ttu-id="e2afd-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="e2afd-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e2afd-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="e2afd-131">Property</span></span>     | <span data-ttu-id="e2afd-132">Тип</span><span class="sxs-lookup"><span data-stu-id="e2afd-132">Type</span></span>   |<span data-ttu-id="e2afd-133">Описание</span><span class="sxs-lookup"><span data-stu-id="e2afd-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e2afd-134">text</span><span class="sxs-lookup"><span data-stu-id="e2afd-134">text</span></span>|<span data-ttu-id="e2afd-135">string</span><span class="sxs-lookup"><span data-stu-id="e2afd-135">string</span></span>|<span data-ttu-id="e2afd-136">Обозначает название оси.</span><span class="sxs-lookup"><span data-stu-id="e2afd-136">Represents the axis title.</span></span>|
|<span data-ttu-id="e2afd-137">visible</span><span class="sxs-lookup"><span data-stu-id="e2afd-137">visible</span></span>|<span data-ttu-id="e2afd-138">boolean</span><span class="sxs-lookup"><span data-stu-id="e2afd-138">boolean</span></span>|<span data-ttu-id="e2afd-139">Логическое значение, которое определяет видимость названия оси.</span><span class="sxs-lookup"><span data-stu-id="e2afd-139">A boolean that specifies the visibility of an axis title.</span></span>|

## <a name="response"></a><span data-ttu-id="e2afd-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2afd-140">Response</span></span>

<span data-ttu-id="e2afd-141">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [воркбукчартаксиститле](../resources/chartaxistitle.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e2afd-141">If successful, this method returns a `200 OK` response code and updated [WorkbookChartAxisTitle](../resources/chartaxistitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e2afd-142">Пример</span><span class="sxs-lookup"><span data-stu-id="e2afd-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e2afd-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="e2afd-143">Request</span></span>
<span data-ttu-id="e2afd-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e2afd-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e2afd-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="e2afd-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_chartaxistitle"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/title
Content-type: application/json
Content-length: 45

{
  "text": "text-value",
  "visible": true
}
```
# <a name="c"></a>[<span data-ttu-id="e2afd-146">C#</span><span class="sxs-lookup"><span data-stu-id="e2afd-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chartaxistitle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e2afd-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e2afd-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chartaxistitle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e2afd-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e2afd-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chartaxistitle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e2afd-149">Java</span><span class="sxs-lookup"><span data-stu-id="e2afd-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-chartaxistitle-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e2afd-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2afd-150">Response</span></span>
<span data-ttu-id="e2afd-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e2afd-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update chartaxistitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

