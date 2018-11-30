---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Отправка приглашения на доступ к элементу
ms.openlocfilehash: 3dc4d4a9c06b5e969476da2aa842db51f61346b2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076986"
---
# <a name="send-a-sharing-invitation"></a><span data-ttu-id="b21b0-102">Отправка приглашения к совместному использованию</span><span class="sxs-lookup"><span data-stu-id="b21b0-102">Send a sharing invitation</span></span>

> <span data-ttu-id="b21b0-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b21b0-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b21b0-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b21b0-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b21b0-p102">Отправляет приглашение к совместному использованию ресурса **DriveItem**. Приглашение к совместному использованию предоставляет получателям разрешения и при необходимости отправляет им на электронную почту уведомления, что к элементу был предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="b21b0-p102">Sends a sharing invitation for a **DriveItem**. A sharing invitation provides permissions to the recipients and optionally sends an email to the recipients to notify them the item was shared.</span></span>

## <a name="permissions"></a><span data-ttu-id="b21b0-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b21b0-107">Permissions</span></span>

<span data-ttu-id="b21b0-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b21b0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b21b0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b21b0-110">Permission type</span></span>      | <span data-ttu-id="b21b0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b21b0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b21b0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b21b0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b21b0-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b21b0-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="b21b0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b21b0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b21b0-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b21b0-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="b21b0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b21b0-116">Application</span></span> | <span data-ttu-id="b21b0-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b21b0-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b21b0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b21b0-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
POST /me/drive/items/{item-id}/invite
POST /sites/{siteId}/drive/items/{itemId}/invite
POST /users/{userId}/drive/items/{itemId}/invite
```

## <a name="request-body"></a><span data-ttu-id="b21b0-119">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b21b0-119">Request body</span></span>

<span data-ttu-id="b21b0-120">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="b21b0-120">In the request body, provide a JSON object with the following parameters.</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.inviteParameters", "scopes": "files.readwrite" } -->

```json
{
  "requireSignIn": false,
  "sendInvitation": false,
  "roles": [ "read | write"],
  "recipients": [
    { "@odata.type": "microsoft.graph.driveRecipient" },
    { "@odata.type": "microsoft.graph.driveRecipient" }
  ],
  "message": "string"
}
```

| <span data-ttu-id="b21b0-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="b21b0-121">Parameter</span></span>        | <span data-ttu-id="b21b0-122">Тип</span><span class="sxs-lookup"><span data-stu-id="b21b0-122">Type</span></span>                                            | <span data-ttu-id="b21b0-123">Описание</span><span class="sxs-lookup"><span data-stu-id="b21b0-123">Description</span></span>                                                                                                |
|:-----------------|:------------------------------------------------|:-----------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="b21b0-124">recipients</span><span class="sxs-lookup"><span data-stu-id="b21b0-124">recipients</span></span>       | <span data-ttu-id="b21b0-125">Collection([DriveRecipient](../resources/driverecipient.md))</span><span class="sxs-lookup"><span data-stu-id="b21b0-125">Collection([DriveRecipient](../resources/driverecipient.md))</span></span> | <span data-ttu-id="b21b0-126">Коллекция получателей, которые будут получать доступ и приглашение к совместному использованию.</span><span class="sxs-lookup"><span data-stu-id="b21b0-126">A collection of recipients who will receive access and the sharing invitation.</span></span>                                            |
| <span data-ttu-id="b21b0-127">message</span><span class="sxs-lookup"><span data-stu-id="b21b0-127">message</span></span>          | <span data-ttu-id="b21b0-128">String</span><span class="sxs-lookup"><span data-stu-id="b21b0-128">String</span></span>                                          | <span data-ttu-id="b21b0-p104">Сообщение с обычным форматированным текстом, включенное в приглашение на доступ. Максимальная длина составляет 2000 символов.</span><span class="sxs-lookup"><span data-stu-id="b21b0-p104">A plain text formatted message that is included in the sharing invitation. Maximum length 2000 characters.</span></span> |
| <span data-ttu-id="b21b0-131">requireSignIn</span><span class="sxs-lookup"><span data-stu-id="b21b0-131">requireSignIn</span></span>    | <span data-ttu-id="b21b0-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="b21b0-132">Boolean</span></span>                                         | <span data-ttu-id="b21b0-133">Указывает, куда должен зайти получатель приглашения, чтобы просмотреть элемент, к которому предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="b21b0-133">Specifies where the recipient of the invitation is required to sign-in to view the shared item.</span></span>            |
| <span data-ttu-id="b21b0-134">sendInvitation</span><span class="sxs-lookup"><span data-stu-id="b21b0-134">sendInvitation</span></span>   | <span data-ttu-id="b21b0-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="b21b0-135">Boolean</span></span>                                         | <span data-ttu-id="b21b0-136">Указывает, создано ли электронное письмо или запись (false) или разрешение (true).</span><span class="sxs-lookup"><span data-stu-id="b21b0-136">Specifies if an email or post is generated (false) or if the permission is just created (true).</span></span>            |
| <span data-ttu-id="b21b0-137">roles</span><span class="sxs-lookup"><span data-stu-id="b21b0-137">roles</span></span>            | <span data-ttu-id="b21b0-138">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="b21b0-138">Collection(String)</span></span>                              | <span data-ttu-id="b21b0-139">Указывает роли, которые необходимо предоставить получателям приглашения к совместному использованию.</span><span class="sxs-lookup"><span data-stu-id="b21b0-139">Specify the roles that are be granted to the recipients of the sharing invitation.</span></span>                         |

## <a name="example"></a><span data-ttu-id="b21b0-140">Пример</span><span class="sxs-lookup"><span data-stu-id="b21b0-140">Example</span></span>

<span data-ttu-id="b21b0-141">В этом примере показано, как отправить приглашение к совместному использованию пользователю с электронным адресом ryan@contoso.org и добавить сообщение о файле, над которым ведется совместная работа.</span><span class="sxs-lookup"><span data-stu-id="b21b0-141">This example sends a sharing invitation to a user with email address "ryan@contoso.org" with a message about a file being collaborated on.</span></span>
<span data-ttu-id="b21b0-142">Приглашение предоставляет пользователю Ryan доступ для чтения и записи к файлу.</span><span class="sxs-lookup"><span data-stu-id="b21b0-142">The invitation grants Ryan read-write access to the file.</span></span>

### <a name="http-request"></a><span data-ttu-id="b21b0-143">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b21b0-143">HTTP Request</span></span>

<span data-ttu-id="b21b0-144">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект коллекции [permission](../resources/permission.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b21b0-144">If successful, this method returns `200 OK` response code and [permission](../resources/permission.md) collection object in the response body.</span></span>

<!-- { "blockType": "request", "name": "send-sharing-invite", "@odata.type": "microsoft.graph.inviteParameters", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /me/drive/items/{item-id}/invite
Content-type: application/json

{
  "recipients": [
    {
      "email": "ryan@contoso.org"
    }
  ],
  "message": "Here's the file that we're collaborating on.",
  "requireSignIn": true,
  "sendInvitation": true,
  "roles": [ "write" ]
}
```

### <a name="response"></a><span data-ttu-id="b21b0-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="b21b0-145">Response</span></span>

<span data-ttu-id="b21b0-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b21b0-146">Here is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "grantedTo": {
        "user": {
          "displayName": "Ryan Gregg",
          "id": "42F177F1-22C0-4BE3-900D-4507125C5C20"
        }
      },
      "id": "CCFC7CA3-7A19-4D57-8CEF-149DB9DDFA62",
      "invitation": {
        "email": "ryan@contoso.com",
        "signInRequired": true
      },
      "roles": [ "write" ]
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="b21b0-147">Примечания</span><span class="sxs-lookup"><span data-stu-id="b21b0-147">Remarks</span></span>

* <span data-ttu-id="b21b0-148">[Дискам](../resources/drive.md), у которых параметр **driveType** имеет значение `personal` (OneDrive персональный), не удастся создать или изменить разрешения в корневой папке ресурса DriveItem.</span><span class="sxs-lookup"><span data-stu-id="b21b0-148">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive personal) cannot create or modify permissions on the root DriveItem.</span></span>
* <span data-ttu-id="b21b0-149">Список доступных ролей см. в разделе [Перечисление ролей](../resources/permission.md#roles-enumeration-values).</span><span class="sxs-lookup"><span data-stu-id="b21b0-149">For a list of available roles, see [Roles enumeration](../resources/permission.md#roles-enumeration-values).</span></span>

## <a name="error-responses"></a><span data-ttu-id="b21b0-150">Отклики с ошибками</span><span class="sxs-lookup"><span data-stu-id="b21b0-150">Error Responses</span></span>

<span data-ttu-id="b21b0-151">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="b21b0-151">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>


[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Add permissions to an item and optionally send a sharing notification.",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Sharing/Add permissions"
} -->
