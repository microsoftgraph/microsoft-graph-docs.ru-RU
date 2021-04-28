---
title: Обновление объекта ChartLineFormat
description: Обновление свойств объекта chartlineformat.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 82e96562c4bd78e542e89b4e122dd7e5ab2626d1
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054170"
---
# <a name="update-chartlineformat"></a><span data-ttu-id="1da98-103">Обновление объекта ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="1da98-103">Update chartlineformat</span></span>

<span data-ttu-id="1da98-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1da98-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1da98-105">Обновление свойств объекта chartlineformat.</span><span class="sxs-lookup"><span data-stu-id="1da98-105">Update the properties of chartlineformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1da98-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1da98-106">Permissions</span></span>
<span data-ttu-id="1da98-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1da98-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1da98-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1da98-109">Permission type</span></span>      | <span data-ttu-id="1da98-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1da98-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1da98-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1da98-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1da98-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1da98-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1da98-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1da98-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1da98-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1da98-114">Not supported.</span></span>    |
|<span data-ttu-id="1da98-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1da98-115">Application</span></span> | <span data-ttu-id="1da98-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1da98-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1da98-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1da98-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/format/line
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/format/line
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/format/line
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/format/line
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/majorgridlines/format/line
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/majorgridlines/format/line
```
## <a name="optional-request-headers"></a><span data-ttu-id="1da98-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1da98-118">Optional request headers</span></span>
| <span data-ttu-id="1da98-119">Имя</span><span class="sxs-lookup"><span data-stu-id="1da98-119">Name</span></span>       | <span data-ttu-id="1da98-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1da98-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="1da98-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1da98-121">Authorization</span></span>  | <span data-ttu-id="1da98-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1da98-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1da98-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1da98-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="1da98-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="1da98-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1da98-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1da98-127">Request body</span></span>
<span data-ttu-id="1da98-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="1da98-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1da98-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="1da98-131">Property</span></span>     | <span data-ttu-id="1da98-132">Тип</span><span class="sxs-lookup"><span data-stu-id="1da98-132">Type</span></span>   |<span data-ttu-id="1da98-133">Описание</span><span class="sxs-lookup"><span data-stu-id="1da98-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1da98-134">color</span><span class="sxs-lookup"><span data-stu-id="1da98-134">color</span></span>|<span data-ttu-id="1da98-135">string</span><span class="sxs-lookup"><span data-stu-id="1da98-135">string</span></span>|<span data-ttu-id="1da98-136">HTML-код цвета, представляющий цвет линий в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="1da98-136">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="response"></a><span data-ttu-id="1da98-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="1da98-137">Response</span></span>

<span data-ttu-id="1da98-138">В случае успешной работы этот метод возвращает код ответа и обновленный объект `200 OK` [WorkbookChartLineFormat](../resources/chartlineformat.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1da98-138">If successful, this method returns a `200 OK` response code and updated [WorkbookChartLineFormat](../resources/chartlineformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1da98-139">Пример</span><span class="sxs-lookup"><span data-stu-id="1da98-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1da98-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="1da98-140">Request</span></span>
<span data-ttu-id="1da98-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1da98-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1da98-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="1da98-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_chartlineformat"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/format/line
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```
# <a name="c"></a>[<span data-ttu-id="1da98-143">C#</span><span class="sxs-lookup"><span data-stu-id="1da98-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chartlineformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1da98-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1da98-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chartlineformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1da98-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1da98-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chartlineformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1da98-146">Java</span><span class="sxs-lookup"><span data-stu-id="1da98-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-chartlineformat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1da98-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="1da98-147">Response</span></span>
<span data-ttu-id="1da98-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1da98-148">Here is an example of the response.</span></span> <span data-ttu-id="1da98-149">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1da98-149">Note: The response object shown here might be shortened for readability.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update chartlineformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

