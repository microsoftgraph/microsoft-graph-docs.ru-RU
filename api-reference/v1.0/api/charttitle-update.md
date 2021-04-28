---
title: Обновление объекта ChartTitle
description: Обновление свойств объекта charttitle.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 84f7f6f074469f11986044575ccf45282ff4d581
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054093"
---
# <a name="update-charttitle"></a><span data-ttu-id="7c839-103">Обновление объекта ChartTitle</span><span class="sxs-lookup"><span data-stu-id="7c839-103">Update charttitle</span></span>

<span data-ttu-id="7c839-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c839-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7c839-105">Обновление свойств объекта charttitle.</span><span class="sxs-lookup"><span data-stu-id="7c839-105">Update the properties of charttitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7c839-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7c839-106">Permissions</span></span>
<span data-ttu-id="7c839-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c839-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c839-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7c839-109">Permission type</span></span>      | <span data-ttu-id="7c839-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7c839-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7c839-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7c839-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7c839-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c839-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7c839-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7c839-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c839-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c839-114">Not supported.</span></span>    |
|<span data-ttu-id="7c839-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7c839-115">Application</span></span> | <span data-ttu-id="7c839-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c839-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7c839-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7c839-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/title
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="7c839-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7c839-118">Optional request headers</span></span>
| <span data-ttu-id="7c839-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7c839-119">Name</span></span>       | <span data-ttu-id="7c839-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7c839-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="7c839-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7c839-121">Authorization</span></span>  | <span data-ttu-id="7c839-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7c839-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7c839-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7c839-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="7c839-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="7c839-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c839-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7c839-127">Request body</span></span>
<span data-ttu-id="7c839-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="7c839-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7c839-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="7c839-131">Property</span></span>     | <span data-ttu-id="7c839-132">Тип</span><span class="sxs-lookup"><span data-stu-id="7c839-132">Type</span></span>   |<span data-ttu-id="7c839-133">Описание</span><span class="sxs-lookup"><span data-stu-id="7c839-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7c839-134">overlay</span><span class="sxs-lookup"><span data-stu-id="7c839-134">overlay</span></span>|<span data-ttu-id="7c839-135">boolean</span><span class="sxs-lookup"><span data-stu-id="7c839-135">boolean</span></span>|<span data-ttu-id="7c839-136">Логическое значение, указывающее, отображается ли заголовок диаграммы поверх нее.</span><span class="sxs-lookup"><span data-stu-id="7c839-136">Boolean value representing if the chart title will overlay the chart or not.</span></span>|
|<span data-ttu-id="7c839-137">text</span><span class="sxs-lookup"><span data-stu-id="7c839-137">text</span></span>|<span data-ttu-id="7c839-138">string</span><span class="sxs-lookup"><span data-stu-id="7c839-138">string</span></span>|<span data-ttu-id="7c839-139">Представляет текст заголовка диаграммы.</span><span class="sxs-lookup"><span data-stu-id="7c839-139">Represents the title text of a chart.</span></span>|
|<span data-ttu-id="7c839-140">visible</span><span class="sxs-lookup"><span data-stu-id="7c839-140">visible</span></span>|<span data-ttu-id="7c839-141">boolean</span><span class="sxs-lookup"><span data-stu-id="7c839-141">boolean</span></span>|<span data-ttu-id="7c839-142">Логическое значение, представляющее видимость объекта заголовка диаграммы.</span><span class="sxs-lookup"><span data-stu-id="7c839-142">A boolean value the represents the visibility of a chart title object.</span></span>|

## <a name="response"></a><span data-ttu-id="7c839-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c839-143">Response</span></span>

<span data-ttu-id="7c839-144">В случае успешной работы этот метод возвращает код ответа и обновленный объект `200 OK` [WorkbookChartTitle](../resources/charttitle.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7c839-144">If successful, this method returns a `200 OK` response code and updated [WorkbookChartTitle](../resources/charttitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7c839-145">Пример</span><span class="sxs-lookup"><span data-stu-id="7c839-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7c839-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="7c839-146">Request</span></span>
<span data-ttu-id="7c839-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7c839-147">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7c839-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="7c839-148">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7c839-149">C#</span><span class="sxs-lookup"><span data-stu-id="7c839-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-charttitle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7c839-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7c839-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-charttitle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7c839-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7c839-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-charttitle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7c839-152">Java</span><span class="sxs-lookup"><span data-stu-id="7c839-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-charttitle-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7c839-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c839-153">Response</span></span>
<span data-ttu-id="7c839-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7c839-154">Here is an example of the response.</span></span> <span data-ttu-id="7c839-155">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7c839-155">Note: The response object shown here might be shortened for readability.</span></span>
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

