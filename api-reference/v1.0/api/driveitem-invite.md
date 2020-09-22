---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Отправка приглашения на доступ к элементу
localization_priority: Normal
ms.prod: sharepoint
description: Отправляет приглашение на доступ к driveItem.
doc_type: apiPageType
ms.openlocfilehash: 0ef9d44623dd27f8172aeaaf07d4ce0d129eae7f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48042151"
---
# <a name="send-a-sharing-invitation"></a><span data-ttu-id="176d3-103">Отправка приглашения к совместному использованию</span><span class="sxs-lookup"><span data-stu-id="176d3-103">Send a sharing invitation</span></span>

<span data-ttu-id="176d3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="176d3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="176d3-105">Отправляет приглашение на доступ к **driveItem**.</span><span class="sxs-lookup"><span data-stu-id="176d3-105">Sends a sharing invitation for a **driveItem**.</span></span>
<span data-ttu-id="176d3-106">Приглашение к совместному использованию предоставляет получателям разрешения и при необходимости отправляет им сообщение электронной почты с [ссылкой совместного доступа][].</span><span class="sxs-lookup"><span data-stu-id="176d3-106">A sharing invitation provides permissions to the recipients and optionally sends them an email with a [sharing link][].</span></span>

## <a name="permissions"></a><span data-ttu-id="176d3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="176d3-107">Permissions</span></span>

<span data-ttu-id="176d3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="176d3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="176d3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="176d3-110">Permission type</span></span>      | <span data-ttu-id="176d3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="176d3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="176d3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="176d3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="176d3-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="176d3-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="176d3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="176d3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="176d3-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="176d3-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="176d3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="176d3-116">Application</span></span> | <span data-ttu-id="176d3-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="176d3-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="176d3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="176d3-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
POST /me/drive/items/{item-id}/invite
POST /sites/{siteId}/drive/items/{itemId}/invite
POST /users/{userId}/drive/items/{itemId}/invite
```

## <a name="request-body"></a><span data-ttu-id="176d3-119">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="176d3-119">Request body</span></span>

<span data-ttu-id="176d3-120">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="176d3-120">In the request body, provide a JSON object with the following parameters.</span></span>

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

| <span data-ttu-id="176d3-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="176d3-121">Parameter</span></span>        | <span data-ttu-id="176d3-122">Тип</span><span class="sxs-lookup"><span data-stu-id="176d3-122">Type</span></span>                           | <span data-ttu-id="176d3-123">Описание</span><span class="sxs-lookup"><span data-stu-id="176d3-123">Description</span></span>
|:-----------------|:-------------------------------|:-------------------------
| <span data-ttu-id="176d3-124">recipients</span><span class="sxs-lookup"><span data-stu-id="176d3-124">recipients</span></span>       | <span data-ttu-id="176d3-125">Collection([DriveRecipient][])</span><span class="sxs-lookup"><span data-stu-id="176d3-125">Collection([DriveRecipient][])</span></span> | <span data-ttu-id="176d3-126">Коллекция получателей, которые будут получать доступ и приглашение к совместному использованию.</span><span class="sxs-lookup"><span data-stu-id="176d3-126">A collection of recipients who will receive access and the sharing invitation.</span></span>
| <span data-ttu-id="176d3-127">message</span><span class="sxs-lookup"><span data-stu-id="176d3-127">message</span></span>          | <span data-ttu-id="176d3-128">String</span><span class="sxs-lookup"><span data-stu-id="176d3-128">String</span></span>                         | <span data-ttu-id="176d3-p103">Сообщение с обычным форматированным текстом, включенное в приглашение на доступ. Максимальная длина составляет 2000 символов.</span><span class="sxs-lookup"><span data-stu-id="176d3-p103">A plain text formatted message that is included in the sharing invitation. Maximum length 2000 characters.</span></span>
| <span data-ttu-id="176d3-131">requireSignIn</span><span class="sxs-lookup"><span data-stu-id="176d3-131">requireSignIn</span></span>    | <span data-ttu-id="176d3-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="176d3-132">Boolean</span></span>                        | <span data-ttu-id="176d3-133">Указывает, должен ли получатель приглашения выполнить вход, чтобы просмотреть элемент, к которому предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="176d3-133">Specifies whether the recipient of the invitation is required to sign-in to view the shared item.</span></span>
| <span data-ttu-id="176d3-134">sendInvitation</span><span class="sxs-lookup"><span data-stu-id="176d3-134">sendInvitation</span></span>   | <span data-ttu-id="176d3-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="176d3-135">Boolean</span></span>                        | <span data-ttu-id="176d3-136">Если указано значение true, получателю отправляется [ссылка совместного доступа][].</span><span class="sxs-lookup"><span data-stu-id="176d3-136">If true, a [sharing link][] is sent to the recipient.</span></span> <span data-ttu-id="176d3-137">В противном случае разрешение предоставляется напрямую без отправки уведомления.</span><span class="sxs-lookup"><span data-stu-id="176d3-137">Otherwise, a permission is granted directly without sending a notification.</span></span>
| <span data-ttu-id="176d3-138">roles</span><span class="sxs-lookup"><span data-stu-id="176d3-138">roles</span></span>            | <span data-ttu-id="176d3-139">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="176d3-139">Collection(String)</span></span>             | <span data-ttu-id="176d3-140">Указывает роли, которые необходимо предоставить получателям приглашения к совместному использованию.</span><span class="sxs-lookup"><span data-stu-id="176d3-140">Specify the roles that are to be granted to the recipients of the sharing invitation.</span></span>
| <span data-ttu-id="176d3-141">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="176d3-141">expirationDateTime</span></span> | <span data-ttu-id="176d3-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="176d3-142">DateTimeOffset</span></span>                       | <span data-ttu-id="176d3-143">Укажите значение даты и времени, после которого истечет срок действия разрешения.</span><span class="sxs-lookup"><span data-stu-id="176d3-143">Specify the DateTime after which the permission expires.</span></span> <span data-ttu-id="176d3-144">Доступно в OneDrive для бизнеса, SharePoint и в личных учетных записях OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="176d3-144">Available on OneDrive for Business, SharePoint, and premium personal OneDrive accounts.</span></span>
| <span data-ttu-id="176d3-145">password</span><span class="sxs-lookup"><span data-stu-id="176d3-145">password</span></span>           | <span data-ttu-id="176d3-146">Строка</span><span class="sxs-lookup"><span data-stu-id="176d3-146">String</span></span>                         | <span data-ttu-id="176d3-147">Пароль, установленный в приглашении создателем.</span><span class="sxs-lookup"><span data-stu-id="176d3-147">The password set on the invite by the creator.</span></span> <span data-ttu-id="176d3-148">Только необязательные и OneDrive персональный.</span><span class="sxs-lookup"><span data-stu-id="176d3-148">Optional and OneDrive Personal only.</span></span>

## <a name="example"></a><span data-ttu-id="176d3-149">Пример</span><span class="sxs-lookup"><span data-stu-id="176d3-149">Example</span></span>

<span data-ttu-id="176d3-150">В этом примере показано, как отправить приглашение к совместному использованию пользователю с электронным адресом ryan@contoso.com и добавить сообщение о файле, над которым ведется совместная работа.</span><span class="sxs-lookup"><span data-stu-id="176d3-150">This example sends a sharing invitation to a user with email address "ryan@contoso.com" with a message about a file being collaborated on.</span></span>
<span data-ttu-id="176d3-151">Приглашение предоставляет пользователю Ryan доступ для чтения и записи к файлу.</span><span class="sxs-lookup"><span data-stu-id="176d3-151">The invitation grants Ryan read-write access to the file.</span></span>

### <a name="http-request"></a><span data-ttu-id="176d3-152">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="176d3-152">HTTP request</span></span>

<span data-ttu-id="176d3-153">При успешном выполнении этот метод возвращает код ответа `200 OK` и объект коллекции [permission](../resources/permission.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="176d3-153">If successful, this method returns `200 OK` response code and [permission](../resources/permission.md) collection object in the response body.</span></span>


# <a name="http"></a>[<span data-ttu-id="176d3-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="176d3-154">HTTP</span></span>](#tab/http)
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
  "roles": [ "write" ],
  "password": "password123",
  "expirationDateTime": "2018-07-15T14:00:00.000Z"
}
```
# <a name="c"></a>[<span data-ttu-id="176d3-155">C#</span><span class="sxs-lookup"><span data-stu-id="176d3-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/send-sharing-invite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="176d3-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="176d3-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/send-sharing-invite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="176d3-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="176d3-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/send-sharing-invite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="176d3-158">Java</span><span class="sxs-lookup"><span data-stu-id="176d3-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/send-sharing-invite-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="176d3-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="176d3-159">Response</span></span>

<span data-ttu-id="176d3-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="176d3-160">Here is an example of the response.</span></span>

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
      "hasPassword": true,
      "id": "CCFC7CA3-7A19-4D57-8CEF-149DB9DDFA62",
      "invitation": {
        "email": "ryan@contoso.com",
        "signInRequired": true
      },
      "roles": [ "write" ],
      "expirationDateTime": "2018-07-15T14:00:00.000Z"
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="176d3-161">Примечания</span><span class="sxs-lookup"><span data-stu-id="176d3-161">Remarks</span></span>

* <span data-ttu-id="176d3-162">[Дискам](../resources/drive.md), у которых параметр **driveType** имеет значение `personal` (OneDrive персональный), не удастся создать или изменить разрешения в корневой папке ресурса DriveItem.</span><span class="sxs-lookup"><span data-stu-id="176d3-162">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive personal) cannot create or modify permissions on the root DriveItem.</span></span>
* <span data-ttu-id="176d3-163">Список доступных ролей приведен в разделе [значения свойств Roles](../resources/permission.md#roles-property-values).</span><span class="sxs-lookup"><span data-stu-id="176d3-163">For a list of available roles, see [roles property values](../resources/permission.md#roles-property-values).</span></span>

## <a name="error-responses"></a><span data-ttu-id="176d3-164">Ответы с ошибками</span><span class="sxs-lookup"><span data-stu-id="176d3-164">Error responses</span></span>

<span data-ttu-id="176d3-165">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="176d3-165">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>


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

