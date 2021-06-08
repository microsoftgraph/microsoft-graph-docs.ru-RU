---
title: Обновление объекта profilephoto
description: Обновление фотографии вошедшего **пользователя** либо указанной **группы** или **контакта**. Так как
localization_priority: Priority
author: kevinbellinger
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: b4b3ef3e40f540c0ad3a8cfb75631e7069976b7f
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786319"
---
# <a name="update-profilephoto"></a><span data-ttu-id="e29cb-104">Обновление объекта profilephoto</span><span class="sxs-lookup"><span data-stu-id="e29cb-104">Update profilephoto</span></span>

<span data-ttu-id="e29cb-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e29cb-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e29cb-p102">Обновление фотографии вошедшего **пользователя** либо указанной **группы** или **контакта**. Так как в настоящее время максимальный общий размер каждого запроса REST составляет 4 МБ, размер добавляемой фотографии не может превышать 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="e29cb-p102">Update the photo for the signed-in **user**, or the specified **group** or **contact**. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the photo you can add to under 4MB.</span></span>

<span data-ttu-id="e29cb-108">В версии 1.0 для этой операции можно использовать запросы PATCH и PUT.</span><span class="sxs-lookup"><span data-stu-id="e29cb-108">You can use either PATCH or PUT for this operation in version 1.0.</span></span>

> <span data-ttu-id="e29cb-109">**Примечание.** Эта операция в версии 1.0 поддерживает только рабочие или учебные почтовые ящики пользователя (не личные).</span><span class="sxs-lookup"><span data-stu-id="e29cb-109">**Note** This operation in version 1.0 supports only a user's work or school mailboxes and not personal mailboxes.</span></span>

## <a name="permissions"></a><span data-ttu-id="e29cb-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e29cb-110">Permissions</span></span>
<span data-ttu-id="e29cb-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e29cb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

- <span data-ttu-id="e29cb-113">Фотография профиля вошедшего **пользователя**: User.ReadWrite, User.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="e29cb-113">Profile photo of the signed-in **user** - User.ReadWrite, User.ReadWrite.All</span></span>
- <span data-ttu-id="e29cb-114">Фотография профиля **группы**: Group.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="e29cb-114">Profile photo of a **group** - Group.ReadWrite.All</span></span>
- <span data-ttu-id="e29cb-115">Фотография **контакта**: Contacts.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="e29cb-115">Photo of a **contact** - Contacts.ReadWrite</span></span>

> <span data-ttu-id="e29cb-p104">**Примечание.** Чтобы обновить фотографию какого-либо пользователя в организации, ваше приложение должно получить разрешение User.ReadWrite.All приложения и вызвать API с применением собственного идентификатора, не от имени пользователя. Дополнительные сведения см. в статье [Получение доступа без пользователя](/graph/auth-v2-service).</span><span class="sxs-lookup"><span data-stu-id="e29cb-p104">**Note** To update the photo of any user in the organization, your app must have the User.ReadWrite.All application permission and call this API under its own identity, not on behalf of a user. To learn more, see [get access without a signed-in user](/graph/auth-v2-service).</span></span>

> <span data-ttu-id="e29cb-118">**Примечание.** В настоящее время существует [известная проблема](/graph/known-issues#groups) с доступом к фотографиям группы при помощи разрешений для приложений.</span><span class="sxs-lookup"><span data-stu-id="e29cb-118">**Note:**  There is currently a [known issue](/graph/known-issues#groups) with accessing group photos using application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="e29cb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e29cb-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/photo/$value
PATCH /users/{id | userPrincipalName}/photo/$value
PATCH /groups/{id}/photo/$value
PATCH /me/contacts/{id}/photo/$value
PATCH /users/{id | userPrincipalName}/contacts/{id}/photo/$value
PATCH /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
PATCH /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value

PUT /me/photo/$value
PUT /users/{id | userPrincipalName}/photo/$value
PUT /groups/{id}/photo/$value
PUT /me/contacts/{id}/photo/$value
PUT /users/{id | userPrincipalName}/contacts/{id}/photo/$value
PUT /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
PUT /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
```
## <a name="request-headers"></a><span data-ttu-id="e29cb-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e29cb-120">Request headers</span></span>
| <span data-ttu-id="e29cb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e29cb-121">Header</span></span>       | <span data-ttu-id="e29cb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e29cb-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e29cb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e29cb-123">Authorization</span></span>  | <span data-ttu-id="e29cb-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e29cb-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e29cb-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e29cb-126">Content-Type</span></span>  | <span data-ttu-id="e29cb-p106">image/jpeg. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e29cb-p106">image/jpeg. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e29cb-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e29cb-129">Request body</span></span>
<span data-ttu-id="e29cb-130">Включите в текст запроса двоичные данные фотографии.</span><span class="sxs-lookup"><span data-stu-id="e29cb-130">In the request body, include the binary data of the photo in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="e29cb-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="e29cb-131">Response</span></span>

<span data-ttu-id="e29cb-132">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="e29cb-132">If successful, this method returns a `200 OK` response code.</span></span>
## <a name="example"></a><span data-ttu-id="e29cb-133">Пример</span><span class="sxs-lookup"><span data-stu-id="e29cb-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e29cb-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e29cb-134">Request</span></span>
<span data-ttu-id="e29cb-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e29cb-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e29cb-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="e29cb-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_profilephoto"
}-->
```http
PUT https://graph.microsoft.com/v1.0/me/photo/$value
Content-type: image/jpeg

Binary data for the image

```
# <a name="c"></a>[<span data-ttu-id="e29cb-137">C#</span><span class="sxs-lookup"><span data-stu-id="e29cb-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-profilephoto-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e29cb-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e29cb-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-profilephoto-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e29cb-139">Java</span><span class="sxs-lookup"><span data-stu-id="e29cb-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-profilephoto-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e29cb-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="e29cb-140">Response</span></span>
<span data-ttu-id="e29cb-p107">Ниже представлен пример отклика. Примечание: показанный здесь объект отклика может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e29cb-p107">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update profilephoto",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

