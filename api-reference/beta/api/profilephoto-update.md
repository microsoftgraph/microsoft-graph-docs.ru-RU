---
title: Обновление объекта profilephoto
description: Обновление фотографии для любого пользователя в клиенте, в том числе пользователя, выполнившего вход, или указанной группы или контакта. Так как
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: kevinbellinger
ms.openlocfilehash: bace39481de10040a58a84e1aafdfa58f00335b7
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981759"
---
# <a name="update-profilephoto"></a><span data-ttu-id="3a144-104">Обновление объекта profilephoto</span><span class="sxs-lookup"><span data-stu-id="3a144-104">Update profilephoto</span></span>

<span data-ttu-id="3a144-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a144-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a144-p102">Обновление фотографии для любого пользователя в клиенте, в том числе пользователя, выполнившего вход, или указанной группы или контакта. Так как ограничение общего размера каждого запроса REST в 8 МБ, размер фотографии, которую можно добавить, ограничен до 8 МБ.</span><span class="sxs-lookup"><span data-stu-id="3a144-p102">Update the photo for any user in the tenant, including the signed-in user or the specified group or contact. Because there is currently a limit of 8MB on the total size of each REST request, the size of the photo you can add is limited to under 8MB.</span></span>

<span data-ttu-id="3a144-108">Используйте PUT только для этой операции.</span><span class="sxs-lookup"><span data-stu-id="3a144-108">Only use PUT for this operation.</span></span>

> <span data-ttu-id="3a144-109">**Note** : при обновлении фотографии **пользователя** эта операция сначала пытается обновить фотографию в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="3a144-109">**Note** :  When updating the **user** photo, this operation first attempts to update the photo in Microsoft 365.</span></span> <span data-ttu-id="3a144-110">Если это не удается (из-за того, что у пользователя нет почтового ящика), этот API будет пытаться обновить фотографию в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3a144-110">If that fails (due to the user not having a mailbox), this API will attempt to update the photo in Azure Active Directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a144-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3a144-111">Permissions</span></span>
<span data-ttu-id="3a144-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a144-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a144-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a144-114">Permission type</span></span>      | <span data-ttu-id="3a144-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a144-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a144-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a144-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="3a144-117">Фотография профиля вошедшего **пользователя** :</span><span class="sxs-lookup"><span data-stu-id="3a144-117">Profile photo of the signed-in **user** :</span></span><br/><span data-ttu-id="3a144-118">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="3a144-118">User.ReadWrite, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="3a144-119">Для ресурса **group** :</span><span class="sxs-lookup"><span data-stu-id="3a144-119">For **group** resource:</span></span><br /><span data-ttu-id="3a144-120">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a144-120">Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="3a144-121">Для ресурса **contact** :</span><span class="sxs-lookup"><span data-stu-id="3a144-121">For **contact** resource:</span></span><br /><span data-ttu-id="3a144-122">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a144-122">Contacts.ReadWrite</span></span> |
|<span data-ttu-id="3a144-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a144-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a144-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a144-124">Not supported.</span></span> |
|<span data-ttu-id="3a144-125">Для приложения</span><span class="sxs-lookup"><span data-stu-id="3a144-125">Application</span></span>                            | <span data-ttu-id="3a144-126">Для ресурса **user** :</span><span class="sxs-lookup"><span data-stu-id="3a144-126">For **user** resource:</span></span><br/><span data-ttu-id="3a144-127">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a144-127">User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="3a144-128">Для ресурса **group** :</span><span class="sxs-lookup"><span data-stu-id="3a144-128">For **group** resource:</span></span><br /><span data-ttu-id="3a144-129">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a144-129">Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="3a144-130">Для ресурса **contact** :</span><span class="sxs-lookup"><span data-stu-id="3a144-130">For **contact** resource:</span></span><br /><span data-ttu-id="3a144-131">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a144-131">Contacts.ReadWrite</span></span> |

> <span data-ttu-id="3a144-132">**Примечание.** Чтобы обновить фотографию какого-либо пользователя в организации, ваше приложение должно получить разрешение User.ReadWrite.All приложения и вызвать API с применением собственного идентификатора, не от имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="3a144-132">**Note** To update the photo of any user in the organization, your app must have the User.ReadWrite.All application permission and call this API under its own identity, not on behalf of a user.</span></span> <span data-ttu-id="3a144-133">Дополнительные сведения см. в статье [Получение доступа без пользователя](/graph/auth-v2-service).</span><span class="sxs-lookup"><span data-stu-id="3a144-133">To learn more, see [get access without a signed-in user](/graph/auth-v2-service).</span></span> <span data-ttu-id="3a144-134">Для обновления фотографии пользователя, выполнившего вход, требуется разрешение User. ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="3a144-134">Updating the photo of the signed-in user only requires User.ReadWrite permission.</span></span>

> <span data-ttu-id="3a144-135">**Примечание.** В настоящее время существует [известная проблема](/graph/known-issues#groups) с доступом к фотографиям группы при помощи разрешений для приложений.</span><span class="sxs-lookup"><span data-stu-id="3a144-135">**Note:**  There is currently a [known issue](/graph/known-issues#groups) with accessing group photos using application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="3a144-136">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a144-136">HTTP request</span></span>
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

<span data-ttu-id="3a144-137">Чтобы обновить фотографию для команды, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="3a144-137">To update the photo for a team:</span></span>

<!-- { "blockType": "ignored" } -->
```http
PUT /groups/{teamId}/photo/$value`
```

## <a name="request-headers"></a><span data-ttu-id="3a144-138">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3a144-138">Request headers</span></span>
| <span data-ttu-id="3a144-139">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3a144-139">Header</span></span>       | <span data-ttu-id="3a144-140">Значение</span><span class="sxs-lookup"><span data-stu-id="3a144-140">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3a144-141">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3a144-141">Authorization</span></span>  | <span data-ttu-id="3a144-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3a144-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3a144-144">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3a144-144">Content-Type</span></span>  | <span data-ttu-id="3a144-p107">image/jpeg. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3a144-p107">image/jpeg. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3a144-147">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3a144-147">Request body</span></span>
<span data-ttu-id="3a144-148">Включите в текст запроса двоичные данные фотографии.</span><span class="sxs-lookup"><span data-stu-id="3a144-148">In the request body, include the binary data of the photo in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="3a144-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a144-149">Response</span></span>

<span data-ttu-id="3a144-150">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="3a144-150">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3a144-151">Пример</span><span class="sxs-lookup"><span data-stu-id="3a144-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="3a144-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a144-152">Request</span></span>
<span data-ttu-id="3a144-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3a144-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3a144-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="3a144-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_profilephoto"
}-->
```http
PUT https://graph.microsoft.com/beta/me/photo/$value
Content-type: image/jpeg

Binary data for the image

```
# <a name="c"></a>[<span data-ttu-id="3a144-155">C#</span><span class="sxs-lookup"><span data-stu-id="3a144-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-profilephoto-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3a144-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3a144-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-profilephoto-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3a144-157">Java</span><span class="sxs-lookup"><span data-stu-id="3a144-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-profilephoto-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="3a144-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a144-158">Response</span></span>
<span data-ttu-id="3a144-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3a144-159">The following is an example of the response.</span></span> 

><span data-ttu-id="3a144-160">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3a144-160">**Note:** The response object shown here might be shortened for readability.</span></span>
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


