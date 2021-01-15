---
title: 'permission: revokeGrants'
description: Обновление разрешений на общий доступ к элементу
author: learafa
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 42a0a3f61349e5ed2741e26a2cb9817f45b4848c
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873460"
---
# <a name="permission-revokegrants"></a><span data-ttu-id="892ec-103">permission: revokeGrants</span><span class="sxs-lookup"><span data-stu-id="892ec-103">permission: revokeGrants</span></span>
<span data-ttu-id="892ec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="892ec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="892ec-105">Удалите доступ к [listItem][] или [driveItem,][] предоставленный по ссылке для общего доступа, удалив указанного получателя [из][] ссылки.</span><span class="sxs-lookup"><span data-stu-id="892ec-105">Revoke access to a [listItem][] or [driveItem][] granted via a sharing link by removing the specified [recipient][] from the link.</span></span>

><span data-ttu-id="892ec-106">**Примечание.** Эта функция доступна только для обмена ссылками, доступными пользователям.</span><span class="sxs-lookup"><span data-stu-id="892ec-106">**Note:** This functionality is only available for sharing links scoped to users.</span></span>

[listItem]: ../resources/listitem.md
[driveItem]: ../resources/driveitem.md
[recipient]: ../resources/driverecipient.md

## <a name="permissions"></a><span data-ttu-id="892ec-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="892ec-110">Permissions</span></span>
<span data-ttu-id="892ec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="892ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="892ec-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="892ec-113">Permission type</span></span>|<span data-ttu-id="892ec-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="892ec-114">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="892ec-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="892ec-115">Delegated (work or school account)</span></span>|<span data-ttu-id="892ec-116">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="892ec-116">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>|
|<span data-ttu-id="892ec-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="892ec-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="892ec-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="892ec-118">Not supported</span></span>|
|<span data-ttu-id="892ec-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="892ec-119">Application</span></span>|<span data-ttu-id="892ec-120">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="892ec-120">Files.ReadWrite.All, Sites.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="892ec-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="892ec-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /drives/{drive-id}/items/{item-id}/permissions/{perm-id}/revokeGrants
POST /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}/revokeGrants
POST /me/drive/items/{item-id}/permissions/{perm-id}/revokeGrants
POST /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}/revokeGrants
POST /sites/{site-id}/lists/{list-id}/items/{listItem-id}/permissions/{perm-id}/revokeGrants
POST /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}/revokeGrants
```

## <a name="request-headers"></a><span data-ttu-id="892ec-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="892ec-122">Request headers</span></span>
|<span data-ttu-id="892ec-123">Имя</span><span class="sxs-lookup"><span data-stu-id="892ec-123">Name</span></span>|<span data-ttu-id="892ec-124">Описание</span><span class="sxs-lookup"><span data-stu-id="892ec-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="892ec-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="892ec-125">Authorization</span></span>|<span data-ttu-id="892ec-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="892ec-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="892ec-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="892ec-128">Content-Type</span></span>|<span data-ttu-id="892ec-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="892ec-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="892ec-131">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="892ec-131">Request body</span></span>
<span data-ttu-id="892ec-132">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="892ec-132">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="892ec-133">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="892ec-133">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="892ec-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="892ec-134">Parameter</span></span>|<span data-ttu-id="892ec-135">Тип</span><span class="sxs-lookup"><span data-stu-id="892ec-135">Type</span></span>|<span data-ttu-id="892ec-136">Описание</span><span class="sxs-lookup"><span data-stu-id="892ec-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="892ec-137">grantees</span><span class="sxs-lookup"><span data-stu-id="892ec-137">grantees</span></span>|<span data-ttu-id="892ec-138">[Коллекция driveRecipient](../resources/driverecipient.md)</span><span class="sxs-lookup"><span data-stu-id="892ec-138">[driveRecipient](../resources/driverecipient.md) collection</span></span>|<span data-ttu-id="892ec-139">Коллекция получателей, которым будет отозван доступ к ссылке для общего доступа.</span><span class="sxs-lookup"><span data-stu-id="892ec-139">A collection of recipients who will be revoked access to the sharing link.</span></span>|

## <a name="response"></a><span data-ttu-id="892ec-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="892ec-140">Response</span></span>

<span data-ttu-id="892ec-141">В случае успеха это действие возвращает код отклика и `200 OK` [разрешение](../resources/permission.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="892ec-141">If successful, this action returns a `200 OK` response code and a [permission](../resources/permission.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="892ec-142">Примеры</span><span class="sxs-lookup"><span data-stu-id="892ec-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="892ec-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="892ec-143">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="892ec-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="892ec-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "permission-revokegrants"
}
-->
``` http
POST /me/drive/items/{item-id}/permissions/{perm-id}/revokeGrants
Content-Type: application/json
Content-length: 95

{
  "grantees": [
    {
      "email": "ryan@contoso.com"
    }
  ]
}
```
# <a name="javascript"></a>[<span data-ttu-id="892ec-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="892ec-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/permission-revokegrants-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="892ec-146">C#</span><span class="sxs-lookup"><span data-stu-id="892ec-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/permission-revokegrants-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="892ec-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="892ec-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/permission-revokegrants-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="892ec-148">Java</span><span class="sxs-lookup"><span data-stu-id="892ec-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/permission-revokegrants-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="892ec-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="892ec-149">Response</span></span>

<span data-ttu-id="892ec-150">В случае успеха этот метод возвращает ресурс [Permission](../resources/permission.md) в теле ответа, который представляет обновленное состояние ссылки для общего доступа.</span><span class="sxs-lookup"><span data-stu-id="892ec-150">If successful, this method returns a [Permission](../resources/permission.md) resource in the response body that represents the updated state of the sharing link.</span></span>

><span data-ttu-id="892ec-151">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="892ec-151">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["write"],
  "link": {
    "type": "edit",
    "scope": "users",
    "webUrl": "https://contoso-my.sharepoint.com/personal/ellen_contoso_com/...",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```


<!-- {
  "type": "#page.annotation",
  "description": "Update an item's sharing permissions",
  "keywords": "permission, permissions, sharing, change permissions, update permission",
  "section": "documentation",
  "tocPath": "Sharing/Update permission"
} -->
