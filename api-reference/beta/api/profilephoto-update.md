---
title: Обновление объекта profilephoto
description: Обновление фотографий для любого пользователя, в том числе выполнил вход для клиентов пользователя, или указанной группы или контакта. Начиная с него
localization_priority: Normal
ms.openlocfilehash: e79a58d92276cc88884874c0a3339d52ac8c2847
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850885"
---
# <a name="update-profilephoto"></a><span data-ttu-id="4b555-104">Обновление объекта profilephoto</span><span class="sxs-lookup"><span data-stu-id="4b555-104">Update profilephoto</span></span>

> <span data-ttu-id="4b555-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4b555-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4b555-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b555-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4b555-107">Обновление фотографий для любого пользователя, в том числе выполнил вход для клиентов пользователя, или указанной группы или контакта.</span><span class="sxs-lookup"><span data-stu-id="4b555-107">Update the photo for any user in the tenant including the signed-in user, or the specified group or contact.</span></span> <span data-ttu-id="4b555-108">Поскольку в настоящее время не более 4 МБ на общий размер каждого запроса REST, этот параметр ограничивает размер фотографию, которую можно добавить в разделе 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="4b555-108">Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the photo you can add to under 4MB.</span></span>

<span data-ttu-id="4b555-109">Используйте только PUT для этой операции в бета-версии.</span><span class="sxs-lookup"><span data-stu-id="4b555-109">Use only PUT for this operation in the beta version.</span></span>

> <span data-ttu-id="4b555-110">**Примечание** Операция обновления фотографий в бета-версии поддерживает только пользователя рабочих или почтовые ящики school и не личные почтовые ящики.</span><span class="sxs-lookup"><span data-stu-id="4b555-110">**Note** The update photo operation in beta supports only the user's work or school mailboxes and not personal mailboxes.</span></span>

## <a name="permissions"></a><span data-ttu-id="4b555-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4b555-111">Permissions</span></span>
<span data-ttu-id="4b555-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b555-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b555-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b555-114">Permission type</span></span>      | <span data-ttu-id="4b555-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b555-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b555-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b555-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="4b555-117">Фотографий профиля выполнившего вход **пользователя**:</span><span class="sxs-lookup"><span data-stu-id="4b555-117">Profile photo of the signed-in **user**:</span></span><br/><span data-ttu-id="4b555-118">User.ReadWrite User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b555-118">User.ReadWrite, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="4b555-119">Для ресурса **group**:</span><span class="sxs-lookup"><span data-stu-id="4b555-119">For **group** resource:</span></span><br /><span data-ttu-id="4b555-120">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b555-120">Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="4b555-121">Для ресурса **contact**:</span><span class="sxs-lookup"><span data-stu-id="4b555-121">For **contact** resource:</span></span><br /><span data-ttu-id="4b555-122">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4b555-122">Contacts.ReadWrite</span></span> |
|<span data-ttu-id="4b555-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b555-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b555-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b555-124">Not supported.</span></span> |
|<span data-ttu-id="4b555-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4b555-125">Application</span></span>                            | <span data-ttu-id="4b555-126">Для ресурса **user**:</span><span class="sxs-lookup"><span data-stu-id="4b555-126">For **user** resource:</span></span><br/><span data-ttu-id="4b555-127">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b555-127">User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="4b555-128">Для ресурса **group**:</span><span class="sxs-lookup"><span data-stu-id="4b555-128">For **group** resource:</span></span><br /><span data-ttu-id="4b555-129">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b555-129">Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="4b555-130">Для ресурса **contact**:</span><span class="sxs-lookup"><span data-stu-id="4b555-130">For **contact** resource:</span></span><br /><span data-ttu-id="4b555-131">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4b555-131">Contacts.ReadWrite</span></span> |

> <span data-ttu-id="4b555-p105">**Примечание.** Чтобы обновить фотографию какого-либо пользователя в организации, ваше приложение должно получить разрешение User.ReadWrite.All приложения и вызвать API с применением собственного идентификатора, не от имени пользователя. Дополнительные сведения см. в статье [Получение доступа без пользователя](/graph/auth-v2-service).</span><span class="sxs-lookup"><span data-stu-id="4b555-p105">**Note** To update the photo of any user in the organization, your app must have the User.ReadWrite.All application permission and call this API under its own identity, not on behalf of a user. To learn more, see [get access without a signed-in user](/graph/auth-v2-service).</span></span>

## <a name="http-request"></a><span data-ttu-id="4b555-134">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b555-134">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="4b555-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4b555-135">Request headers</span></span>
| <span data-ttu-id="4b555-136">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4b555-136">Header</span></span>       | <span data-ttu-id="4b555-137">Значение</span><span class="sxs-lookup"><span data-stu-id="4b555-137">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4b555-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4b555-138">Authorization</span></span>  | <span data-ttu-id="4b555-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b555-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4b555-141">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4b555-141">Content-Type</span></span>  | <span data-ttu-id="4b555-p107">image/jpeg. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b555-p107">image/jpeg. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4b555-144">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4b555-144">Request body</span></span>
<span data-ttu-id="4b555-145">Включите в текст запроса двоичные данные фотографии.</span><span class="sxs-lookup"><span data-stu-id="4b555-145">In the request body, include the binary data of the photo in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="4b555-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b555-146">Response</span></span>

<span data-ttu-id="4b555-147">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="4b555-147">If successful, this method returns a `200 OK` response code.</span></span>
## <a name="example"></a><span data-ttu-id="4b555-148">Пример</span><span class="sxs-lookup"><span data-stu-id="4b555-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4b555-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b555-149">Request</span></span>
<span data-ttu-id="4b555-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b555-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_profilephoto"
}-->
```http
PUT https://graph.microsoft.com/beta/me/photo/$value
Content-type: image/jpeg

Binary data for the image

```
##### <a name="response"></a><span data-ttu-id="4b555-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="4b555-151">Response</span></span>
<span data-ttu-id="4b555-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4b555-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
