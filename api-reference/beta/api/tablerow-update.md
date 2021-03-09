---
title: Обновление объекта tableRow
description: Обновление свойств объекта tablerow.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: c9851fc18da74a9867b7985c81dde4c7cdbf527d
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50578264"
---
# <a name="update-tablerow"></a><span data-ttu-id="6cbbb-103">Обновление объекта tableRow</span><span class="sxs-lookup"><span data-stu-id="6cbbb-103">Update tablerow</span></span>

<span data-ttu-id="6cbbb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6cbbb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6cbbb-105">Обновление свойств объекта tablerow.</span><span class="sxs-lookup"><span data-stu-id="6cbbb-105">Update the properties of tablerow object.</span></span>
## <a name="permissions"></a><span data-ttu-id="6cbbb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6cbbb-106">Permissions</span></span>
<span data-ttu-id="6cbbb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6cbbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6cbbb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6cbbb-109">Permission type</span></span>      | <span data-ttu-id="6cbbb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6cbbb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6cbbb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6cbbb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6cbbb-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6cbbb-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6cbbb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6cbbb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6cbbb-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6cbbb-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6cbbb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6cbbb-115">Application</span></span> | <span data-ttu-id="6cbbb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6cbbb-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6cbbb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6cbbb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}
PATCH /me/drive/root:/{item-path}:/workbook/tables/{id|name}/rows/{index}
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/rows/{index}
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/rows/{index}
```
## <a name="optional-request-headers"></a><span data-ttu-id="6cbbb-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6cbbb-118">Optional request headers</span></span>
| <span data-ttu-id="6cbbb-119">Имя</span><span class="sxs-lookup"><span data-stu-id="6cbbb-119">Name</span></span>       | <span data-ttu-id="6cbbb-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6cbbb-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="6cbbb-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6cbbb-121">Authorization</span></span>  | <span data-ttu-id="6cbbb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6cbbb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6cbbb-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="6cbbb-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="6cbbb-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="6cbbb-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6cbbb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6cbbb-127">Request body</span></span>
<span data-ttu-id="6cbbb-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="6cbbb-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6cbbb-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="6cbbb-131">Property</span></span>     | <span data-ttu-id="6cbbb-132">Тип</span><span class="sxs-lookup"><span data-stu-id="6cbbb-132">Type</span></span>   |<span data-ttu-id="6cbbb-133">Описание</span><span class="sxs-lookup"><span data-stu-id="6cbbb-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6cbbb-134">values</span><span class="sxs-lookup"><span data-stu-id="6cbbb-134">values</span></span>|<span data-ttu-id="6cbbb-135">Json</span><span class="sxs-lookup"><span data-stu-id="6cbbb-135">Json</span></span>|<span data-ttu-id="6cbbb-p105">Представляет необработанные значения указанного диапазона. Могут возвращаться строковые и числовые данные, а также логические значения. Ячейка, которая содержит ошибку, вернет строку ошибки.</span><span class="sxs-lookup"><span data-stu-id="6cbbb-p105">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="6cbbb-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="6cbbb-139">Response</span></span>

<span data-ttu-id="6cbbb-140">В случае успешной работы этот метод возвращает код ответа и обновленный объект `200 OK` [workbookTableRow](../resources/workbooktablerow.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="6cbbb-140">If successful, this method returns a `200 OK` response code and updated [workbookTableRow](../resources/workbooktablerow.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6cbbb-141">Пример</span><span class="sxs-lookup"><span data-stu-id="6cbbb-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6cbbb-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="6cbbb-142">Request</span></span>
<span data-ttu-id="6cbbb-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6cbbb-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6cbbb-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="6cbbb-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_tablerow"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```
# <a name="c"></a>[<span data-ttu-id="6cbbb-145">C#</span><span class="sxs-lookup"><span data-stu-id="6cbbb-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tablerow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6cbbb-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6cbbb-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tablerow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6cbbb-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6cbbb-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tablerow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6cbbb-148">Java</span><span class="sxs-lookup"><span data-stu-id="6cbbb-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tablerow-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6cbbb-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="6cbbb-149">Response</span></span>
<span data-ttu-id="6cbbb-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6cbbb-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableRow"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update tablerow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


