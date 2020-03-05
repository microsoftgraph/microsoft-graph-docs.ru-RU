---
author: JeremyKelley
description: Отправляет приглашение к совместному использованию ресурса DriveItem.
ms.date: 09/10/2017
title: Отправка приглашения на доступ к элементу
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 1b9d704b1375bc0bc3f4239572e3cfd80fb954a4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42432574"
---
# <a name="send-a-sharing-invitation"></a><span data-ttu-id="56ba6-103">Отправка приглашения к совместному использованию</span><span class="sxs-lookup"><span data-stu-id="56ba6-103">Send a sharing invitation</span></span>

<span data-ttu-id="56ba6-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="56ba6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56ba6-p101">Отправляет приглашение к совместному использованию ресурса **DriveItem**. Приглашение к совместному использованию предоставляет получателям разрешения и при необходимости отправляет им на электронную почту уведомления, что к элементу был предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="56ba6-p101">Sends a sharing invitation for a **DriveItem**. A sharing invitation provides permissions to the recipients and optionally sends an email to the recipients to notify them the item was shared.</span></span>

## <a name="permissions"></a><span data-ttu-id="56ba6-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="56ba6-107">Permissions</span></span>

<span data-ttu-id="56ba6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56ba6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56ba6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="56ba6-110">Permission type</span></span>      | <span data-ttu-id="56ba6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="56ba6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56ba6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="56ba6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="56ba6-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56ba6-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="56ba6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="56ba6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56ba6-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56ba6-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="56ba6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="56ba6-116">Application</span></span> | <span data-ttu-id="56ba6-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56ba6-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="56ba6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="56ba6-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
POST /me/drive/items/{item-id}/invite
POST /sites/{siteId}/drive/items/{itemId}/invite
POST /users/{userId}/drive/items/{itemId}/invite
```

## <a name="request-body"></a><span data-ttu-id="56ba6-119">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="56ba6-119">Request body</span></span>

<span data-ttu-id="56ba6-120">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="56ba6-120">In the request body, provide a JSON object with the following parameters.</span></span>

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

| <span data-ttu-id="56ba6-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="56ba6-121">Parameter</span></span>        | <span data-ttu-id="56ba6-122">Тип</span><span class="sxs-lookup"><span data-stu-id="56ba6-122">Type</span></span>                                            | <span data-ttu-id="56ba6-123">Описание</span><span class="sxs-lookup"><span data-stu-id="56ba6-123">Description</span></span>                                                                                                |
|:-----------------|:------------------------------------------------|:-----------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="56ba6-124">recipients</span><span class="sxs-lookup"><span data-stu-id="56ba6-124">recipients</span></span>       | <span data-ttu-id="56ba6-125">Collection([DriveRecipient](../resources/driverecipient.md))</span><span class="sxs-lookup"><span data-stu-id="56ba6-125">Collection([DriveRecipient](../resources/driverecipient.md))</span></span> | <span data-ttu-id="56ba6-126">Коллекция получателей, которые будут получать доступ и приглашение к совместному использованию.</span><span class="sxs-lookup"><span data-stu-id="56ba6-126">A collection of recipients who will receive access and the sharing invitation.</span></span>                                            |
| <span data-ttu-id="56ba6-127">message</span><span class="sxs-lookup"><span data-stu-id="56ba6-127">message</span></span>          | <span data-ttu-id="56ba6-128">String</span><span class="sxs-lookup"><span data-stu-id="56ba6-128">String</span></span>                                          | <span data-ttu-id="56ba6-p103">Сообщение с обычным форматированным текстом, включенное в приглашение на доступ. Максимальная длина составляет 2000 символов.</span><span class="sxs-lookup"><span data-stu-id="56ba6-p103">A plain text formatted message that is included in the sharing invitation. Maximum length 2000 characters.</span></span> |
| <span data-ttu-id="56ba6-131">requireSignIn</span><span class="sxs-lookup"><span data-stu-id="56ba6-131">requireSignIn</span></span>    | <span data-ttu-id="56ba6-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="56ba6-132">Boolean</span></span>                                         | <span data-ttu-id="56ba6-133">Указывает, куда должен зайти получатель приглашения, чтобы просмотреть элемент, к которому предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="56ba6-133">Specifies where the recipient of the invitation is required to sign-in to view the shared item.</span></span>            |
| <span data-ttu-id="56ba6-134">sendInvitation</span><span class="sxs-lookup"><span data-stu-id="56ba6-134">sendInvitation</span></span>   | <span data-ttu-id="56ba6-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="56ba6-135">Boolean</span></span>                                         | <span data-ttu-id="56ba6-136">Указывает, создано ли электронное письмо или запись (false) или разрешение (true).</span><span class="sxs-lookup"><span data-stu-id="56ba6-136">Specifies if an email or post is generated (false) or if the permission is just created (true).</span></span>            |
| <span data-ttu-id="56ba6-137">roles</span><span class="sxs-lookup"><span data-stu-id="56ba6-137">roles</span></span>            | <span data-ttu-id="56ba6-138">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="56ba6-138">Collection(String)</span></span>                              | <span data-ttu-id="56ba6-139">Указывают роли, которые предоставляются получателям приглашения на доступ.</span><span class="sxs-lookup"><span data-stu-id="56ba6-139">Specify the roles that are be granted to the recipients of the sharing invitation.</span></span>                         |
| <span data-ttu-id="56ba6-140">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="56ba6-140">expirationDateTime</span></span> | <span data-ttu-id="56ba6-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56ba6-141">DateTimeOffset</span></span>                       | <span data-ttu-id="56ba6-142">Укажите значение даты и времени, после которого истечет срок действия разрешения.</span><span class="sxs-lookup"><span data-stu-id="56ba6-142">Specify the DateTime after which the permission expires.</span></span> <span data-ttu-id="56ba6-143">Доступно в OneDrive для бизнеса, SharePoint и в личных учетных записях OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="56ba6-143">Available on OneDrive for Business, SharePoint, and premium personal OneDrive accounts.</span></span>
| <span data-ttu-id="56ba6-144">password</span><span class="sxs-lookup"><span data-stu-id="56ba6-144">password</span></span>           | <span data-ttu-id="56ba6-145">Строка</span><span class="sxs-lookup"><span data-stu-id="56ba6-145">String</span></span>                         | <span data-ttu-id="56ba6-146">Пароль, установленный в приглашении создателем.</span><span class="sxs-lookup"><span data-stu-id="56ba6-146">The password set on the invite by the creator.</span></span> <span data-ttu-id="56ba6-147">Только необязательные и OneDrive персональный</span><span class="sxs-lookup"><span data-stu-id="56ba6-147">Optional and OneDrive Personal only</span></span>

## <a name="example"></a><span data-ttu-id="56ba6-148">Пример</span><span class="sxs-lookup"><span data-stu-id="56ba6-148">Example</span></span>

<span data-ttu-id="56ba6-149">В этом примере показано, как отправить приглашение к совместному использованию пользователю с электронным адресом ryan@contoso.org и добавить сообщение о файле, над которым ведется совместная работа.</span><span class="sxs-lookup"><span data-stu-id="56ba6-149">This example sends a sharing invitation to a user with email address "ryan@contoso.org" with a message about a file being collaborated on.</span></span>
<span data-ttu-id="56ba6-150">Приглашение предоставляет пользователю Ryan доступ для чтения и записи к файлу.</span><span class="sxs-lookup"><span data-stu-id="56ba6-150">The invitation grants Ryan read-write access to the file.</span></span>

### <a name="http-request"></a><span data-ttu-id="56ba6-151">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="56ba6-151">HTTP request</span></span>

<span data-ttu-id="56ba6-152">При успешном выполнении этот метод возвращает код ответа `200 OK` и объект коллекции [permission](../resources/permission.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="56ba6-152">If successful, this method returns `200 OK` response code and [permission](../resources/permission.md) collection object in the response body.</span></span>


# <a name="http"></a>[<span data-ttu-id="56ba6-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="56ba6-153">HTTP</span></span>](#tab/http)
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
  "roles": [ "write" ],
  "password": "password123",
  "expirationDateTime": "2018-07-15T14:00:00.000Z"
}
```
# <a name="c"></a>[<span data-ttu-id="56ba6-154">C#</span><span class="sxs-lookup"><span data-stu-id="56ba6-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/send-sharing-invite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="56ba6-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="56ba6-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/send-sharing-invite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="56ba6-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="56ba6-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/send-sharing-invite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="56ba6-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="56ba6-157">Response</span></span>

<span data-ttu-id="56ba6-158">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="56ba6-158">Here is an example of the response.</span></span>

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
### <a name="partial-success-response"></a><span data-ttu-id="56ba6-159">Частичный отклик об успешном выполнении</span><span class="sxs-lookup"><span data-stu-id="56ba6-159">Partial success response</span></span>

<span data-ttu-id="56ba6-160">При приглашении нескольких получателей уведомление может завершиться успешно для некоторых и не для других.</span><span class="sxs-lookup"><span data-stu-id="56ba6-160">When inviting multiple recipients, it's possible for the notification to succeed for some and fail for others.</span></span>
<span data-ttu-id="56ba6-161">В этом случае служба возвращает частичный отклик об успешном выполнении с кодом состояния HTTP 207.</span><span class="sxs-lookup"><span data-stu-id="56ba6-161">In this case, the service returns a partial success response with an HTTP status code of 207.</span></span>
<span data-ttu-id="56ba6-162">Когда возвращается частичный успех, ответ для каждого неудачного получателя будет содержать `error` объект со сведениями о том, что пошло не так, и как исправить его.</span><span class="sxs-lookup"><span data-stu-id="56ba6-162">When partial success is returned, the response for each failed recipient will contain an `error` object with information about what went wrong and how to fix it.</span></span>

<span data-ttu-id="56ba6-163">Ниже приведен пример частичного ответа.</span><span class="sxs-lookup"><span data-stu-id="56ba6-163">Here is an example of the partial response.</span></span>  

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

```json
HTTP/1.1 207 Multi-Status
Content-type: application/json

{
  "value": [
    {
      "grantedTo": {
        "user": {
          "displayName": "John Adams",
          "id": "5D8CA5D0-FFF8-4A97-B0A6-8F5AEA339681"
        }
      },
      "id": "1EFG7CA3-7A19-4D57-8CEF-149DB9DDFA62",
      "invitation": {
        "email": "adams@contoso.com",
        "signInRequired": true
      },
      "roles": [ "write" ],
      "error": {
        "code":"notAllowed",
        "message":"Account verification needed to unblock sending emails.",
        "localizedMessage": "Kontobestätigung erforderlich, um das Senden von E-Mails zu entsperren.",
        "fixItUrl":"http://g.live.com/8SESkydrive/VerifyAccount",
        "innererror":{  
          "code":"accountVerificationRequired" 
        }
      }
    },
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
      "roles": [ "write" ],
      "expirationDateTime": "2018-07-15T14:00:00.000Z"
    }
  ]
}
```
### <a name="sendnotification-errors"></a><span data-ttu-id="56ba6-164">Ошибки Сенднотификатион</span><span class="sxs-lookup"><span data-stu-id="56ba6-164">SendNotification errors</span></span>
<span data-ttu-id="56ba6-165">Ниже приведены некоторые дополнительные ошибки, которые приложение может столкнуть во вложенных `innererror` объектах при сбое отправки уведомления.</span><span class="sxs-lookup"><span data-stu-id="56ba6-165">The following are some additional errors that your app might encounter within the nested `innererror` objects when sending notification fails.</span></span> <span data-ttu-id="56ba6-166">Приложения не обязаны обрабатывать эти приложения.</span><span class="sxs-lookup"><span data-stu-id="56ba6-166">Apps are not required to handle these.</span></span>

| <span data-ttu-id="56ba6-167">Код</span><span class="sxs-lookup"><span data-stu-id="56ba6-167">Code</span></span>                           | <span data-ttu-id="56ba6-168">Описание</span><span class="sxs-lookup"><span data-stu-id="56ba6-168">Description</span></span>
|:-------------------------------|:--------------------------------------------------------------------------------------
| <span data-ttu-id="56ba6-169">аккаунтверификатионрекуиред</span><span class="sxs-lookup"><span data-stu-id="56ba6-169">accountVerificationRequired</span></span>    | <span data-ttu-id="56ba6-170">Для разблокировки уведомлений об отправке требуется проверка учетной записи.</span><span class="sxs-lookup"><span data-stu-id="56ba6-170">Account verification is required to unblock sending notifications.</span></span>
| <span data-ttu-id="56ba6-171">хипчеккрекуиред</span><span class="sxs-lookup"><span data-stu-id="56ba6-171">hipCheckRequired</span></span>               | <span data-ttu-id="56ba6-172">Необходимо выполнить разрешение ГИП (предотвращение проникновения на узел) — разрешить отправку уведомлений об отправке.</span><span class="sxs-lookup"><span data-stu-id="56ba6-172">Need to solve HIP (Host Intrusion Prevention) check to unblock sending notifications.</span></span>
| <span data-ttu-id="56ba6-173">ексчанжеинвалидусер</span><span class="sxs-lookup"><span data-stu-id="56ba6-173">exchangeInvalidUser</span></span>            | <span data-ttu-id="56ba6-174">Не найден почтовый ящик текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="56ba6-174">Current user's mailbox was not found.</span></span>
| <span data-ttu-id="56ba6-175">ексчанжеаутофмаилбокскуота</span><span class="sxs-lookup"><span data-stu-id="56ba6-175">exchangeOutOfMailboxQuota</span></span>      | <span data-ttu-id="56ba6-176">Недостаточно квоты.</span><span class="sxs-lookup"><span data-stu-id="56ba6-176">Out of quota.</span></span>
| <span data-ttu-id="56ba6-177">ексчанжемаксреЦипиентс</span><span class="sxs-lookup"><span data-stu-id="56ba6-177">exchangeMaxRecipients</span></span>          | <span data-ttu-id="56ba6-178">Превышено максимальное количество получателей, которые могут быть отправлены в одно и то же время.</span><span class="sxs-lookup"><span data-stu-id="56ba6-178">Exceeded maximum number of recipients that can be sent notifications at the same time.</span></span>

><span data-ttu-id="56ba6-179">**Примечание:** В любой момент служба может добавить новые коды ошибок или прекратить возврат старых.</span><span class="sxs-lookup"><span data-stu-id="56ba6-179">**Note:** The service can add new error codes or stop returning old ones at any time.</span></span>

## <a name="remarks"></a><span data-ttu-id="56ba6-180">Примечания</span><span class="sxs-lookup"><span data-stu-id="56ba6-180">Remarks</span></span>

* <span data-ttu-id="56ba6-181">[Дискам](../resources/drive.md), у которых параметр **driveType** имеет значение `personal` (OneDrive персональный), не удастся создать или изменить разрешения в корневой папке ресурса DriveItem.</span><span class="sxs-lookup"><span data-stu-id="56ba6-181">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive personal) cannot create or modify permissions on the root DriveItem.</span></span>
* <span data-ttu-id="56ba6-182">Список доступных ролей см. в таблице [Перечисление ролей](../resources/permission.md#roles-enumeration-values).</span><span class="sxs-lookup"><span data-stu-id="56ba6-182">For a list of available roles, see [Roles enumeration](../resources/permission.md#roles-enumeration-values).</span></span>

## <a name="error-responses"></a><span data-ttu-id="56ba6-183">Ответы с ошибками</span><span class="sxs-lookup"><span data-stu-id="56ba6-183">Error responses</span></span>

<span data-ttu-id="56ba6-184">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="56ba6-184">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>


[error-response]: /graph/errors

<!--
{
  "type": "#page.annotation",
  "description": "Add permissions to an item and optionally send a sharing notification.",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Sharing/Add permissions",
  "suppressions": [
  ]
}
-->
