---
title: Обновление объекта profilephoto
description: Обновление фотографии вошедшего **пользователя** либо указанной **группы** или **контакта**. Так как
localization_priority: Priority
author: kevinbellinger
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: efd5568dcb03f3cbfab4105a58c0024f35f5f4a9
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48972593"
---
# <a name="update-profilephoto"></a><span data-ttu-id="e29bb-104">Обновление объекта profilephoto</span><span class="sxs-lookup"><span data-stu-id="e29bb-104">Update profilephoto</span></span>

<span data-ttu-id="e29bb-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e29bb-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e29bb-p102">Обновление фотографии вошедшего **пользователя** либо указанной **группы** или **контакта**. Так как в настоящее время максимальный общий размер каждого запроса REST составляет 4 МБ, размер добавляемой фотографии не может превышать 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="e29bb-p102">Update the photo for the signed-in **user**, or the specified **group** or **contact**. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the photo you can add to under 4MB.</span></span>

<span data-ttu-id="e29bb-108">В версии 1.0 для этой операции можно использовать запросы PATCH и PUT.</span><span class="sxs-lookup"><span data-stu-id="e29bb-108">You can use either PATCH or PUT for this operation in version 1.0.</span></span>

> <span data-ttu-id="e29bb-109">**Примечание.** Эта операция в версии 1.0 поддерживает только рабочие или учебные почтовые ящики пользователя (не личные).</span><span class="sxs-lookup"><span data-stu-id="e29bb-109">**Note** This operation in version 1.0 supports only a user's work or school mailboxes and not personal mailboxes.</span></span>

## <a name="permissions"></a><span data-ttu-id="e29bb-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e29bb-110">Permissions</span></span>
<span data-ttu-id="e29bb-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e29bb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

- <span data-ttu-id="e29bb-113">Фотография профиля вошедшего **пользователя**: User.ReadWrite, User.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="e29bb-113">Profile photo of the signed-in **user** - User.ReadWrite, User.ReadWrite.All</span></span>
- <span data-ttu-id="e29bb-114">Фотография профиля **группы**: Group.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="e29bb-114">Profile photo of a **group** - Group.ReadWrite.All</span></span>
- <span data-ttu-id="e29bb-115">Фотография **контакта**: Contacts.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="e29bb-115">Photo of a **contact** - Contacts.ReadWrite</span></span>

> <span data-ttu-id="e29bb-116">**Примечание.** Чтобы обновить фотографию какого-либо пользователя в организации, ваше приложение должно получить разрешение User.ReadWrite.All приложения и вызвать API с применением собственного идентификатора, не от имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="e29bb-116">**Note** To update the photo of any user in the organization, your app must have the User.ReadWrite.All application permission and call this API under its own identity, not on behalf of a user.</span></span> <span data-ttu-id="e29bb-117">Дополнительные сведения см. в статье [Получение доступа без пользователя](/graph/auth-v2-service).</span><span class="sxs-lookup"><span data-stu-id="e29bb-117">To learn more, see [get access without a signed-in user](/graph/auth-v2-service).</span></span>

> <span data-ttu-id="e29bb-118">**Примечание.** В настоящее время существует [известная проблема](/graph/known-issues#groups) с доступом к фотографиям группы при помощи разрешений для приложений.</span><span class="sxs-lookup"><span data-stu-id="e29bb-118">**Note:**  There is currently a [known issue](/graph/known-issues#groups) with accessing group photos using application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="e29bb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e29bb-119">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="e29bb-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e29bb-120">Request headers</span></span>
| <span data-ttu-id="e29bb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e29bb-121">Header</span></span>       | <span data-ttu-id="e29bb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e29bb-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e29bb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e29bb-123">Authorization</span></span>  | <span data-ttu-id="e29bb-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e29bb-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e29bb-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e29bb-126">Content-Type</span></span>  | <span data-ttu-id="e29bb-p106">image/jpeg. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e29bb-p106">image/jpeg. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e29bb-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e29bb-129">Request body</span></span>
<span data-ttu-id="e29bb-130">Включите в текст запроса двоичные данные фотографии.</span><span class="sxs-lookup"><span data-stu-id="e29bb-130">In the request body, include the binary data of the photo in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="e29bb-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="e29bb-131">Response</span></span>

<span data-ttu-id="e29bb-132">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="e29bb-132">If successful, this method returns a `200 OK` response code.</span></span>
## <a name="example"></a><span data-ttu-id="e29bb-133">Пример</span><span class="sxs-lookup"><span data-stu-id="e29bb-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e29bb-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e29bb-134">Request</span></span>
<span data-ttu-id="e29bb-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e29bb-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e29bb-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="e29bb-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_profilephoto"
}-->
```http
PUT https://graph.microsoft.com/v1.0/me/photo/$value
Content-type: image/jpeg

Binary data for the image

```
# <a name="c"></a>[<span data-ttu-id="e29bb-137">C#</span><span class="sxs-lookup"><span data-stu-id="e29bb-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-profilephoto-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e29bb-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e29bb-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-profilephoto-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e29bb-139">Java</span><span class="sxs-lookup"><span data-stu-id="e29bb-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-profilephoto-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e29bb-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="e29bb-140">Response</span></span>
<span data-ttu-id="e29bb-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e29bb-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profilePhoto"
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

