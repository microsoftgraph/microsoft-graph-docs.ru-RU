---
title: Обновление объекта profilephoto
description: Обновление фотографий для любого пользователя, в том числе выполнил вход для клиентов пользователя, или указанной группы или контакта. Начиная с него
ms.openlocfilehash: 801ccd58e57cb02c1805f927dc22c9fd593cbae5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079534"
---
# <a name="update-profilephoto"></a><span data-ttu-id="6d1c6-104">Обновление объекта profilephoto</span><span class="sxs-lookup"><span data-stu-id="6d1c6-104">Update profilephoto</span></span>

> <span data-ttu-id="6d1c6-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6d1c6-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6d1c6-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d1c6-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6d1c6-107">Обновление фотографий для любого пользователя, в том числе выполнил вход для клиентов пользователя, или указанной группы или контакта.</span><span class="sxs-lookup"><span data-stu-id="6d1c6-107">Update the photo for any user in the tenant including the signed-in user, or the specified group or contact.</span></span> <span data-ttu-id="6d1c6-108">Поскольку в настоящее время не более 4 МБ на общий размер каждого запроса REST, этот параметр ограничивает размер фотографию, которую можно добавить в разделе 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="6d1c6-108">Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the photo you can add to under 4MB.</span></span>

<span data-ttu-id="6d1c6-109">Используйте только PUT для этой операции в бета-версии.</span><span class="sxs-lookup"><span data-stu-id="6d1c6-109">Use only PUT for this operation in the beta version.</span></span>

> <span data-ttu-id="6d1c6-110">**Примечание** Операция обновления фотографий в бета-версии поддерживает только пользователя рабочих или почтовые ящики school и не личные почтовые ящики.</span><span class="sxs-lookup"><span data-stu-id="6d1c6-110">**Note** The update photo operation in beta supports only the user's work or school mailboxes and not personal mailboxes.</span></span>

## <a name="permissions"></a><span data-ttu-id="6d1c6-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6d1c6-111">Permissions</span></span>
<span data-ttu-id="6d1c6-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d1c6-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d1c6-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6d1c6-114">Permission type</span></span>      | <span data-ttu-id="6d1c6-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6d1c6-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6d1c6-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6d1c6-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="6d1c6-117">Фотографий профиля выполнившего вход **пользователя**:</span><span class="sxs-lookup"><span data-stu-id="6d1c6-117">Profile photo of the signed-in **user**:</span></span><br/><span data-ttu-id="6d1c6-118">User.ReadWrite User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d1c6-118">User.ReadWrite, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="6d1c6-119">Для ресурса **group**:</span><span class="sxs-lookup"><span data-stu-id="6d1c6-119">For **group** resource:</span></span><br /><span data-ttu-id="6d1c6-120">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d1c6-120">Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="6d1c6-121">Для ресурса **contact**:</span><span class="sxs-lookup"><span data-stu-id="6d1c6-121">For **contact** resource:</span></span><br /><span data-ttu-id="6d1c6-122">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6d1c6-122">Contacts.ReadWrite</span></span> |
|<span data-ttu-id="6d1c6-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6d1c6-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d1c6-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d1c6-124">Not supported.</span></span> |
|<span data-ttu-id="6d1c6-125">Для приложения</span><span class="sxs-lookup"><span data-stu-id="6d1c6-125">Application</span></span>                            | <span data-ttu-id="6d1c6-126">Для ресурса **user**:</span><span class="sxs-lookup"><span data-stu-id="6d1c6-126">For **user** resource:</span></span><br/><span data-ttu-id="6d1c6-127">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d1c6-127">User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="6d1c6-128">Для ресурса **group**:</span><span class="sxs-lookup"><span data-stu-id="6d1c6-128">For **group** resource:</span></span><br /><span data-ttu-id="6d1c6-129">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d1c6-129">Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="6d1c6-130">Для ресурса **contact**:</span><span class="sxs-lookup"><span data-stu-id="6d1c6-130">For **contact** resource:</span></span><br /><span data-ttu-id="6d1c6-131">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6d1c6-131">Contacts.ReadWrite</span></span> |

> <span data-ttu-id="6d1c6-p105">**Примечание.** Чтобы обновить фотографию какого-либо пользователя в организации, ваше приложение должно получить разрешение User.ReadWrite.All приложения и вызвать API с применением собственного идентификатора, не от имени пользователя. Дополнительные сведения см. в статье [Получение доступа без пользователя](/graph/auth-v2-service).</span><span class="sxs-lookup"><span data-stu-id="6d1c6-p105">**Note** To update the photo of any user in the organization, your app must have the User.ReadWrite.All application permission and call this API under its own identity, not on behalf of a user. To learn more, see [get access without a signed-in user](/graph/auth-v2-service).</span></span>

## <a name="http-request"></a><span data-ttu-id="6d1c6-134">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6d1c6-134">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="6d1c6-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6d1c6-135">Request headers</span></span>
| <span data-ttu-id="6d1c6-136">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6d1c6-136">Header</span></span>       | <span data-ttu-id="6d1c6-137">Значение</span><span class="sxs-lookup"><span data-stu-id="6d1c6-137">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6d1c6-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6d1c6-138">Authorization</span></span>  | <span data-ttu-id="6d1c6-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6d1c6-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6d1c6-141">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6d1c6-141">Content-Type</span></span>  | <span data-ttu-id="6d1c6-p107">image/jpeg. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6d1c6-p107">image/jpeg. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6d1c6-144">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6d1c6-144">Request body</span></span>
<span data-ttu-id="6d1c6-145">Включите в текст запроса двоичные данные фотографии.</span><span class="sxs-lookup"><span data-stu-id="6d1c6-145">In the request body, include the binary data of the photo in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="6d1c6-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d1c6-146">Response</span></span>

<span data-ttu-id="6d1c6-147">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="6d1c6-147">If successful, this method returns a `200 OK` response code.</span></span>
## <a name="example"></a><span data-ttu-id="6d1c6-148">Пример</span><span class="sxs-lookup"><span data-stu-id="6d1c6-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6d1c6-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="6d1c6-149">Request</span></span>
<span data-ttu-id="6d1c6-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6d1c6-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_profilephoto"
}-->
```http
PUT https://graph.microsoft.com/beta/me/photo/$value
Content-type: image/jpeg

Binary data for the image

```
##### <a name="response"></a><span data-ttu-id="6d1c6-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="6d1c6-151">Response</span></span>
<span data-ttu-id="6d1c6-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="6d1c6-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
