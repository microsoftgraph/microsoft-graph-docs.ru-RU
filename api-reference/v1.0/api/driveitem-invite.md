---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Отправка приглашения на доступ к элементу
localization_priority: Normal
ms.prod: sharepoint
description: Отправляет приглашение к совместному использованию ресурса DriveItem.
doc_type: apiPageType
ms.openlocfilehash: 129cbeaf43c9c409b645a7a94b8b4a3371329a8b
ms.sourcegitcommit: 6db0b7a473594653dda332ce7da45ea2ad90772b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/04/2020
ms.locfileid: "43146424"
---
# <a name="send-a-sharing-invitation"></a><span data-ttu-id="e290c-103">Отправка приглашения к совместному использованию</span><span class="sxs-lookup"><span data-stu-id="e290c-103">Send a sharing invitation</span></span>

<span data-ttu-id="e290c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e290c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e290c-105">Отправляет приглашение к совместному использованию ресурса **DriveItem**.</span><span class="sxs-lookup"><span data-stu-id="e290c-105">Sends a sharing invitation for a **DriveItem**.</span></span>
<span data-ttu-id="e290c-106">Приглашение к совместному использованию предоставляет получателям разрешения и при необходимости отправляет им сообщение электронной почты с [ссылкой совместного доступа][].</span><span class="sxs-lookup"><span data-stu-id="e290c-106">A sharing invitation provides permissions to the recipients and optionally sends them an email with a [sharing link][].</span></span>

## <a name="permissions"></a><span data-ttu-id="e290c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e290c-107">Permissions</span></span>

<span data-ttu-id="e290c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e290c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e290c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e290c-110">Permission type</span></span>      | <span data-ttu-id="e290c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e290c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e290c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e290c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e290c-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e290c-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="e290c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e290c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e290c-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e290c-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="e290c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e290c-116">Application</span></span> | <span data-ttu-id="e290c-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e290c-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e290c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e290c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
POST /me/drive/items/{item-id}/invite
POST /sites/{siteId}/drive/items/{itemId}/invite
POST /users/{userId}/drive/items/{itemId}/invite
```

## <a name="request-body"></a><span data-ttu-id="e290c-119">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e290c-119">Request body</span></span>

<span data-ttu-id="e290c-120">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="e290c-120">In the request body, provide a JSON object with the following parameters.</span></span>

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

| <span data-ttu-id="e290c-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="e290c-121">Parameter</span></span>        | <span data-ttu-id="e290c-122">Тип</span><span class="sxs-lookup"><span data-stu-id="e290c-122">Type</span></span>                           | <span data-ttu-id="e290c-123">Описание</span><span class="sxs-lookup"><span data-stu-id="e290c-123">Description</span></span>
|:-----------------|:-------------------------------|:-------------------------
| <span data-ttu-id="e290c-124">recipients</span><span class="sxs-lookup"><span data-stu-id="e290c-124">recipients</span></span>       | <span data-ttu-id="e290c-125">Collection([DriveRecipient][])</span><span class="sxs-lookup"><span data-stu-id="e290c-125">Collection([DriveRecipient][])</span></span> | <span data-ttu-id="e290c-126">Коллекция получателей, которые будут получать доступ и приглашение к совместному использованию.</span><span class="sxs-lookup"><span data-stu-id="e290c-126">A collection of recipients who will receive access and the sharing invitation.</span></span>
| <span data-ttu-id="e290c-127">message</span><span class="sxs-lookup"><span data-stu-id="e290c-127">message</span></span>          | <span data-ttu-id="e290c-128">String</span><span class="sxs-lookup"><span data-stu-id="e290c-128">String</span></span>                         | <span data-ttu-id="e290c-p103">Сообщение с обычным форматированным текстом, включенное в приглашение на доступ. Максимальная длина составляет 2000 символов.</span><span class="sxs-lookup"><span data-stu-id="e290c-p103">A plain text formatted message that is included in the sharing invitation. Maximum length 2000 characters.</span></span>
| <span data-ttu-id="e290c-131">requireSignIn</span><span class="sxs-lookup"><span data-stu-id="e290c-131">requireSignIn</span></span>    | <span data-ttu-id="e290c-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="e290c-132">Boolean</span></span>                        | <span data-ttu-id="e290c-133">Указывает, должен ли получатель приглашения выполнить вход, чтобы просмотреть элемент, к которому предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="e290c-133">Specifies whether the recipient of the invitation is required to sign-in to view the shared item.</span></span>
| <span data-ttu-id="e290c-134">sendInvitation</span><span class="sxs-lookup"><span data-stu-id="e290c-134">sendInvitation</span></span>   | <span data-ttu-id="e290c-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="e290c-135">Boolean</span></span>                        | <span data-ttu-id="e290c-136">Если указано значение true, получателю отправляется [ссылка совместного доступа][].</span><span class="sxs-lookup"><span data-stu-id="e290c-136">If true, a [sharing link][] is sent to the recipient.</span></span> <span data-ttu-id="e290c-137">В противном случае разрешение предоставляется напрямую без отправки уведомления.</span><span class="sxs-lookup"><span data-stu-id="e290c-137">Otherwise, a permission is granted directly without sending a notification.</span></span>
| <span data-ttu-id="e290c-138">roles</span><span class="sxs-lookup"><span data-stu-id="e290c-138">roles</span></span>            | <span data-ttu-id="e290c-139">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="e290c-139">Collection(String)</span></span>             | <span data-ttu-id="e290c-140">Указывает роли, которые необходимо предоставить получателям приглашения к совместному использованию.</span><span class="sxs-lookup"><span data-stu-id="e290c-140">Specify the roles that are to be granted to the recipients of the sharing invitation.</span></span>

## <a name="example"></a><span data-ttu-id="e290c-141">Пример</span><span class="sxs-lookup"><span data-stu-id="e290c-141">Example</span></span>

<span data-ttu-id="e290c-142">В этом примере показано, как отправить приглашение к совместному использованию пользователю с электронным адресом ryan@contoso.com и добавить сообщение о файле, над которым ведется совместная работа.</span><span class="sxs-lookup"><span data-stu-id="e290c-142">This example sends a sharing invitation to a user with email address "ryan@contoso.com" with a message about a file being collaborated on.</span></span>
<span data-ttu-id="e290c-143">Приглашение предоставляет пользователю Ryan доступ для чтения и записи к файлу.</span><span class="sxs-lookup"><span data-stu-id="e290c-143">The invitation grants Ryan read-write access to the file.</span></span>

### <a name="http-request"></a><span data-ttu-id="e290c-144">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e290c-144">HTTP Request</span></span>

<span data-ttu-id="e290c-145">При успешном выполнении этот метод возвращает код ответа `200 OK` и объект коллекции [permission](../resources/permission.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e290c-145">If successful, this method returns `200 OK` response code and [permission](../resources/permission.md) collection object in the response body.</span></span>


# <a name="http"></a>[<span data-ttu-id="e290c-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="e290c-146">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e290c-147">C#</span><span class="sxs-lookup"><span data-stu-id="e290c-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/send-sharing-invite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e290c-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e290c-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/send-sharing-invite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e290c-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e290c-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/send-sharing-invite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e290c-150">Java</span><span class="sxs-lookup"><span data-stu-id="e290c-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/send-sharing-invite-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e290c-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="e290c-151">Response</span></span>

<span data-ttu-id="e290c-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e290c-152">Here is an example of the response.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="e290c-153">Примечания</span><span class="sxs-lookup"><span data-stu-id="e290c-153">Remarks</span></span>

* <span data-ttu-id="e290c-154">[Дискам](../resources/drive.md), у которых параметр **driveType** имеет значение `personal` (OneDrive персональный), не удастся создать или изменить разрешения в корневой папке ресурса DriveItem.</span><span class="sxs-lookup"><span data-stu-id="e290c-154">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive personal) cannot create or modify permissions on the root DriveItem.</span></span>
* <span data-ttu-id="e290c-155">Список доступных ролей приведен в разделе [значения свойств Roles](../resources/permission.md#roles-property-values).</span><span class="sxs-lookup"><span data-stu-id="e290c-155">For a list of available roles, see [roles property values](../resources/permission.md#roles-property-values).</span></span>

## <a name="error-responses"></a><span data-ttu-id="e290c-156">Ответы с ошибками</span><span class="sxs-lookup"><span data-stu-id="e290c-156">Error Responses</span></span>

<span data-ttu-id="e290c-157">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="e290c-157">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>


[driveRecipient]: ../resources/driverecipient.md
[error-response]: /graph/errors
[ссылка совместного доступа]: ../resources/permission.md#sharing-links
[sharing link]: ../resources/permission.md#sharing-links

<!-- {
  "type": "#page.annotation",
  "description": "Add permissions to an item and optionally send a sharing notification.",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Sharing/Add permissions",
  "suppressions": [
  ]
} -->
