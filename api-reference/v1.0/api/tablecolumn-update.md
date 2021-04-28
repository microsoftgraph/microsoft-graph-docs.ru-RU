---
title: Обновление объекта TableColumn
description: Обновление свойств объекта tablecolumn.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: dc69cc73bcc39dd2014ffa2d6074c8f601dd5d8d
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050278"
---
# <a name="update-tablecolumn"></a><span data-ttu-id="74ae7-103">Обновление объекта TableColumn</span><span class="sxs-lookup"><span data-stu-id="74ae7-103">Update tablecolumn</span></span>

<span data-ttu-id="74ae7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74ae7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="74ae7-105">Обновление свойств объекта tablecolumn.</span><span class="sxs-lookup"><span data-stu-id="74ae7-105">Update the properties of tablecolumn object.</span></span>
## <a name="permissions"></a><span data-ttu-id="74ae7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="74ae7-106">Permissions</span></span>
<span data-ttu-id="74ae7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74ae7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74ae7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="74ae7-109">Permission type</span></span>      | <span data-ttu-id="74ae7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="74ae7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="74ae7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="74ae7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="74ae7-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="74ae7-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="74ae7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="74ae7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74ae7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74ae7-114">Not supported.</span></span>    |
|<span data-ttu-id="74ae7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="74ae7-115">Application</span></span> | <span data-ttu-id="74ae7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74ae7-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="74ae7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="74ae7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}
PATCH /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="74ae7-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="74ae7-118">Optional request headers</span></span>
| <span data-ttu-id="74ae7-119">Имя</span><span class="sxs-lookup"><span data-stu-id="74ae7-119">Name</span></span>       | <span data-ttu-id="74ae7-120">Описание</span><span class="sxs-lookup"><span data-stu-id="74ae7-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="74ae7-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="74ae7-121">Authorization</span></span>  | <span data-ttu-id="74ae7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="74ae7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="74ae7-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="74ae7-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="74ae7-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="74ae7-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="74ae7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="74ae7-127">Request body</span></span>
<span data-ttu-id="74ae7-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="74ae7-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="74ae7-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="74ae7-131">Property</span></span>     | <span data-ttu-id="74ae7-132">Тип</span><span class="sxs-lookup"><span data-stu-id="74ae7-132">Type</span></span>   |<span data-ttu-id="74ae7-133">Описание</span><span class="sxs-lookup"><span data-stu-id="74ae7-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="74ae7-134">values</span><span class="sxs-lookup"><span data-stu-id="74ae7-134">values</span></span>|<span data-ttu-id="74ae7-135">Json</span><span class="sxs-lookup"><span data-stu-id="74ae7-135">Json</span></span>|<span data-ttu-id="74ae7-p105">Представляет необработанные значения указанного диапазона. Могут возвращаться строковые и числовые данные, а также логические значения. Ячейка, которая содержит ошибку, вернет строку ошибки.</span><span class="sxs-lookup"><span data-stu-id="74ae7-p105">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="74ae7-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="74ae7-139">Response</span></span>

<span data-ttu-id="74ae7-140">В случае успеха этот метод возвращает код ответа и обновленный объект `200 OK` [WorkbookTableColumn](../resources/workbooktablecolumn.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="74ae7-140">If successful, this method returns a `200 OK` response code and updated [WorkbookTableColumn](../resources/workbooktablecolumn.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="74ae7-141">Пример</span><span class="sxs-lookup"><span data-stu-id="74ae7-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="74ae7-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="74ae7-142">Request</span></span>
<span data-ttu-id="74ae7-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="74ae7-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="74ae7-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="74ae7-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_tablecolumn"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}
Content-type: application/json
Content-length: 81

{
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```
# <a name="c"></a>[<span data-ttu-id="74ae7-145">C#</span><span class="sxs-lookup"><span data-stu-id="74ae7-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tablecolumn-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="74ae7-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="74ae7-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tablecolumn-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="74ae7-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="74ae7-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tablecolumn-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="74ae7-148">Java</span><span class="sxs-lookup"><span data-stu-id="74ae7-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tablecolumn-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---
> [!NOTE]
> <span data-ttu-id="74ae7-149">Если необходимо обновить несколько полей столбца, сделайте **значения** строки массива в запросе.</span><span class="sxs-lookup"><span data-stu-id="74ae7-149">If you want to update multiple fields of a column, make **values** a string array in the request.</span></span> <span data-ttu-id="74ae7-150">Пример: `"values": [["a"], [1], [2], [3]]`.</span><span class="sxs-lookup"><span data-stu-id="74ae7-150">For example: `"values": [["a"], [1], [2], [3]]`.</span></span>

##### <a name="response"></a><span data-ttu-id="74ae7-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="74ae7-151">Response</span></span>
<span data-ttu-id="74ae7-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="74ae7-152">Here is an example of the response.</span></span> <span data-ttu-id="74ae7-153">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="74ae7-153">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableColumn"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 81

{
  "id": "99",
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update tablecolumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

