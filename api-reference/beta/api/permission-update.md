---
author: JeremyKelley
description: В этой статье рассказывается, как обновить свойства разрешения на общий доступ путем обновления ресурса разрешения.
ms.date: 09/10/2017
title: Изменение разрешений общего доступа
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 56f9d600a36fb7b94757e6c783e2d397306e2de0
ms.sourcegitcommit: de175a11806f9e9ba3c916384e897aee1cc7f75c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/09/2021
ms.locfileid: "49790687"
---
# <a name="update-sharing-permission"></a><span data-ttu-id="e73c4-103">Обновление разрешения на общий доступ</span><span class="sxs-lookup"><span data-stu-id="e73c4-103">Update sharing permission</span></span>

<span data-ttu-id="e73c4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e73c4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e73c4-105">В этой статье рассказывается, как обновить свойства разрешения на общий доступ путем обновления ресурса разрешения.</span><span class="sxs-lookup"><span data-stu-id="e73c4-105">Update the properties of a sharing permission by patching the permission resource.</span></span>

<span data-ttu-id="e73c4-106">Таким способом можно изменить только свойство **roles**.</span><span class="sxs-lookup"><span data-stu-id="e73c4-106">Only the **roles** property can be modified this way.</span></span>

## <a name="permissions"></a><span data-ttu-id="e73c4-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e73c4-107">Permissions</span></span>

<span data-ttu-id="e73c4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e73c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e73c4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e73c4-110">Permission type</span></span>      | <span data-ttu-id="e73c4-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e73c4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e73c4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e73c4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e73c4-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e73c4-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="e73c4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e73c4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e73c4-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e73c4-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="e73c4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e73c4-116">Application</span></span> | <span data-ttu-id="e73c4-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e73c4-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e73c4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e73c4-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
PATCH /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
PATCH /me/drive/items/{item-id}/permissions/{perm-id}
PATCH /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
PATCH /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="e73c4-119">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e73c4-119">Optional request headers</span></span>

| <span data-ttu-id="e73c4-120">Имя</span><span class="sxs-lookup"><span data-stu-id="e73c4-120">Name</span></span>          | <span data-ttu-id="e73c4-121">Тип</span><span class="sxs-lookup"><span data-stu-id="e73c4-121">Type</span></span>   | <span data-ttu-id="e73c4-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e73c4-122">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="e73c4-123">if-match</span><span class="sxs-lookup"><span data-stu-id="e73c4-123">if-match</span></span>      | <span data-ttu-id="e73c4-124">string</span><span class="sxs-lookup"><span data-stu-id="e73c4-124">string</span></span> | <span data-ttu-id="e73c4-125">Если указан заголовок запроса, а предоставленный тег eTag (или cTag) не совпадает с текущим тегом элемента, то возвращается отклик `412 Precondition Failed`, а элемент не удаляется.</span><span class="sxs-lookup"><span data-stu-id="e73c4-125">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e73c4-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e73c4-126">Request body</span></span>

<span data-ttu-id="e73c4-127">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="e73c4-127">In the request body, supply the values for relevant fields that should be updated.</span></span>

<span data-ttu-id="e73c4-128">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="e73c4-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span>
<span data-ttu-id="e73c4-129">Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="e73c4-129">For best performance you shouldn't include existing values that haven't changed.</span></span>

<span data-ttu-id="e73c4-130">Следующие свойства этих типов разрешений можно изменить.</span><span class="sxs-lookup"><span data-stu-id="e73c4-130">The following properties on these permission types can be modified.</span></span>

| <span data-ttu-id="e73c4-131">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e73c4-131">Permission Type</span></span>        | <span data-ttu-id="e73c4-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="e73c4-132">Property</span></span> | <span data-ttu-id="e73c4-133">Тип</span><span class="sxs-lookup"><span data-stu-id="e73c4-133">Type</span></span>              | <span data-ttu-id="e73c4-134">Описание</span><span class="sxs-lookup"><span data-stu-id="e73c4-134">Description</span></span>                   |
|:-----------------------|:---------|:------------------|:------------------------------|
| <span data-ttu-id="e73c4-135">User</span><span class="sxs-lookup"><span data-stu-id="e73c4-135">User</span></span>                   | <span data-ttu-id="e73c4-136">roles</span><span class="sxs-lookup"><span data-stu-id="e73c4-136">roles</span></span>    | <span data-ttu-id="e73c4-137">Набор строк</span><span class="sxs-lookup"><span data-stu-id="e73c4-137">String collection</span></span> | <span data-ttu-id="e73c4-138">Массив типов разрешений.</span><span class="sxs-lookup"><span data-stu-id="e73c4-138">An array of permission types.</span></span> |
| <span data-ttu-id="e73c4-139">Ссылка для анонимного общего доступа</span><span class="sxs-lookup"><span data-stu-id="e73c4-139">Anonymous Sharing Link</span></span> | <span data-ttu-id="e73c4-140">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="e73c4-140">expirationDateTime</span></span> | <span data-ttu-id="e73c4-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e73c4-141">DateTimeOffset</span></span> | <span data-ttu-id="e73c4-142">Формат y-MM-ddTHH:mm:ssZ dateTimeOffset в течение срока действия разрешения.</span><span class="sxs-lookup"><span data-stu-id="e73c4-142">A format of yyyy-MM-ddTHH:mm:ssZ of DateTimeOffset for the expiration time of the permission.</span></span> |

### <a name="remarks"></a><span data-ttu-id="e73c4-143">Примечания</span><span class="sxs-lookup"><span data-stu-id="e73c4-143">Remarks</span></span>
<span data-ttu-id="e73c4-144">Неподтверченные изменения разрешений включают следующие:</span><span class="sxs-lookup"><span data-stu-id="e73c4-144">Unsupported permission modifications include the following:</span></span>
- <span data-ttu-id="e73c4-145">Организационные ссылки для общего доступа</span><span class="sxs-lookup"><span data-stu-id="e73c4-145">Organizational sharing links</span></span>
- <span data-ttu-id="e73c4-146">Ссылки для общего доступа людей</span><span class="sxs-lookup"><span data-stu-id="e73c4-146">People sharing links</span></span>

## <a name="response"></a><span data-ttu-id="e73c4-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="e73c4-147">Response</span></span>

<span data-ttu-id="e73c4-148">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [permission](../resources/permission.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e73c4-148">If successful, this method returns a `200 OK` response code and updated [permission](../resources/permission.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e73c4-149">Пример</span><span class="sxs-lookup"><span data-stu-id="e73c4-149">Example</span></span>

<span data-ttu-id="e73c4-150">Вот пример запроса, изменяющего роль в разрешении на общий доступ на роль "только чтение".</span><span class="sxs-lookup"><span data-stu-id="e73c4-150">Here is an example of the request that changes the role on the sharing permission to read-only.</span></span>


# <a name="http"></a>[<span data-ttu-id="e73c4-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="e73c4-151">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "update-permission", "@odata.type": "microsoft.graph.permission", "scopes": "files.readwrite"} -->

```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{item-id}/permissions/{perm-id}
Content-type: application/json

{
  "roles": [ "read" ]
}
```
# <a name="c"></a>[<span data-ttu-id="e73c4-152">C#</span><span class="sxs-lookup"><span data-stu-id="e73c4-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-permission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e73c4-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e73c4-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-permission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e73c4-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e73c4-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-permission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e73c4-155">Java</span><span class="sxs-lookup"><span data-stu-id="e73c4-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-permission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e73c4-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="e73c4-156">Response</span></span>

<span data-ttu-id="e73c4-157">При успешном выполнении этот метод возвращает ресурс [Permission](../resources/permission.md), представляющий обновленное состояние разрешения, в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e73c4-157">If successful, this method returns a [Permission](../resources/permission.md) resource in the response body that represents the updated state of the permission.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "grantedTo": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "efee1b77-fb3b-4f65-99d6-274c11914d12"
    }
  },
  "id": "1",
  "roles": [ "read" ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update an item's sharing permissions",
  "keywords": "permission, permissions, sharing, change permissions, update permission",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Update permission",
  "suppressions": [
  ]
}
-->


