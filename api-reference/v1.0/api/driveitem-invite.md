---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Отправка приглашения на доступ к элементу
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: f7d3a974143b738b966a8953848f4837c16cd6c8
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480742"
---
# <a name="send-a-sharing-invitation"></a><span data-ttu-id="7a79f-102">Отправка приглашения к совместному использованию</span><span class="sxs-lookup"><span data-stu-id="7a79f-102">Send a sharing invitation</span></span>

<span data-ttu-id="7a79f-103">Отправляет приглашение к совместному использованию ресурса **DriveItem**.</span><span class="sxs-lookup"><span data-stu-id="7a79f-103">Sends a sharing invitation for a **DriveItem**.</span></span>
<span data-ttu-id="7a79f-104">Приглашение к совместному использованию предоставляет разрешения получателям и при необходимости отправляет им сообщение электронной почты с [ссылкой для совместного доступа][].</span><span class="sxs-lookup"><span data-stu-id="7a79f-104">A sharing invitation provides permissions to the recipients and optionally sends them an email with a [sharing link][].</span></span>

## <a name="permissions"></a><span data-ttu-id="7a79f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7a79f-105">Permissions</span></span>

<span data-ttu-id="7a79f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a79f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a79f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7a79f-108">Permission type</span></span>      | <span data-ttu-id="7a79f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7a79f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7a79f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7a79f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7a79f-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a79f-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="7a79f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7a79f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7a79f-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a79f-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="7a79f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7a79f-114">Application</span></span> | <span data-ttu-id="7a79f-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a79f-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7a79f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7a79f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
POST /me/drive/items/{item-id}/invite
POST /sites/{siteId}/drive/items/{itemId}/invite
POST /users/{userId}/drive/items/{itemId}/invite
```

## <a name="request-body"></a><span data-ttu-id="7a79f-117">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7a79f-117">Request body</span></span>

<span data-ttu-id="7a79f-118">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="7a79f-118">In the request body, provide a JSON object with the following parameters.</span></span>

<!-- { "blockType": "ignored", "scopes": "files.readwrite" } -->

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

| <span data-ttu-id="7a79f-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="7a79f-119">Parameter</span></span>        | <span data-ttu-id="7a79f-120">Тип</span><span class="sxs-lookup"><span data-stu-id="7a79f-120">Type</span></span>                           | <span data-ttu-id="7a79f-121">Описание</span><span class="sxs-lookup"><span data-stu-id="7a79f-121">Description</span></span>
|:-----------------|:-------------------------------|:-------------------------
| <span data-ttu-id="7a79f-122">recipients</span><span class="sxs-lookup"><span data-stu-id="7a79f-122">recipients</span></span>       | <span data-ttu-id="7a79f-123">Collection([DriveRecipient][])</span><span class="sxs-lookup"><span data-stu-id="7a79f-123">Collection([DriveRecipient][])</span></span> | <span data-ttu-id="7a79f-124">Коллекция получателей, которые будут получать доступ и приглашение к совместному использованию.</span><span class="sxs-lookup"><span data-stu-id="7a79f-124">A collection of recipients who will receive access and the sharing invitation.</span></span>
| <span data-ttu-id="7a79f-125">message</span><span class="sxs-lookup"><span data-stu-id="7a79f-125">message</span></span>          | <span data-ttu-id="7a79f-126">String</span><span class="sxs-lookup"><span data-stu-id="7a79f-126">String</span></span>                         | <span data-ttu-id="7a79f-p103">Сообщение с обычным форматированным текстом, включенное в приглашение на доступ. Максимальная длина составляет 2000 символов.</span><span class="sxs-lookup"><span data-stu-id="7a79f-p103">A plain text formatted message that is included in the sharing invitation. Maximum length 2000 characters.</span></span>
| <span data-ttu-id="7a79f-129">requireSignIn</span><span class="sxs-lookup"><span data-stu-id="7a79f-129">requireSignIn</span></span>    | <span data-ttu-id="7a79f-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="7a79f-130">Boolean</span></span>                        | <span data-ttu-id="7a79f-131">Указывает, требуется ли получателю приглашения на вход для просмотра общего элемента.</span><span class="sxs-lookup"><span data-stu-id="7a79f-131">Specifies whether the recipient of the invitation is required to sign-in to view the shared item.</span></span>
| <span data-ttu-id="7a79f-132">sendInvitation</span><span class="sxs-lookup"><span data-stu-id="7a79f-132">sendInvitation</span></span>   | <span data-ttu-id="7a79f-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="7a79f-133">Boolean</span></span>                        | <span data-ttu-id="7a79f-134">Если этот параметр имеет значение true, получателю отправляется [ссылка для совместного доступа][] .</span><span class="sxs-lookup"><span data-stu-id="7a79f-134">If true, a [sharing link][] is sent to the recipient.</span></span> <span data-ttu-id="7a79f-135">В противном случае разрешение предоставляется напрямую без отправки уведомления.</span><span class="sxs-lookup"><span data-stu-id="7a79f-135">Otherwise, a permission is granted directly without sending a notification.</span></span>
| <span data-ttu-id="7a79f-136">roles</span><span class="sxs-lookup"><span data-stu-id="7a79f-136">roles</span></span>            | <span data-ttu-id="7a79f-137">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="7a79f-137">Collection(String)</span></span>             | <span data-ttu-id="7a79f-138">Укажите роли, которые должны быть предоставлены получателям приглашения к совместному использованию.</span><span class="sxs-lookup"><span data-stu-id="7a79f-138">Specify the roles that are to be granted to the recipients of the sharing invitation.</span></span>

## <a name="example"></a><span data-ttu-id="7a79f-139">Пример</span><span class="sxs-lookup"><span data-stu-id="7a79f-139">Example</span></span>

<span data-ttu-id="7a79f-140">В этом примере показано, как отправить приглашение к совместному использованию пользователю с адресом электронной почты "ryan@contoso.com" с сообщением о том, что файл работает совместно.</span><span class="sxs-lookup"><span data-stu-id="7a79f-140">This example sends a sharing invitation to a user with email address "ryan@contoso.com" with a message about a file being collaborated on.</span></span>
<span data-ttu-id="7a79f-141">Приглашение предоставляет пользователю Ryan доступ для чтения и записи к файлу.</span><span class="sxs-lookup"><span data-stu-id="7a79f-141">The invitation grants Ryan read-write access to the file.</span></span>

### <a name="http-request"></a><span data-ttu-id="7a79f-142">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7a79f-142">HTTP Request</span></span>

<span data-ttu-id="7a79f-143">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект коллекции [permission](../resources/permission.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7a79f-143">If successful, this method returns `200 OK` response code and [permission](../resources/permission.md) collection object in the response body.</span></span>

<!-- { "blockType": "request", "name": "send-sharing-invite", "scopes": "files.readwrite", "target": "action" } -->

```json
POST /me/drive/items/{item-id}/invite
Content-type: application/json

{
  "recipients": [
    {
      "email": "ryan@contoso.com"
    }
  ],
  "message": "Here's the file that we're collaborating on.",
  "requireSignIn": true,
  "sendInvitation": true,
  "roles": [ "write" ]
}
```

### <a name="response"></a><span data-ttu-id="7a79f-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a79f-144">Response</span></span>

<span data-ttu-id="7a79f-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7a79f-145">Here is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

```json
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

## <a name="remarks"></a><span data-ttu-id="7a79f-146">Замечания</span><span class="sxs-lookup"><span data-stu-id="7a79f-146">Remarks</span></span>

* <span data-ttu-id="7a79f-147">[Дискам](../resources/drive.md), у которых параметр **driveType** имеет значение `personal` (OneDrive персональный), не удастся создать или изменить разрешения в корневой папке ресурса DriveItem.</span><span class="sxs-lookup"><span data-stu-id="7a79f-147">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive personal) cannot create or modify permissions on the root DriveItem.</span></span>
* <span data-ttu-id="7a79f-148">Список доступных ролей см. в разделе [Перечисление ролей](../resources/permission.md#roles-enumeration).</span><span class="sxs-lookup"><span data-stu-id="7a79f-148">For a list of available roles, see [Roles enumeration](../resources/permission.md#roles-enumeration).</span></span>

## <a name="error-responses"></a><span data-ttu-id="7a79f-149">Отклики с ошибками</span><span class="sxs-lookup"><span data-stu-id="7a79f-149">Error Responses</span></span>

<span data-ttu-id="7a79f-150">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="7a79f-150">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>


[driveRecipient]: ../resources/driverecipient.md
[error-response]: /graph/errors
[Ссылка для совместного доступа]: ../resources/permission.md#sharing-links
[sharing link]: ../resources/permission.md#sharing-links

<!-- {
  "type": "#page.annotation",
  "description": "Add permissions to an item and optionally send a sharing notification.",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Sharing/Add permissions"
} -->
