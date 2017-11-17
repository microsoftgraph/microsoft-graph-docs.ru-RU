---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: "Отправка приглашения на доступ к элементу"
ms.openlocfilehash: 5be2060c190434c4b9d587d20fe68d69786b3aa5
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="send-a-sharing-invitation"></a><span data-ttu-id="53d4c-102">Отправка приглашения к совместному использованию</span><span class="sxs-lookup"><span data-stu-id="53d4c-102">Send a sharing invitation</span></span>

<span data-ttu-id="53d4c-p101">Отправляет приглашение к совместному использованию ресурса **DriveItem**. Приглашение к совместному использованию предоставляет получателям разрешения и при необходимости отправляет им на электронную почту уведомления, что к элементу был предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="53d4c-p101">Sends a sharing invitation for a **DriveItem**. A sharing invitation provides permissions to the recipients and optionally sends an email to the recipients to notify them the item was shared.</span></span>

## <a name="permissions"></a><span data-ttu-id="53d4c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="53d4c-105">Permissions</span></span>

<span data-ttu-id="53d4c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="53d4c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="53d4c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53d4c-108">Permission type</span></span>      | <span data-ttu-id="53d4c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="53d4c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53d4c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53d4c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="53d4c-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53d4c-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="53d4c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53d4c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53d4c-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53d4c-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="53d4c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="53d4c-114">Application</span></span> | <span data-ttu-id="53d4c-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53d4c-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="53d4c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53d4c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
POST /me/drive/items/{item-id}/invite
POST /sites/{siteId}/drive/items/{itemId}/invite
POST /users/{userId}/drive/items/{itemId}/invite
```

## <a name="request-body"></a><span data-ttu-id="53d4c-117">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="53d4c-117">Request body</span></span>

<span data-ttu-id="53d4c-118">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="53d4c-118">In the request body, provide a JSON object with the following parameters.</span></span>

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

| <span data-ttu-id="53d4c-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="53d4c-119">Parameter</span></span>        | <span data-ttu-id="53d4c-120">Тип</span><span class="sxs-lookup"><span data-stu-id="53d4c-120">Type</span></span>                                            | <span data-ttu-id="53d4c-121">Описание</span><span class="sxs-lookup"><span data-stu-id="53d4c-121">Description</span></span>                                                                                                |
|:-----------------|:------------------------------------------------|:-----------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="53d4c-122">recipients</span><span class="sxs-lookup"><span data-stu-id="53d4c-122">recipients</span></span>       | <span data-ttu-id="53d4c-123">Collection([DriveRecipient](../resources/driverecipient.md))</span><span class="sxs-lookup"><span data-stu-id="53d4c-123">Collection([DriveRecipient](../resources/driverecipient.md))</span></span> | <span data-ttu-id="53d4c-124">Коллекция получателей, которые будут получать доступ и приглашение к совместному использованию.</span><span class="sxs-lookup"><span data-stu-id="53d4c-124">A collection of recipients who will receive access and the sharing invitation.</span></span>                                            |
| <span data-ttu-id="53d4c-125">message</span><span class="sxs-lookup"><span data-stu-id="53d4c-125">message</span></span>          | <span data-ttu-id="53d4c-126">String</span><span class="sxs-lookup"><span data-stu-id="53d4c-126">String</span></span>                                          | <span data-ttu-id="53d4c-p103">Сообщение с обычным форматированным текстом, включенное в приглашение на доступ. Максимальная длина составляет 2000 символов.</span><span class="sxs-lookup"><span data-stu-id="53d4c-p103">A plain text formatted message that is included in the sharing invitation. Maximum length 2000 characters.</span></span> |
| <span data-ttu-id="53d4c-129">requireSignIn</span><span class="sxs-lookup"><span data-stu-id="53d4c-129">requireSignIn</span></span>    | <span data-ttu-id="53d4c-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="53d4c-130">Boolean</span></span>                                         | <span data-ttu-id="53d4c-131">Указывает, куда должен зайти получатель приглашения, чтобы просмотреть элемент, к которому предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="53d4c-131">Specifies where the recipient of the invitation is required to sign-in to view the shared item.</span></span>            |
| <span data-ttu-id="53d4c-132">sendInvitation</span><span class="sxs-lookup"><span data-stu-id="53d4c-132">sendInvitation</span></span>   | <span data-ttu-id="53d4c-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="53d4c-133">Boolean</span></span>                                         | <span data-ttu-id="53d4c-134">Указывает, создано ли электронное письмо или запись (false) или разрешение (true).</span><span class="sxs-lookup"><span data-stu-id="53d4c-134">Specifies if an email or post is generated (false) or if the permission is just created (true).</span></span>            |
| <span data-ttu-id="53d4c-135">roles</span><span class="sxs-lookup"><span data-stu-id="53d4c-135">roles</span></span>            | <span data-ttu-id="53d4c-136">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="53d4c-136">Collection(String)</span></span>                              | <span data-ttu-id="53d4c-137">Указывает роли, которые необходимо предоставить получателям приглашения к совместному использованию.</span><span class="sxs-lookup"><span data-stu-id="53d4c-137">Specify the roles that are be granted to the recipients of the sharing invitation.</span></span>                         |

## <a name="example"></a><span data-ttu-id="53d4c-138">Пример</span><span class="sxs-lookup"><span data-stu-id="53d4c-138">Example</span></span>

<span data-ttu-id="53d4c-139">В этот примере показано, как отправить приглашение к совместному использованию пользователю с электронным адресом ryan@contoso.org и добавить сообщение о файле, над которым ведется совместная работа.</span><span class="sxs-lookup"><span data-stu-id="53d4c-139">This example sends a sharing invitation to a user with email address "ryan@contoso.org" with a message about a file being collaborated on.</span></span>
<span data-ttu-id="53d4c-140">Приглашение предоставляет пользователю Ryan доступ для чтения и записи к файлу.</span><span class="sxs-lookup"><span data-stu-id="53d4c-140">The invitation grants Ryan read-write access to the file.</span></span>

### <a name="http-request"></a><span data-ttu-id="53d4c-141">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53d4c-141">HTTP Request</span></span>

<span data-ttu-id="53d4c-142">При успешном выполнении этот метод возвращает код ответа `200 OK` и объект коллекции [permission](../resources/permission.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="53d4c-142">If successful, this method returns `200 OK` response code and [permission](../resources/permission.md) collection object in the response body.</span></span>

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

### <a name="response"></a><span data-ttu-id="53d4c-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="53d4c-143">Response</span></span>

<span data-ttu-id="53d4c-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="53d4c-144">Here is an example of the response.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="53d4c-145">Примечания</span><span class="sxs-lookup"><span data-stu-id="53d4c-145">Remarks</span></span>

* <span data-ttu-id="53d4c-146">[Дискам](../resources/drive.md), у которых параметр **driveType** имеет значение `personal` (OneDrive персональный), не удастся создать или изменить разрешения в корневой папке ресурса DriveItem.</span><span class="sxs-lookup"><span data-stu-id="53d4c-146">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive Personal) cannot create or modify permissions on the root DriveItem.</span></span>
* <span data-ttu-id="53d4c-147">Список доступных ролей см. в таблице [Перечисление ролей](../resources/permission.md#roles-enumeration).</span><span class="sxs-lookup"><span data-stu-id="53d4c-147">For a list of available roles, see [Roles enumeration](../resources/permission.md#roles-enumeration).</span></span>

## <a name="error-responses"></a><span data-ttu-id="53d4c-148">Ответы с ошибками</span><span class="sxs-lookup"><span data-stu-id="53d4c-148">Error Responses</span></span>

<span data-ttu-id="53d4c-149">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="53d4c-149">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>


[error-response]: ../../../concepts/errors.md

<!-- {
  "type": "#page.annotation",
  "description": "Add permissions to an item and optionally send a sharing notification.",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Sharing/Add permissions"
} -->
