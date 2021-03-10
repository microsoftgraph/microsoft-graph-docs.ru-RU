---
title: Обновление объекта TableColumn
description: Обновление свойств объекта tablecolumn.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 634861ae08d2ed85593e46fa56f31ce6c5b23b21
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50575506"
---
# <a name="update-tablecolumn"></a><span data-ttu-id="dacec-103">Обновление объекта TableColumn</span><span class="sxs-lookup"><span data-stu-id="dacec-103">Update tablecolumn</span></span>

<span data-ttu-id="dacec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dacec-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dacec-105">Обновление свойств объекта tablecolumn.</span><span class="sxs-lookup"><span data-stu-id="dacec-105">Update the properties of tablecolumn object.</span></span>
## <a name="permissions"></a><span data-ttu-id="dacec-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dacec-106">Permissions</span></span>
<span data-ttu-id="dacec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dacec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dacec-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dacec-109">Permission type</span></span>      | <span data-ttu-id="dacec-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dacec-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dacec-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dacec-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dacec-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dacec-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dacec-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dacec-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dacec-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dacec-114">Not supported.</span></span>    |
|<span data-ttu-id="dacec-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dacec-115">Application</span></span> | <span data-ttu-id="dacec-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dacec-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dacec-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dacec-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}
PATCH /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="dacec-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dacec-118">Optional request headers</span></span>
| <span data-ttu-id="dacec-119">Имя</span><span class="sxs-lookup"><span data-stu-id="dacec-119">Name</span></span>       | <span data-ttu-id="dacec-120">Описание</span><span class="sxs-lookup"><span data-stu-id="dacec-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="dacec-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dacec-121">Authorization</span></span>  | <span data-ttu-id="dacec-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dacec-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dacec-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="dacec-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="dacec-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="dacec-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dacec-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dacec-127">Request body</span></span>
<span data-ttu-id="dacec-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="dacec-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="dacec-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="dacec-131">Property</span></span>     | <span data-ttu-id="dacec-132">Тип</span><span class="sxs-lookup"><span data-stu-id="dacec-132">Type</span></span>   |<span data-ttu-id="dacec-133">Описание</span><span class="sxs-lookup"><span data-stu-id="dacec-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dacec-134">values</span><span class="sxs-lookup"><span data-stu-id="dacec-134">values</span></span>|<span data-ttu-id="dacec-135">Json</span><span class="sxs-lookup"><span data-stu-id="dacec-135">Json</span></span>|<span data-ttu-id="dacec-p105">Представляет необработанные значения указанного диапазона. Могут возвращаться строковые и числовые данные, а также логические значения. Ячейка, которая содержит ошибку, вернет строку ошибки.</span><span class="sxs-lookup"><span data-stu-id="dacec-p105">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="dacec-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="dacec-139">Response</span></span>

<span data-ttu-id="dacec-140">В случае успеха этот метод возвращает код ответа и обновленный объект `200 OK` [WorkbookTableColumn](../resources/workbooktablecolumn.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="dacec-140">If successful, this method returns a `200 OK` response code and updated [WorkbookTableColumn](../resources/workbooktablecolumn.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dacec-141">Пример</span><span class="sxs-lookup"><span data-stu-id="dacec-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dacec-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="dacec-142">Request</span></span>
<span data-ttu-id="dacec-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dacec-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dacec-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="dacec-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="dacec-145">C#</span><span class="sxs-lookup"><span data-stu-id="dacec-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tablecolumn-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dacec-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dacec-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tablecolumn-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dacec-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dacec-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tablecolumn-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dacec-148">Java</span><span class="sxs-lookup"><span data-stu-id="dacec-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tablecolumn-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---
> [!NOTE]
> <span data-ttu-id="dacec-149">Если необходимо обновить несколько полей столбца, сделайте **значения** строки массива в запросе.</span><span class="sxs-lookup"><span data-stu-id="dacec-149">If you want to update multiple fields of a column, make **values** a string array in the request.</span></span> <span data-ttu-id="dacec-150">Пример: `"values": [["a"], [1], [2], [3]]`.</span><span class="sxs-lookup"><span data-stu-id="dacec-150">For example: `"values": [["a"], [1], [2], [3]]`.</span></span>

##### <a name="response"></a><span data-ttu-id="dacec-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="dacec-151">Response</span></span>
<span data-ttu-id="dacec-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dacec-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

