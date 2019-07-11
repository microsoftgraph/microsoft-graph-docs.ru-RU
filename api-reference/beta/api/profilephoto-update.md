---
title: Обновление объекта profilephoto
description: Обновление фотографии для любого пользователя в клиенте, в том числе пользователя, выполнившего вход, или указанной группы или контакта. Так как
localization_priority: Normal
ms.openlocfilehash: 8a3c6d2ce042fa068fb0e0d99798fd8fa2be1d07
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/11/2019
ms.locfileid: "35621343"
---
# <a name="update-profilephoto"></a><span data-ttu-id="e8fe8-104">Обновление объекта profilephoto</span><span class="sxs-lookup"><span data-stu-id="e8fe8-104">Update profilephoto</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8fe8-105">Обновление фотографии для любого пользователя в клиенте, в том числе пользователя, выполнившего вход, или указанной группы или контакта.</span><span class="sxs-lookup"><span data-stu-id="e8fe8-105">Update the photo for any user in the tenant including the signed-in user, or the specified group or contact.</span></span> <span data-ttu-id="e8fe8-106">Так как в настоящее время максимальный общий размер каждого запроса REST составляет 4 МБ, размер добавляемой фотографии не может превышать 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="e8fe8-106">Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the photo you can add to under 4MB.</span></span>

<span data-ttu-id="e8fe8-107">Используйте только PUT для этой операции в бета-версии.</span><span class="sxs-lookup"><span data-stu-id="e8fe8-107">Use only PUT for this operation in the beta version.</span></span>

> <span data-ttu-id="e8fe8-108">**Note (Примечание** ) Операция обновления фотографий в бета-версии поддерживает только рабочие и учебные почтовые ящики пользователей, а не личные почтовые ящики.</span><span class="sxs-lookup"><span data-stu-id="e8fe8-108">**Note** The update photo operation in beta supports only the user's work or school mailboxes and not personal mailboxes.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8fe8-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e8fe8-109">Permissions</span></span>
<span data-ttu-id="e8fe8-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8fe8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8fe8-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e8fe8-112">Permission type</span></span>      | <span data-ttu-id="e8fe8-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e8fe8-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8fe8-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e8fe8-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="e8fe8-115">Фотография профиля вошедшего **пользователя**:</span><span class="sxs-lookup"><span data-stu-id="e8fe8-115">Profile photo of the signed-in **user**:</span></span><br/><span data-ttu-id="e8fe8-116">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e8fe8-116">User.ReadWrite, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="e8fe8-117">Для ресурса **group**:</span><span class="sxs-lookup"><span data-stu-id="e8fe8-117">For **group** resource:</span></span><br /><span data-ttu-id="e8fe8-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8fe8-118">Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="e8fe8-119">Для ресурса **contact**:</span><span class="sxs-lookup"><span data-stu-id="e8fe8-119">For **contact** resource:</span></span><br /><span data-ttu-id="e8fe8-120">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e8fe8-120">Contacts.ReadWrite</span></span> |
|<span data-ttu-id="e8fe8-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e8fe8-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8fe8-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8fe8-122">Not supported.</span></span> |
|<span data-ttu-id="e8fe8-123">Для приложения</span><span class="sxs-lookup"><span data-stu-id="e8fe8-123">Application</span></span>                            | <span data-ttu-id="e8fe8-124">Для ресурса **user**:</span><span class="sxs-lookup"><span data-stu-id="e8fe8-124">For **user** resource:</span></span><br/><span data-ttu-id="e8fe8-125">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8fe8-125">User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="e8fe8-126">Для ресурса **group**:</span><span class="sxs-lookup"><span data-stu-id="e8fe8-126">For **group** resource:</span></span><br /><span data-ttu-id="e8fe8-127">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8fe8-127">Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="e8fe8-128">Для ресурса **contact**:</span><span class="sxs-lookup"><span data-stu-id="e8fe8-128">For **contact** resource:</span></span><br /><span data-ttu-id="e8fe8-129">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e8fe8-129">Contacts.ReadWrite</span></span> |

> <span data-ttu-id="e8fe8-130">**Примечание.** Чтобы обновить фотографию какого-либо пользователя в организации, ваше приложение должно получить разрешение User.ReadWrite.All приложения и вызвать API с применением собственного идентификатора, не от имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="e8fe8-130">**Note** To update the photo of any user in the organization, your app must have the User.ReadWrite.All application permission and call this API under its own identity, not on behalf of a user.</span></span> <span data-ttu-id="e8fe8-131">Дополнительные сведения см. в статье [Получение доступа без пользователя](/graph/auth-v2-service).</span><span class="sxs-lookup"><span data-stu-id="e8fe8-131">To learn more, see [get access without a signed-in user](/graph/auth-v2-service).</span></span>

> <span data-ttu-id="e8fe8-132">**Примечание:**  В настоящее время существует [известная ошибка](https://docs.microsoft.com/en-us/graph/known-issues#groups) при доступе к фотографиям группы с помощью разрешений приложения.</span><span class="sxs-lookup"><span data-stu-id="e8fe8-132">**Note:**  There is currently a [known issue](https://docs.microsoft.com/en-us/graph/known-issues#groups) with accessing group photos using application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="e8fe8-133">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e8fe8-133">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="e8fe8-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e8fe8-134">Request headers</span></span>
| <span data-ttu-id="e8fe8-135">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e8fe8-135">Header</span></span>       | <span data-ttu-id="e8fe8-136">Значение</span><span class="sxs-lookup"><span data-stu-id="e8fe8-136">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e8fe8-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e8fe8-137">Authorization</span></span>  | <span data-ttu-id="e8fe8-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e8fe8-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e8fe8-140">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e8fe8-140">Content-Type</span></span>  | <span data-ttu-id="e8fe8-p106">image/jpeg. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e8fe8-p106">image/jpeg. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e8fe8-143">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e8fe8-143">Request body</span></span>
<span data-ttu-id="e8fe8-144">Включите в текст запроса двоичные данные фотографии.</span><span class="sxs-lookup"><span data-stu-id="e8fe8-144">In the request body, include the binary data of the photo in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="e8fe8-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8fe8-145">Response</span></span>

<span data-ttu-id="e8fe8-146">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="e8fe8-146">If successful, this method returns a `200 OK` response code.</span></span>
## <a name="example"></a><span data-ttu-id="e8fe8-147">Пример</span><span class="sxs-lookup"><span data-stu-id="e8fe8-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e8fe8-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8fe8-148">Request</span></span>
<span data-ttu-id="e8fe8-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e8fe8-149">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e8fe8-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="e8fe8-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_profilephoto"
}-->
```http
PUT https://graph.microsoft.com/beta/me/photo/$value
Content-type: image/jpeg

Binary data for the image

```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e8fe8-151">C#</span><span class="sxs-lookup"><span data-stu-id="e8fe8-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-profilephoto-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e8fe8-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="e8fe8-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-profilephoto-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e8fe8-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="e8fe8-153">Response</span></span>
<span data-ttu-id="e8fe8-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e8fe8-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
