---
author: JeremyKelley
ms.date: 09/10/2017
title: Отправка приглашения на доступ к элементу
localization_priority: Normal
ms.prod: sharepoint
description: Отправляет приглашение к совместному доступу для driveItem.
doc_type: apiPageType
ms.openlocfilehash: e514fbd3b8f79d3696f894a6b15ad55055137b70
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50240292"
---
# <a name="send-a-sharing-invitation"></a><span data-ttu-id="2c169-103">Отправка приглашения к совместному использованию</span><span class="sxs-lookup"><span data-stu-id="2c169-103">Send a sharing invitation</span></span>

<span data-ttu-id="2c169-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c169-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2c169-105">Отправляет приглашение к совместному доступу для **driveItem.**</span><span class="sxs-lookup"><span data-stu-id="2c169-105">Sends a sharing invitation for a **driveItem**.</span></span>
<span data-ttu-id="2c169-106">Приглашение к совместному использованию предоставляет получателям разрешения и при необходимости отправляет им сообщение электронной почты с [ссылкой совместного доступа][].</span><span class="sxs-lookup"><span data-stu-id="2c169-106">A sharing invitation provides permissions to the recipients and optionally sends them an email with a [sharing link][].</span></span>

## <a name="permissions"></a><span data-ttu-id="2c169-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2c169-107">Permissions</span></span>

<span data-ttu-id="2c169-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c169-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c169-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2c169-110">Permission type</span></span>      | <span data-ttu-id="2c169-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2c169-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c169-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2c169-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2c169-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c169-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="2c169-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2c169-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c169-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c169-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="2c169-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2c169-116">Application</span></span> | <span data-ttu-id="2c169-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c169-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2c169-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2c169-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
POST /me/drive/items/{item-id}/invite
POST /sites/{siteId}/drive/items/{itemId}/invite
POST /users/{userId}/drive/items/{itemId}/invite
```

## <a name="request-body"></a><span data-ttu-id="2c169-119">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2c169-119">Request body</span></span>

<span data-ttu-id="2c169-120">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="2c169-120">In the request body, provide a JSON object with the following parameters.</span></span>

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

| <span data-ttu-id="2c169-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="2c169-121">Parameter</span></span>        | <span data-ttu-id="2c169-122">Тип</span><span class="sxs-lookup"><span data-stu-id="2c169-122">Type</span></span>                           | <span data-ttu-id="2c169-123">Описание</span><span class="sxs-lookup"><span data-stu-id="2c169-123">Description</span></span>
|:-----------------|:-------------------------------|:-------------------------
| <span data-ttu-id="2c169-124">recipients</span><span class="sxs-lookup"><span data-stu-id="2c169-124">recipients</span></span>       | <span data-ttu-id="2c169-125">Collection([DriveRecipient][])</span><span class="sxs-lookup"><span data-stu-id="2c169-125">Collection([DriveRecipient][])</span></span> | <span data-ttu-id="2c169-126">Коллекция получателей, которые будут получать доступ и приглашение к совместному использованию.</span><span class="sxs-lookup"><span data-stu-id="2c169-126">A collection of recipients who will receive access and the sharing invitation.</span></span>
| <span data-ttu-id="2c169-127">message</span><span class="sxs-lookup"><span data-stu-id="2c169-127">message</span></span>          | <span data-ttu-id="2c169-128">String</span><span class="sxs-lookup"><span data-stu-id="2c169-128">String</span></span>                         | <span data-ttu-id="2c169-p103">Сообщение с обычным форматированным текстом, включенное в приглашение на доступ. Максимальная длина составляет 2000 символов.</span><span class="sxs-lookup"><span data-stu-id="2c169-p103">A plain text formatted message that is included in the sharing invitation. Maximum length 2000 characters.</span></span>
| <span data-ttu-id="2c169-131">requireSignIn</span><span class="sxs-lookup"><span data-stu-id="2c169-131">requireSignIn</span></span>    | <span data-ttu-id="2c169-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c169-132">Boolean</span></span>                        | <span data-ttu-id="2c169-133">Указывает, должен ли получатель приглашения выполнить вход, чтобы просмотреть элемент, к которому предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="2c169-133">Specifies whether the recipient of the invitation is required to sign-in to view the shared item.</span></span>
| <span data-ttu-id="2c169-134">sendInvitation</span><span class="sxs-lookup"><span data-stu-id="2c169-134">sendInvitation</span></span>   | <span data-ttu-id="2c169-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c169-135">Boolean</span></span>                        | <span data-ttu-id="2c169-136">Если указано значение true, получателю отправляется [ссылка совместного доступа][].</span><span class="sxs-lookup"><span data-stu-id="2c169-136">If true, a [sharing link][] is sent to the recipient.</span></span> <span data-ttu-id="2c169-137">В противном случае разрешение предоставляется напрямую без отправки уведомления.</span><span class="sxs-lookup"><span data-stu-id="2c169-137">Otherwise, a permission is granted directly without sending a notification.</span></span>
| <span data-ttu-id="2c169-138">roles</span><span class="sxs-lookup"><span data-stu-id="2c169-138">roles</span></span>            | <span data-ttu-id="2c169-139">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="2c169-139">Collection(String)</span></span>             | <span data-ttu-id="2c169-140">Указывает роли, которые необходимо предоставить получателям приглашения к совместному использованию.</span><span class="sxs-lookup"><span data-stu-id="2c169-140">Specify the roles that are to be granted to the recipients of the sharing invitation.</span></span>
| <span data-ttu-id="2c169-141">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2c169-141">expirationDateTime</span></span> | <span data-ttu-id="2c169-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c169-142">DateTimeOffset</span></span>                       | <span data-ttu-id="2c169-143">Укажите дату и время окончания срока действия разрешения.</span><span class="sxs-lookup"><span data-stu-id="2c169-143">Specify the DateTime after which the permission expires.</span></span> <span data-ttu-id="2c169-144">Доступно в OneDrive для бизнеса, SharePoint и личных учетных записях OneDrive премиум- и премиум-версий.</span><span class="sxs-lookup"><span data-stu-id="2c169-144">Available on OneDrive for Business, SharePoint, and premium personal OneDrive accounts.</span></span>
| <span data-ttu-id="2c169-145">password</span><span class="sxs-lookup"><span data-stu-id="2c169-145">password</span></span>           | <span data-ttu-id="2c169-146">Строка</span><span class="sxs-lookup"><span data-stu-id="2c169-146">String</span></span>                         | <span data-ttu-id="2c169-147">Пароль, установленный в приглашении создателем.</span><span class="sxs-lookup"><span data-stu-id="2c169-147">The password set on the invite by the creator.</span></span> <span data-ttu-id="2c169-148">Необязательный и только OneDrive персональный.</span><span class="sxs-lookup"><span data-stu-id="2c169-148">Optional and OneDrive Personal only.</span></span>

## <a name="example"></a><span data-ttu-id="2c169-149">Пример</span><span class="sxs-lookup"><span data-stu-id="2c169-149">Example</span></span>

<span data-ttu-id="2c169-150">В этом примере показано, как отправить приглашение к совместному использованию пользователю с электронным адресом ryan@contoso.com и добавить сообщение о файле, над которым ведется совместная работа.</span><span class="sxs-lookup"><span data-stu-id="2c169-150">This example sends a sharing invitation to a user with email address "ryan@contoso.com" with a message about a file being collaborated on.</span></span>
<span data-ttu-id="2c169-151">Приглашение предоставляет пользователю Ryan доступ для чтения и записи к файлу.</span><span class="sxs-lookup"><span data-stu-id="2c169-151">The invitation grants Ryan read-write access to the file.</span></span>

### <a name="http-request"></a><span data-ttu-id="2c169-152">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2c169-152">HTTP request</span></span>

<span data-ttu-id="2c169-153">При успешном выполнении этот метод возвращает код ответа `200 OK` и объект коллекции [permission](../resources/permission.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2c169-153">If successful, this method returns `200 OK` response code and [permission](../resources/permission.md) collection object in the response body.</span></span>


# <a name="http"></a>[<span data-ttu-id="2c169-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="2c169-154">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="2c169-155">C#</span><span class="sxs-lookup"><span data-stu-id="2c169-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/send-sharing-invite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2c169-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2c169-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/send-sharing-invite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2c169-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2c169-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/send-sharing-invite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2c169-158">Java</span><span class="sxs-lookup"><span data-stu-id="2c169-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/send-sharing-invite-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2c169-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c169-159">Response</span></span>

<span data-ttu-id="2c169-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2c169-160">Here is an example of the response.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="2c169-161">Примечания</span><span class="sxs-lookup"><span data-stu-id="2c169-161">Remarks</span></span>

* <span data-ttu-id="2c169-162">[Дискам](../resources/drive.md), у которых параметр **driveType** имеет значение `personal` (OneDrive персональный), не удастся создать или изменить разрешения в корневой папке ресурса DriveItem.</span><span class="sxs-lookup"><span data-stu-id="2c169-162">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive personal) cannot create or modify permissions on the root DriveItem.</span></span>
* <span data-ttu-id="2c169-163">Список доступных ролей см. в [значениях свойств ролей.](../resources/permission.md#roles-property-values)</span><span class="sxs-lookup"><span data-stu-id="2c169-163">For a list of available roles, see [roles property values](../resources/permission.md#roles-property-values).</span></span>

## <a name="error-responses"></a><span data-ttu-id="2c169-164">Отклики с ошибками</span><span class="sxs-lookup"><span data-stu-id="2c169-164">Error responses</span></span>

<span data-ttu-id="2c169-165">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="2c169-165">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>


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

