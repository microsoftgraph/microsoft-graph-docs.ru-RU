---
title: Обновление объекта chartaxistitle
description: Обновление свойств объекта chartaxistitle.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 7da47f47c595ce4807d986507af8f74e5f7bf94d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36331989"
---
# <a name="update-chartaxistitle"></a><span data-ttu-id="d2ea2-103">Обновление объекта chartaxistitle</span><span class="sxs-lookup"><span data-stu-id="d2ea2-103">Update chartaxistitle</span></span>

<span data-ttu-id="d2ea2-104">Обновление свойств объекта chartaxistitle.</span><span class="sxs-lookup"><span data-stu-id="d2ea2-104">Update the properties of chartaxistitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d2ea2-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d2ea2-105">Permissions</span></span>
<span data-ttu-id="d2ea2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2ea2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2ea2-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2ea2-108">Permission type</span></span>      | <span data-ttu-id="d2ea2-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2ea2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2ea2-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2ea2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d2ea2-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d2ea2-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d2ea2-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2ea2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2ea2-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2ea2-113">Not supported.</span></span>    |
|<span data-ttu-id="d2ea2-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d2ea2-114">Application</span></span> | <span data-ttu-id="d2ea2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2ea2-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2ea2-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2ea2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/title
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/title
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="d2ea2-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d2ea2-117">Optional request headers</span></span>
| <span data-ttu-id="d2ea2-118">Имя</span><span class="sxs-lookup"><span data-stu-id="d2ea2-118">Name</span></span>       | <span data-ttu-id="d2ea2-119">Описание</span><span class="sxs-lookup"><span data-stu-id="d2ea2-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d2ea2-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d2ea2-120">Authorization</span></span>  | <span data-ttu-id="d2ea2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2ea2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d2ea2-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d2ea2-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="d2ea2-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="d2ea2-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2ea2-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d2ea2-126">Request body</span></span>
<span data-ttu-id="d2ea2-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="d2ea2-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d2ea2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d2ea2-130">Property</span></span>     | <span data-ttu-id="d2ea2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d2ea2-131">Type</span></span>   |<span data-ttu-id="d2ea2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d2ea2-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d2ea2-133">text</span><span class="sxs-lookup"><span data-stu-id="d2ea2-133">text</span></span>|<span data-ttu-id="d2ea2-134">string</span><span class="sxs-lookup"><span data-stu-id="d2ea2-134">string</span></span>|<span data-ttu-id="d2ea2-135">Обозначает название оси.</span><span class="sxs-lookup"><span data-stu-id="d2ea2-135">Represents the axis title.</span></span>|
|<span data-ttu-id="d2ea2-136">visible</span><span class="sxs-lookup"><span data-stu-id="d2ea2-136">visible</span></span>|<span data-ttu-id="d2ea2-137">boolean</span><span class="sxs-lookup"><span data-stu-id="d2ea2-137">boolean</span></span>|<span data-ttu-id="d2ea2-138">Логическое значение, которое определяет видимость названия оси.</span><span class="sxs-lookup"><span data-stu-id="d2ea2-138">A boolean that specifies the visibility of an axis title.</span></span>|

## <a name="response"></a><span data-ttu-id="d2ea2-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2ea2-139">Response</span></span>

<span data-ttu-id="d2ea2-140">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [воркбукчартаксиститле](../resources/chartaxistitle.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d2ea2-140">If successful, this method returns a `200 OK` response code and updated [WorkbookChartAxisTitle](../resources/chartaxistitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d2ea2-141">Пример</span><span class="sxs-lookup"><span data-stu-id="d2ea2-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d2ea2-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2ea2-142">Request</span></span>
<span data-ttu-id="d2ea2-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d2ea2-143">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d2ea2-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="d2ea2-144">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="d2ea2-145">C#</span><span class="sxs-lookup"><span data-stu-id="d2ea2-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chartaxistitle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d2ea2-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d2ea2-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chartaxistitle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d2ea2-147">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d2ea2-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chartaxistitle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d2ea2-148">Java</span><span class="sxs-lookup"><span data-stu-id="d2ea2-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-chartaxistitle-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d2ea2-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2ea2-149">Response</span></span>
<span data-ttu-id="d2ea2-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d2ea2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
