---
title: Обновление объекта NamedItem
description: Обновление свойств объекта nameditem.
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: c5b1ee93b0c94d8be9b53476319331519640ae73
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055892"
---
# <a name="update-nameditem"></a><span data-ttu-id="4d822-103">Обновление объекта NamedItem</span><span class="sxs-lookup"><span data-stu-id="4d822-103">Update nameditem</span></span>

<span data-ttu-id="4d822-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d822-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4d822-105">Обновление свойств объекта nameditem.</span><span class="sxs-lookup"><span data-stu-id="4d822-105">Update the properties of nameditem object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4d822-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4d822-106">Permissions</span></span>
<span data-ttu-id="4d822-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d822-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d822-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4d822-109">Permission type</span></span>      | <span data-ttu-id="4d822-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4d822-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d822-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4d822-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4d822-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4d822-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4d822-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4d822-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d822-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d822-114">Not supported.</span></span>    |
|<span data-ttu-id="4d822-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4d822-115">Application</span></span> | <span data-ttu-id="4d822-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d822-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d822-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4d822-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/names/{name}
PATCH /me/drive/root:/{item-path}:/workbook/names/{name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="4d822-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4d822-118">Optional request headers</span></span>
| <span data-ttu-id="4d822-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4d822-119">Name</span></span>       | <span data-ttu-id="4d822-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4d822-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="4d822-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4d822-121">Authorization</span></span>  | <span data-ttu-id="4d822-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4d822-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4d822-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4d822-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="4d822-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="4d822-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d822-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4d822-127">Request body</span></span>
<span data-ttu-id="4d822-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="4d822-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4d822-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="4d822-131">Property</span></span>     | <span data-ttu-id="4d822-132">Тип</span><span class="sxs-lookup"><span data-stu-id="4d822-132">Type</span></span>   |<span data-ttu-id="4d822-133">Описание</span><span class="sxs-lookup"><span data-stu-id="4d822-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4d822-134">visible</span><span class="sxs-lookup"><span data-stu-id="4d822-134">visible</span></span>|<span data-ttu-id="4d822-135">boolean</span><span class="sxs-lookup"><span data-stu-id="4d822-135">boolean</span></span>|<span data-ttu-id="4d822-136">Определяет, является ли объект видимым.</span><span class="sxs-lookup"><span data-stu-id="4d822-136">Specifies whether the object is visible or not.</span></span>|
|<span data-ttu-id="4d822-137">comment</span><span class="sxs-lookup"><span data-stu-id="4d822-137">comment</span></span>|   <span data-ttu-id="4d822-138">string</span><span class="sxs-lookup"><span data-stu-id="4d822-138">string</span></span>  |<span data-ttu-id="4d822-139">Представляет примечание, связанное с этим именем.</span><span class="sxs-lookup"><span data-stu-id="4d822-139">Represents the comment associated with this name.</span></span>|

## <a name="response"></a><span data-ttu-id="4d822-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="4d822-140">Response</span></span>

<span data-ttu-id="4d822-141">В случае успешной работы этот метод возвращает код ответа и обновленный `200 OK` [объект WorkbookNamedItem](../resources/nameditem.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="4d822-141">If successful, this method returns a `200 OK` response code and updated [WorkbookNamedItem](../resources/nameditem.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4d822-142">Пример</span><span class="sxs-lookup"><span data-stu-id="4d822-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4d822-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="4d822-143">Request</span></span>
<span data-ttu-id="4d822-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4d822-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4d822-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="4d822-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_nameditem"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}
Content-type: application/json
Content-length: 87

{
  "type": "type-value",
  "scope": "scope-value",
  "comment": "comment-value",
  "value": {
  },
  "visible": true
}
```
# <a name="c"></a>[<span data-ttu-id="4d822-146">C#</span><span class="sxs-lookup"><span data-stu-id="4d822-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-nameditem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4d822-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4d822-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-nameditem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4d822-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4d822-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-nameditem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4d822-149">Java</span><span class="sxs-lookup"><span data-stu-id="4d822-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-nameditem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4d822-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d822-150">Response</span></span>
<span data-ttu-id="4d822-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4d822-151">Here is an example of the response.</span></span> <span data-ttu-id="4d822-152">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4d822-152">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookNamedItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 87

{
  "name": "name-value",
  "type": "type-value",
  "value": {
  },
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update nameditem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

