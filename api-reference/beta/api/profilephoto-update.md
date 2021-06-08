---
title: Обновление объекта profilephoto
description: Обновление фотографии любого пользователя в клиенте, в том числе пользователя, выполнившего вход, либо указанной группы или контакта. Так как
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: kevinbellinger
ms.openlocfilehash: e6ccd0fe70f2e48c890df074c6a7865cbf502f83
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787592"
---
# <a name="update-profilephoto"></a><span data-ttu-id="271b5-104">Обновление объекта profilephoto</span><span class="sxs-lookup"><span data-stu-id="271b5-104">Update profilephoto</span></span>

<span data-ttu-id="271b5-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="271b5-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="271b5-106">Обновим фотографию для любого пользователя в клиенте, включая пользователя, включаемого в нее, или указанной группы или контакта.</span><span class="sxs-lookup"><span data-stu-id="271b5-106">Update the photo for any user in the tenant, including the signed-in user or the specified group or contact.</span></span> <span data-ttu-id="271b5-107">Так как в настоящее время существует ограничение в 8 МБ на общий размер каждого запроса REST, размер фотографии, которая можно добавить, ограничен до 8 МБ.</span><span class="sxs-lookup"><span data-stu-id="271b5-107">Because there is currently a limit of 8MB on the total size of each REST request, the size of the photo you can add is limited to under 8MB.</span></span>

<span data-ttu-id="271b5-108">Только используйте PUT для этой операции.</span><span class="sxs-lookup"><span data-stu-id="271b5-108">Only use PUT for this operation.</span></span>

> <span data-ttu-id="271b5-109">**Примечание.** При обновлении **фотографии** пользователя эта операция сначала пытается обновить фотографию в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="271b5-109">**Note**:  When updating the **user** photo, this operation first attempts to update the photo in Microsoft 365.</span></span> <span data-ttu-id="271b5-110">Если это не удается (из-за того, что у пользователя нет почтового ящика), этот API попытается обновить фотографию в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="271b5-110">If that fails (due to the user not having a mailbox), this API will attempt to update the photo in Azure Active Directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="271b5-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="271b5-111">Permissions</span></span>
<span data-ttu-id="271b5-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="271b5-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="271b5-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="271b5-114">Permission type</span></span>      | <span data-ttu-id="271b5-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="271b5-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="271b5-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="271b5-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="271b5-117">Фотография профиля подписанного **пользователя:**</span><span class="sxs-lookup"><span data-stu-id="271b5-117">Profile photo of the signed-in **user**:</span></span><br/><span data-ttu-id="271b5-118">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="271b5-118">User.ReadWrite, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="271b5-119">Для ресурса **group**:</span><span class="sxs-lookup"><span data-stu-id="271b5-119">For **group** resource:</span></span><br /><span data-ttu-id="271b5-120">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="271b5-120">Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="271b5-121">Для ресурса **contact**:</span><span class="sxs-lookup"><span data-stu-id="271b5-121">For **contact** resource:</span></span><br /><span data-ttu-id="271b5-122">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="271b5-122">Contacts.ReadWrite</span></span> |
|<span data-ttu-id="271b5-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="271b5-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="271b5-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="271b5-124">Not supported.</span></span> |
|<span data-ttu-id="271b5-125">Для приложения</span><span class="sxs-lookup"><span data-stu-id="271b5-125">Application</span></span>                            | <span data-ttu-id="271b5-126">Для ресурса **user**:</span><span class="sxs-lookup"><span data-stu-id="271b5-126">For **user** resource:</span></span><br/><span data-ttu-id="271b5-127">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="271b5-127">User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="271b5-128">Для ресурса **group**:</span><span class="sxs-lookup"><span data-stu-id="271b5-128">For **group** resource:</span></span><br /><span data-ttu-id="271b5-129">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="271b5-129">Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="271b5-130">Для ресурса **contact**:</span><span class="sxs-lookup"><span data-stu-id="271b5-130">For **contact** resource:</span></span><br /><span data-ttu-id="271b5-131">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="271b5-131">Contacts.ReadWrite</span></span> |

> <span data-ttu-id="271b5-132">**Примечание.** Чтобы обновить фотографию какого-либо пользователя в организации, ваше приложение должно получить разрешение User.ReadWrite.All приложения и вызвать API с применением собственного идентификатора, не от имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="271b5-132">**Note** To update the photo of any user in the organization, your app must have the User.ReadWrite.All application permission and call this API under its own identity, not on behalf of a user.</span></span> <span data-ttu-id="271b5-133">Дополнительные сведения см. в статье [Получение доступа без пользователя](/graph/auth-v2-service).</span><span class="sxs-lookup"><span data-stu-id="271b5-133">To learn more, see [get access without a signed-in user](/graph/auth-v2-service).</span></span> <span data-ttu-id="271b5-134">Обновление фотографии подписанного пользователя требует только разрешения User.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="271b5-134">Updating the photo of the signed-in user only requires User.ReadWrite permission.</span></span>

> <span data-ttu-id="271b5-135">**Примечание.** В настоящее время существует [известная проблема](/graph/known-issues#groups) с доступом к фотографиям группы при помощи разрешений для приложений.</span><span class="sxs-lookup"><span data-stu-id="271b5-135">**Note:**  There is currently a [known issue](/graph/known-issues#groups) with accessing group photos using application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="271b5-136">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="271b5-136">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /me/photo/$value
PUT /users/{id | userPrincipalName}/photo/$value
PUT /groups/{id}/photo/$value
PUT /me/contacts/{id}/photo/$value
PUT /users/{id | userPrincipalName}/contacts/{id}/photo/$value
PUT /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
PUT /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
```

<span data-ttu-id="271b5-137">Обновление фотографии для группы:</span><span class="sxs-lookup"><span data-stu-id="271b5-137">To update the photo for a team:</span></span>

<!-- { "blockType": "ignored" } -->
```http
PUT /groups/{teamId}/photo/$value
```

## <a name="request-headers"></a><span data-ttu-id="271b5-138">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="271b5-138">Request headers</span></span>
| <span data-ttu-id="271b5-139">Заголовок</span><span class="sxs-lookup"><span data-stu-id="271b5-139">Header</span></span>       | <span data-ttu-id="271b5-140">Значение</span><span class="sxs-lookup"><span data-stu-id="271b5-140">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="271b5-141">Авторизация</span><span class="sxs-lookup"><span data-stu-id="271b5-141">Authorization</span></span>  | <span data-ttu-id="271b5-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="271b5-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="271b5-144">Content-Type</span><span class="sxs-lookup"><span data-stu-id="271b5-144">Content-Type</span></span>  | <span data-ttu-id="271b5-p107">image/jpeg. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="271b5-p107">image/jpeg. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="271b5-147">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="271b5-147">Request body</span></span>
<span data-ttu-id="271b5-148">Включите в текст запроса двоичные данные фотографии.</span><span class="sxs-lookup"><span data-stu-id="271b5-148">In the request body, include the binary data of the photo in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="271b5-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="271b5-149">Response</span></span>

<span data-ttu-id="271b5-150">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="271b5-150">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="271b5-151">Пример</span><span class="sxs-lookup"><span data-stu-id="271b5-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="271b5-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="271b5-152">Request</span></span>
<span data-ttu-id="271b5-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="271b5-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="271b5-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="271b5-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_profilephoto"
}-->
```http
PUT https://graph.microsoft.com/beta/me/photo/$value
Content-type: image/jpeg

Binary data for the image

```
# <a name="c"></a>[<span data-ttu-id="271b5-155">C#</span><span class="sxs-lookup"><span data-stu-id="271b5-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-profilephoto-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="271b5-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="271b5-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-profilephoto-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="271b5-157">Java</span><span class="sxs-lookup"><span data-stu-id="271b5-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-profilephoto-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="271b5-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="271b5-158">Response</span></span>
<span data-ttu-id="271b5-159">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="271b5-159">The following is an example of the response.</span></span> 

><span data-ttu-id="271b5-160">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="271b5-160">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update profilephoto",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


