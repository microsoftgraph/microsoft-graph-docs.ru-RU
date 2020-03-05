---
title: Обновление объекта NamedItem
description: Обновление свойств объекта nameditem.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 5d3d6fb8bd9bae83b53ce1a39e6f385aaf4c397c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456791"
---
# <a name="update-nameditem"></a><span data-ttu-id="9111c-103">Обновление объекта NamedItem</span><span class="sxs-lookup"><span data-stu-id="9111c-103">Update nameditem</span></span>

<span data-ttu-id="9111c-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9111c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9111c-105">Обновление свойств объекта nameditem.</span><span class="sxs-lookup"><span data-stu-id="9111c-105">Update the properties of nameditem object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9111c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9111c-106">Permissions</span></span>
<span data-ttu-id="9111c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9111c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9111c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9111c-109">Permission type</span></span>      | <span data-ttu-id="9111c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9111c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9111c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9111c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9111c-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9111c-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9111c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9111c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9111c-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9111c-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9111c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9111c-115">Application</span></span> | <span data-ttu-id="9111c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9111c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9111c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9111c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="9111c-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9111c-118">Optional request headers</span></span>
| <span data-ttu-id="9111c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="9111c-119">Name</span></span>       | <span data-ttu-id="9111c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9111c-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="9111c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9111c-121">Authorization</span></span>  | <span data-ttu-id="9111c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9111c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9111c-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9111c-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="9111c-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="9111c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9111c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9111c-127">Request body</span></span>
<span data-ttu-id="9111c-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="9111c-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9111c-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="9111c-131">Property</span></span>     | <span data-ttu-id="9111c-132">Тип</span><span class="sxs-lookup"><span data-stu-id="9111c-132">Type</span></span>   |<span data-ttu-id="9111c-133">Описание</span><span class="sxs-lookup"><span data-stu-id="9111c-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9111c-134">visible</span><span class="sxs-lookup"><span data-stu-id="9111c-134">visible</span></span>|<span data-ttu-id="9111c-135">boolean</span><span class="sxs-lookup"><span data-stu-id="9111c-135">boolean</span></span>|<span data-ttu-id="9111c-136">Определяет, является ли объект видимым.</span><span class="sxs-lookup"><span data-stu-id="9111c-136">Specifies whether the object is visible or not.</span></span>|
|<span data-ttu-id="9111c-137">comment</span><span class="sxs-lookup"><span data-stu-id="9111c-137">comment</span></span>|   <span data-ttu-id="9111c-138">string</span><span class="sxs-lookup"><span data-stu-id="9111c-138">string</span></span>  |<span data-ttu-id="9111c-139">Представляет примечание, связанное с этим именем.</span><span class="sxs-lookup"><span data-stu-id="9111c-139">Represents the comment associated with this name.</span></span>|

## <a name="response"></a><span data-ttu-id="9111c-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="9111c-140">Response</span></span>

<span data-ttu-id="9111c-141">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [воркбукнамедитем](../resources/workbooknameditem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9111c-141">If successful, this method returns a `200 OK` response code and updated [workbookNamedItem](../resources/workbooknameditem.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9111c-142">Пример</span><span class="sxs-lookup"><span data-stu-id="9111c-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9111c-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="9111c-143">Request</span></span>
<span data-ttu-id="9111c-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9111c-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9111c-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="9111c-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_nameditem"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}
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
# <a name="c"></a>[<span data-ttu-id="9111c-146">C#</span><span class="sxs-lookup"><span data-stu-id="9111c-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-nameditem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9111c-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9111c-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-nameditem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9111c-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9111c-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-nameditem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9111c-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="9111c-149">Response</span></span>
<span data-ttu-id="9111c-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9111c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update nameditem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
