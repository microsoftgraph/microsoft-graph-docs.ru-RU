---
author: JeremyKelley
description: В этой статье рассказывается, как обновить свойства разрешения на общий доступ путем обновления ресурса разрешения.
ms.date: 09/10/2017
title: Изменение разрешений на общий доступ
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: ef46b64db30c6d8ceaf65a2f4a7f4c935834b9b0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35983497"
---
# <a name="update-sharing-permission"></a><span data-ttu-id="36363-103">Обновление разрешения на общий доступ</span><span class="sxs-lookup"><span data-stu-id="36363-103">Update sharing permission</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36363-104">В этой статье рассказывается, как обновить свойства разрешения на общий доступ путем обновления ресурса разрешения.</span><span class="sxs-lookup"><span data-stu-id="36363-104">Update the properties of a sharing permission by patching the permission resource.</span></span>

<span data-ttu-id="36363-105">Таким способом можно изменить только свойство **roles**.</span><span class="sxs-lookup"><span data-stu-id="36363-105">Only the **roles** property can be modified this way.</span></span>

## <a name="permissions"></a><span data-ttu-id="36363-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="36363-106">Permissions</span></span>

<span data-ttu-id="36363-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36363-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36363-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="36363-109">Permission type</span></span>      | <span data-ttu-id="36363-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="36363-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36363-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="36363-111">Delegated (work or school account)</span></span> | <span data-ttu-id="36363-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36363-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="36363-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="36363-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36363-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36363-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="36363-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="36363-115">Application</span></span> | <span data-ttu-id="36363-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36363-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="36363-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="36363-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
PATCH /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
PATCH /me/drive/items/{item-id}/permissions/{perm-id}
PATCH /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
PATCH /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="36363-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="36363-118">Optional request headers</span></span>

| <span data-ttu-id="36363-119">Имя</span><span class="sxs-lookup"><span data-stu-id="36363-119">Name</span></span>          | <span data-ttu-id="36363-120">Тип</span><span class="sxs-lookup"><span data-stu-id="36363-120">Type</span></span>   | <span data-ttu-id="36363-121">Описание</span><span class="sxs-lookup"><span data-stu-id="36363-121">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="36363-122">if-match</span><span class="sxs-lookup"><span data-stu-id="36363-122">if-match</span></span>      | <span data-ttu-id="36363-123">string</span><span class="sxs-lookup"><span data-stu-id="36363-123">string</span></span> | <span data-ttu-id="36363-124">Если указан заголовок запроса, а предоставленный тег eTag (или cTag) не совпадает с текущим тегом элемента, то возвращается отклик `412 Precondition Failed`, а элемент не удаляется.</span><span class="sxs-lookup"><span data-stu-id="36363-124">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="request-body"></a><span data-ttu-id="36363-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="36363-125">Request body</span></span>

<span data-ttu-id="36363-126">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="36363-126">In the request body, supply the values for relevant fields that should be updated.</span></span>

<span data-ttu-id="36363-127">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="36363-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span>
<span data-ttu-id="36363-128">Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="36363-128">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="36363-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="36363-129">Property</span></span>     | <span data-ttu-id="36363-130">Тип</span><span class="sxs-lookup"><span data-stu-id="36363-130">Type</span></span>   | <span data-ttu-id="36363-131">Описание</span><span class="sxs-lookup"><span data-stu-id="36363-131">Description</span></span>                   |
|:-------------|:-------|:------------------------------|
| <span data-ttu-id="36363-132">**roles**</span><span class="sxs-lookup"><span data-stu-id="36363-132">**roles**</span></span>    | <span data-ttu-id="36363-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="36363-133">String collection</span></span> | <span data-ttu-id="36363-134">Массив типов разрешений.</span><span class="sxs-lookup"><span data-stu-id="36363-134">An array of permission types.</span></span> |

## <a name="response"></a><span data-ttu-id="36363-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="36363-135">Response</span></span>

<span data-ttu-id="36363-136">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [permission](../resources/permission.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="36363-136">If successful, this method returns a `200 OK` response code and updated [permission](../resources/permission.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36363-137">Пример</span><span class="sxs-lookup"><span data-stu-id="36363-137">Example</span></span>

<span data-ttu-id="36363-138">Вот пример запроса, изменяющего роль в разрешении на общий доступ на роль "только чтение".</span><span class="sxs-lookup"><span data-stu-id="36363-138">Here is an example of the request that changes the role on the sharing permission to read-only.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="36363-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="36363-139">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "update-permission", "@odata.type": "microsoft.graph.permission", "scopes": "files.readwrite"} -->

```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{item-id}/permissions/{perm-id}
Content-type: application/json

{
  "roles": [ "read" ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="36363-140">C#</span><span class="sxs-lookup"><span data-stu-id="36363-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-permission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="36363-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="36363-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-permission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="36363-142">Цель — C</span><span class="sxs-lookup"><span data-stu-id="36363-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-permission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="36363-143">Java</span><span class="sxs-lookup"><span data-stu-id="36363-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-permission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="36363-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="36363-144">Response</span></span>

<span data-ttu-id="36363-145">При успешном выполнении этот метод возвращает ресурс [Permission](../resources/permission.md), представляющий обновленное состояние разрешения, в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="36363-145">If successful, this method returns a [Permission](../resources/permission.md) resource in the response body that represents the updated state of the permission.</span></span>

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
