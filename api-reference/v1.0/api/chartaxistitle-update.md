---
title: Обновление объекта chartaxistitle
description: Обновление свойств объекта chartaxistitle.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 07503fd8a90aecdf07737ddf0cf2c11438777a51
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048829"
---
# <a name="update-chartaxistitle"></a><span data-ttu-id="794c5-103">Обновление объекта chartaxistitle</span><span class="sxs-lookup"><span data-stu-id="794c5-103">Update chartaxistitle</span></span>

<span data-ttu-id="794c5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="794c5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="794c5-105">Обновление свойств объекта chartaxistitle.</span><span class="sxs-lookup"><span data-stu-id="794c5-105">Update the properties of chartaxistitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="794c5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="794c5-106">Permissions</span></span>
<span data-ttu-id="794c5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="794c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="794c5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="794c5-109">Permission type</span></span>      | <span data-ttu-id="794c5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="794c5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="794c5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="794c5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="794c5-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="794c5-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="794c5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="794c5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="794c5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="794c5-114">Not supported.</span></span>    |
|<span data-ttu-id="794c5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="794c5-115">Application</span></span> | <span data-ttu-id="794c5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="794c5-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="794c5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="794c5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/title
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/title
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/title
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/title
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/title
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="794c5-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="794c5-118">Optional request headers</span></span>
| <span data-ttu-id="794c5-119">Имя</span><span class="sxs-lookup"><span data-stu-id="794c5-119">Name</span></span>       | <span data-ttu-id="794c5-120">Описание</span><span class="sxs-lookup"><span data-stu-id="794c5-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="794c5-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="794c5-121">Authorization</span></span>  | <span data-ttu-id="794c5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="794c5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="794c5-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="794c5-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="794c5-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="794c5-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="794c5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="794c5-127">Request body</span></span>
<span data-ttu-id="794c5-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="794c5-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="794c5-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="794c5-131">Property</span></span>     | <span data-ttu-id="794c5-132">Тип</span><span class="sxs-lookup"><span data-stu-id="794c5-132">Type</span></span>   |<span data-ttu-id="794c5-133">Описание</span><span class="sxs-lookup"><span data-stu-id="794c5-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="794c5-134">text</span><span class="sxs-lookup"><span data-stu-id="794c5-134">text</span></span>|<span data-ttu-id="794c5-135">string</span><span class="sxs-lookup"><span data-stu-id="794c5-135">string</span></span>|<span data-ttu-id="794c5-136">Обозначает название оси.</span><span class="sxs-lookup"><span data-stu-id="794c5-136">Represents the axis title.</span></span>|
|<span data-ttu-id="794c5-137">visible</span><span class="sxs-lookup"><span data-stu-id="794c5-137">visible</span></span>|<span data-ttu-id="794c5-138">boolean</span><span class="sxs-lookup"><span data-stu-id="794c5-138">boolean</span></span>|<span data-ttu-id="794c5-139">Логическое значение, которое определяет видимость названия оси.</span><span class="sxs-lookup"><span data-stu-id="794c5-139">A boolean that specifies the visibility of an axis title.</span></span>|

## <a name="response"></a><span data-ttu-id="794c5-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="794c5-140">Response</span></span>

<span data-ttu-id="794c5-141">В случае успешной работы этот метод возвращает код ответа и обновленный объект `200 OK` [WorkbookChartAxisTitle](../resources/chartaxistitle.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="794c5-141">If successful, this method returns a `200 OK` response code and updated [WorkbookChartAxisTitle](../resources/chartaxistitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="794c5-142">Пример</span><span class="sxs-lookup"><span data-stu-id="794c5-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="794c5-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="794c5-143">Request</span></span>
<span data-ttu-id="794c5-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="794c5-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="794c5-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="794c5-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="794c5-146">C#</span><span class="sxs-lookup"><span data-stu-id="794c5-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chartaxistitle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="794c5-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="794c5-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chartaxistitle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="794c5-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="794c5-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chartaxistitle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="794c5-149">Java</span><span class="sxs-lookup"><span data-stu-id="794c5-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-chartaxistitle-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="794c5-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="794c5-150">Response</span></span>
<span data-ttu-id="794c5-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="794c5-151">Here is an example of the response.</span></span> <span data-ttu-id="794c5-152">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="794c5-152">Note: The response object shown here might be shortened for readability.</span></span>
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

