---
title: Обновление объекта ChartTitle
description: Обновление свойств объекта charttitle.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 55cf1e0bfaede185c963db6b343bf2ed48d88848
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50574932"
---
# <a name="update-charttitle"></a><span data-ttu-id="e86a0-103">Обновление объекта ChartTitle</span><span class="sxs-lookup"><span data-stu-id="e86a0-103">Update charttitle</span></span>

<span data-ttu-id="e86a0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e86a0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e86a0-105">Обновление свойств объекта charttitle.</span><span class="sxs-lookup"><span data-stu-id="e86a0-105">Update the properties of charttitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e86a0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e86a0-106">Permissions</span></span>
<span data-ttu-id="e86a0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e86a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e86a0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e86a0-109">Permission type</span></span>      | <span data-ttu-id="e86a0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e86a0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e86a0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e86a0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e86a0-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e86a0-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e86a0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e86a0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e86a0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e86a0-114">Not supported.</span></span>    |
|<span data-ttu-id="e86a0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e86a0-115">Application</span></span> | <span data-ttu-id="e86a0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e86a0-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e86a0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e86a0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/title
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="e86a0-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e86a0-118">Optional request headers</span></span>
| <span data-ttu-id="e86a0-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e86a0-119">Name</span></span>       | <span data-ttu-id="e86a0-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e86a0-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e86a0-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e86a0-121">Authorization</span></span>  | <span data-ttu-id="e86a0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e86a0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e86a0-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e86a0-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="e86a0-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="e86a0-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e86a0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e86a0-127">Request body</span></span>
<span data-ttu-id="e86a0-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="e86a0-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e86a0-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="e86a0-131">Property</span></span>     | <span data-ttu-id="e86a0-132">Тип</span><span class="sxs-lookup"><span data-stu-id="e86a0-132">Type</span></span>   |<span data-ttu-id="e86a0-133">Описание</span><span class="sxs-lookup"><span data-stu-id="e86a0-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e86a0-134">overlay</span><span class="sxs-lookup"><span data-stu-id="e86a0-134">overlay</span></span>|<span data-ttu-id="e86a0-135">boolean</span><span class="sxs-lookup"><span data-stu-id="e86a0-135">boolean</span></span>|<span data-ttu-id="e86a0-136">Логическое значение, указывающее, отображается ли заголовок диаграммы поверх нее.</span><span class="sxs-lookup"><span data-stu-id="e86a0-136">Boolean value representing if the chart title will overlay the chart or not.</span></span>|
|<span data-ttu-id="e86a0-137">text</span><span class="sxs-lookup"><span data-stu-id="e86a0-137">text</span></span>|<span data-ttu-id="e86a0-138">string</span><span class="sxs-lookup"><span data-stu-id="e86a0-138">string</span></span>|<span data-ttu-id="e86a0-139">Представляет текст заголовка диаграммы.</span><span class="sxs-lookup"><span data-stu-id="e86a0-139">Represents the title text of a chart.</span></span>|
|<span data-ttu-id="e86a0-140">visible</span><span class="sxs-lookup"><span data-stu-id="e86a0-140">visible</span></span>|<span data-ttu-id="e86a0-141">boolean</span><span class="sxs-lookup"><span data-stu-id="e86a0-141">boolean</span></span>|<span data-ttu-id="e86a0-142">Логическое значение, представляющее видимость объекта заголовка диаграммы.</span><span class="sxs-lookup"><span data-stu-id="e86a0-142">A boolean value the represents the visibility of a chart title object.</span></span>|

## <a name="response"></a><span data-ttu-id="e86a0-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="e86a0-143">Response</span></span>

<span data-ttu-id="e86a0-144">В случае успешной работы этот метод возвращает код ответа и обновленный объект `200 OK` [WorkbookChartTitle](../resources/charttitle.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e86a0-144">If successful, this method returns a `200 OK` response code and updated [WorkbookChartTitle](../resources/charttitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e86a0-145">Пример</span><span class="sxs-lookup"><span data-stu-id="e86a0-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e86a0-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="e86a0-146">Request</span></span>
<span data-ttu-id="e86a0-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e86a0-147">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e86a0-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="e86a0-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_charttitle"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/title
Content-type: application/json
Content-length: 64

{
  "overlay": true,
  "text": "text-value",
  "visible": true
}
```
# <a name="c"></a>[<span data-ttu-id="e86a0-149">C#</span><span class="sxs-lookup"><span data-stu-id="e86a0-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-charttitle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e86a0-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e86a0-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-charttitle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e86a0-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e86a0-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-charttitle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e86a0-152">Java</span><span class="sxs-lookup"><span data-stu-id="e86a0-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-charttitle-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e86a0-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="e86a0-153">Response</span></span>
<span data-ttu-id="e86a0-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e86a0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartTitle"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 64

{
  "overlay": true,
  "text": "text-value",
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update charttitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

