---
title: Обновление объекта profilephoto
description: Обновление фотографии для любого пользователя в клиенте, в том числе пользователя, выполнившего вход, или указанной группы или контакта. Так как
localization_priority: Normal
ms.openlocfilehash: b4f1cc2cf446d540d4143263bdb68bf9c09cccf4
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35455366"
---
# <a name="update-profilephoto"></a><span data-ttu-id="064b1-104">Обновление объекта profilephoto</span><span class="sxs-lookup"><span data-stu-id="064b1-104">Update profilephoto</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="064b1-105">Обновление фотографии для любого пользователя в клиенте, в том числе пользователя, выполнившего вход, или указанной группы или контакта.</span><span class="sxs-lookup"><span data-stu-id="064b1-105">Update the photo for any user in the tenant including the signed-in user, or the specified group or contact.</span></span> <span data-ttu-id="064b1-106">Так как в настоящее время максимальный общий размер каждого запроса REST составляет 4 МБ, размер добавляемой фотографии не может превышать 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="064b1-106">Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the photo you can add to under 4MB.</span></span>

<span data-ttu-id="064b1-107">Используйте только PUT для этой операции в бета-версии.</span><span class="sxs-lookup"><span data-stu-id="064b1-107">Use only PUT for this operation in the beta version.</span></span>

> <span data-ttu-id="064b1-108">**Note (Примечание** ) Операция обновления фотографий в бета-версии поддерживает только рабочие и учебные почтовые ящики пользователей, а не личные почтовые ящики.</span><span class="sxs-lookup"><span data-stu-id="064b1-108">**Note** The update photo operation in beta supports only the user's work or school mailboxes and not personal mailboxes.</span></span>

## <a name="permissions"></a><span data-ttu-id="064b1-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="064b1-109">Permissions</span></span>
<span data-ttu-id="064b1-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="064b1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="064b1-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="064b1-112">Permission type</span></span>      | <span data-ttu-id="064b1-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="064b1-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="064b1-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="064b1-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="064b1-115">Фотография профиля вошедшего **пользователя**:</span><span class="sxs-lookup"><span data-stu-id="064b1-115">Profile photo of the signed-in **user**:</span></span><br/><span data-ttu-id="064b1-116">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="064b1-116">User.ReadWrite, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="064b1-117">Для ресурса **group**:</span><span class="sxs-lookup"><span data-stu-id="064b1-117">For **group** resource:</span></span><br /><span data-ttu-id="064b1-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="064b1-118">Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="064b1-119">Для ресурса **contact**:</span><span class="sxs-lookup"><span data-stu-id="064b1-119">For **contact** resource:</span></span><br /><span data-ttu-id="064b1-120">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="064b1-120">Contacts.ReadWrite</span></span> |
|<span data-ttu-id="064b1-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="064b1-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="064b1-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="064b1-122">Not supported.</span></span> |
|<span data-ttu-id="064b1-123">Для приложения</span><span class="sxs-lookup"><span data-stu-id="064b1-123">Application</span></span>                            | <span data-ttu-id="064b1-124">Для ресурса **user**:</span><span class="sxs-lookup"><span data-stu-id="064b1-124">For **user** resource:</span></span><br/><span data-ttu-id="064b1-125">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="064b1-125">User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="064b1-126">Для ресурса **group**:</span><span class="sxs-lookup"><span data-stu-id="064b1-126">For **group** resource:</span></span><br /><span data-ttu-id="064b1-127">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="064b1-127">Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="064b1-128">Для ресурса **contact**:</span><span class="sxs-lookup"><span data-stu-id="064b1-128">For **contact** resource:</span></span><br /><span data-ttu-id="064b1-129">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="064b1-129">Contacts.ReadWrite</span></span> |

> <span data-ttu-id="064b1-130">**Примечание.** Чтобы обновить фотографию какого-либо пользователя в организации, ваше приложение должно получить разрешение User.ReadWrite.All приложения и вызвать API с применением собственного идентификатора, не от имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="064b1-130">**Note** To update the photo of any user in the organization, your app must have the User.ReadWrite.All application permission and call this API under its own identity, not on behalf of a user.</span></span> <span data-ttu-id="064b1-131">Дополнительные сведения см. в статье [Получение доступа без пользователя](/graph/auth-v2-service).</span><span class="sxs-lookup"><span data-stu-id="064b1-131">To learn more, see [get access without a signed-in user](/graph/auth-v2-service).</span></span>

## <a name="http-request"></a><span data-ttu-id="064b1-132">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="064b1-132">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="064b1-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="064b1-133">Request headers</span></span>
| <span data-ttu-id="064b1-134">Заголовок</span><span class="sxs-lookup"><span data-stu-id="064b1-134">Header</span></span>       | <span data-ttu-id="064b1-135">Значение</span><span class="sxs-lookup"><span data-stu-id="064b1-135">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="064b1-136">Авторизация</span><span class="sxs-lookup"><span data-stu-id="064b1-136">Authorization</span></span>  | <span data-ttu-id="064b1-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="064b1-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="064b1-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="064b1-139">Content-Type</span></span>  | <span data-ttu-id="064b1-p106">image/jpeg. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="064b1-p106">image/jpeg. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="064b1-142">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="064b1-142">Request body</span></span>
<span data-ttu-id="064b1-143">Включите в текст запроса двоичные данные фотографии.</span><span class="sxs-lookup"><span data-stu-id="064b1-143">In the request body, include the binary data of the photo in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="064b1-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="064b1-144">Response</span></span>

<span data-ttu-id="064b1-145">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="064b1-145">If successful, this method returns a `200 OK` response code.</span></span>
## <a name="example"></a><span data-ttu-id="064b1-146">Пример</span><span class="sxs-lookup"><span data-stu-id="064b1-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="064b1-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="064b1-147">Request</span></span>
<span data-ttu-id="064b1-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="064b1-148">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="064b1-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="064b1-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_profilephoto"
}-->
```http
PUT https://graph.microsoft.com/beta/me/photo/$value
Content-type: image/jpeg

Binary data for the image

```
# <a name="ctabcsharp"></a>[<span data-ttu-id="064b1-150">C#</span><span class="sxs-lookup"><span data-stu-id="064b1-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-profilephoto-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="064b1-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="064b1-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-profilephoto-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="064b1-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="064b1-152">Response</span></span>
<span data-ttu-id="064b1-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="064b1-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
