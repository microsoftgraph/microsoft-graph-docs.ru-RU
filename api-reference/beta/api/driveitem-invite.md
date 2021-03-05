---
author: JeremyKelley
description: Отправляет приглашение к совместному использованию ресурса DriveItem.
ms.date: 09/10/2017
title: Отправка приглашения для доступа к элементу
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 00252b35b786d467848ed417d9a80dab2b165bc7
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473450"
---
# <a name="send-a-sharing-invitation"></a><span data-ttu-id="a42eb-103">Отправка приглашения к совместному использованию</span><span class="sxs-lookup"><span data-stu-id="a42eb-103">Send a sharing invitation</span></span>

<span data-ttu-id="a42eb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a42eb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a42eb-p101">Отправляет приглашение к совместному использованию ресурса **DriveItem**. Приглашение к совместному использованию предоставляет получателям разрешения и при необходимости отправляет им на электронную почту уведомления, что к элементу был предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="a42eb-p101">Sends a sharing invitation for a **DriveItem**. A sharing invitation provides permissions to the recipients and optionally sends an email to the recipients to notify them the item was shared.</span></span>

## <a name="permissions"></a><span data-ttu-id="a42eb-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a42eb-107">Permissions</span></span>

<span data-ttu-id="a42eb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a42eb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a42eb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a42eb-110">Permission type</span></span>      | <span data-ttu-id="a42eb-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a42eb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a42eb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a42eb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a42eb-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a42eb-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a42eb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a42eb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a42eb-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a42eb-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="a42eb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a42eb-116">Application</span></span> | <span data-ttu-id="a42eb-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a42eb-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a42eb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a42eb-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
POST /me/drive/items/{item-id}/invite
POST /sites/{siteId}/drive/items/{itemId}/invite
POST /users/{userId}/drive/items/{itemId}/invite
```

## <a name="request-body"></a><span data-ttu-id="a42eb-119">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a42eb-119">Request body</span></span>

<span data-ttu-id="a42eb-120">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="a42eb-120">In the request body, provide a JSON object with the following parameters.</span></span>

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

| <span data-ttu-id="a42eb-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="a42eb-121">Parameter</span></span>        | <span data-ttu-id="a42eb-122">Тип</span><span class="sxs-lookup"><span data-stu-id="a42eb-122">Type</span></span>                                            | <span data-ttu-id="a42eb-123">Описание</span><span class="sxs-lookup"><span data-stu-id="a42eb-123">Description</span></span>                                                                                                |
|:-----------------|:------------------------------------------------|:-----------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="a42eb-124">recipients</span><span class="sxs-lookup"><span data-stu-id="a42eb-124">recipients</span></span>       | <span data-ttu-id="a42eb-125">Collection([DriveRecipient](../resources/driverecipient.md))</span><span class="sxs-lookup"><span data-stu-id="a42eb-125">Collection([DriveRecipient](../resources/driverecipient.md))</span></span> | <span data-ttu-id="a42eb-126">Коллекция получателей, которые будут получать доступ и приглашение к совместному использованию.</span><span class="sxs-lookup"><span data-stu-id="a42eb-126">A collection of recipients who will receive access and the sharing invitation.</span></span>                                            |
| <span data-ttu-id="a42eb-127">message</span><span class="sxs-lookup"><span data-stu-id="a42eb-127">message</span></span>          | <span data-ttu-id="a42eb-128">String</span><span class="sxs-lookup"><span data-stu-id="a42eb-128">String</span></span>                                          | <span data-ttu-id="a42eb-p103">Сообщение с обычным форматированным текстом, включенное в приглашение на доступ. Максимальная длина составляет 2000 символов.</span><span class="sxs-lookup"><span data-stu-id="a42eb-p103">A plain text formatted message that is included in the sharing invitation. Maximum length 2000 characters.</span></span> |
| <span data-ttu-id="a42eb-131">requireSignIn</span><span class="sxs-lookup"><span data-stu-id="a42eb-131">requireSignIn</span></span>    | <span data-ttu-id="a42eb-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="a42eb-132">Boolean</span></span>                                         | <span data-ttu-id="a42eb-133">Указывает, куда должен зайти получатель приглашения, чтобы просмотреть элемент, к которому предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="a42eb-133">Specifies where the recipient of the invitation is required to sign-in to view the shared item.</span></span>            |
| <span data-ttu-id="a42eb-134">sendInvitation</span><span class="sxs-lookup"><span data-stu-id="a42eb-134">sendInvitation</span></span>   | <span data-ttu-id="a42eb-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="a42eb-135">Boolean</span></span>                                         | <span data-ttu-id="a42eb-136">Указывает, создано ли электронное письмо или запись (false) или разрешение (true).</span><span class="sxs-lookup"><span data-stu-id="a42eb-136">Specifies if an email or post is generated (false) or if the permission is just created (true).</span></span>            |
| <span data-ttu-id="a42eb-137">roles</span><span class="sxs-lookup"><span data-stu-id="a42eb-137">roles</span></span>            | <span data-ttu-id="a42eb-138">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="a42eb-138">Collection(String)</span></span>                              | <span data-ttu-id="a42eb-139">Указывают роли, которые предоставляются получателям приглашения на доступ.</span><span class="sxs-lookup"><span data-stu-id="a42eb-139">Specify the roles that are be granted to the recipients of the sharing invitation.</span></span>                         |
| <span data-ttu-id="a42eb-140">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a42eb-140">expirationDateTime</span></span> | <span data-ttu-id="a42eb-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a42eb-141">DateTimeOffset</span></span>                       | <span data-ttu-id="a42eb-142">Укажите dateTime, по истечении которого истекает срок действия разрешения.</span><span class="sxs-lookup"><span data-stu-id="a42eb-142">Specify the DateTime after which the permission expires.</span></span> <span data-ttu-id="a42eb-143">Доступно на персональных учетных записях OneDrive для бизнеса, SharePoint и Премиум OneDrive.</span><span class="sxs-lookup"><span data-stu-id="a42eb-143">Available on OneDrive for Business, SharePoint, and premium personal OneDrive accounts.</span></span>
| <span data-ttu-id="a42eb-144">password</span><span class="sxs-lookup"><span data-stu-id="a42eb-144">password</span></span>           | <span data-ttu-id="a42eb-145">Строка</span><span class="sxs-lookup"><span data-stu-id="a42eb-145">String</span></span>                         | <span data-ttu-id="a42eb-146">Пароль, установленный на приглашении создателем.</span><span class="sxs-lookup"><span data-stu-id="a42eb-146">The password set on the invite by the creator.</span></span> <span data-ttu-id="a42eb-147">Необязательный и только OneDrive Personal</span><span class="sxs-lookup"><span data-stu-id="a42eb-147">Optional and OneDrive Personal only</span></span>

## <a name="example"></a><span data-ttu-id="a42eb-148">Пример</span><span class="sxs-lookup"><span data-stu-id="a42eb-148">Example</span></span>

<span data-ttu-id="a42eb-149">В этом примере показано, как отправить приглашение к совместному использованию пользователю с электронным адресом ryan@contoso.org и добавить сообщение о файле, над которым ведется совместная работа.</span><span class="sxs-lookup"><span data-stu-id="a42eb-149">This example sends a sharing invitation to a user with email address "ryan@contoso.org" with a message about a file being collaborated on.</span></span>
<span data-ttu-id="a42eb-150">Приглашение предоставляет пользователю Ryan доступ для чтения и записи к файлу.</span><span class="sxs-lookup"><span data-stu-id="a42eb-150">The invitation grants Ryan read-write access to the file.</span></span>

### <a name="http-request"></a><span data-ttu-id="a42eb-151">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a42eb-151">HTTP request</span></span>

<span data-ttu-id="a42eb-152">При успешном выполнении этот метод возвращает код ответа `200 OK` и объект коллекции [permission](../resources/permission.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a42eb-152">If successful, this method returns `200 OK` response code and [permission](../resources/permission.md) collection object in the response body.</span></span>


# <a name="http"></a>[<span data-ttu-id="a42eb-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="a42eb-153">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a42eb-154">C#</span><span class="sxs-lookup"><span data-stu-id="a42eb-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/send-sharing-invite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a42eb-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a42eb-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/send-sharing-invite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a42eb-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a42eb-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/send-sharing-invite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a42eb-157">Java</span><span class="sxs-lookup"><span data-stu-id="a42eb-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/send-sharing-invite-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a42eb-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="a42eb-158">Response</span></span>

<span data-ttu-id="a42eb-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a42eb-159">Here is an example of the response.</span></span>

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
### <a name="partial-success-response"></a><span data-ttu-id="a42eb-160">Частичный отклик на успех</span><span class="sxs-lookup"><span data-stu-id="a42eb-160">Partial success response</span></span>

<span data-ttu-id="a42eb-161">При приглашении нескольких получателей уведомление может быть успешным для одних и неудалось для других.</span><span class="sxs-lookup"><span data-stu-id="a42eb-161">When inviting multiple recipients, it's possible for the notification to succeed for some and fail for others.</span></span>
<span data-ttu-id="a42eb-162">В этом случае служба возвращает частичный ответ на успех с кодом состояния HTTP 207.</span><span class="sxs-lookup"><span data-stu-id="a42eb-162">In this case, the service returns a partial success response with an HTTP status code of 207.</span></span>
<span data-ttu-id="a42eb-163">Когда возвращается частичный успех, ответ для каждого неудатного получателя будет содержать объект с информацией о том, что пошло не так и `error` как это исправить.</span><span class="sxs-lookup"><span data-stu-id="a42eb-163">When partial success is returned, the response for each failed recipient will contain an `error` object with information about what went wrong and how to fix it.</span></span>

<span data-ttu-id="a42eb-164">Вот пример частичного ответа.</span><span class="sxs-lookup"><span data-stu-id="a42eb-164">Here is an example of the partial response.</span></span>  

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

```http
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
### <a name="sendnotification-errors"></a><span data-ttu-id="a42eb-165">Ошибки SendNotification</span><span class="sxs-lookup"><span data-stu-id="a42eb-165">SendNotification errors</span></span>
<span data-ttu-id="a42eb-166">Ниже приводится ряд дополнительных ошибок, с которыми ваше приложение может столкнуться в вложенных объектах при `innererror` сбойе отправки уведомления.</span><span class="sxs-lookup"><span data-stu-id="a42eb-166">The following are some additional errors that your app might encounter within the nested `innererror` objects when sending notification fails.</span></span> <span data-ttu-id="a42eb-167">Приложения не требуются для обработки этих данных.</span><span class="sxs-lookup"><span data-stu-id="a42eb-167">Apps are not required to handle these.</span></span>

| <span data-ttu-id="a42eb-168">Код</span><span class="sxs-lookup"><span data-stu-id="a42eb-168">Code</span></span>                           | <span data-ttu-id="a42eb-169">Описание</span><span class="sxs-lookup"><span data-stu-id="a42eb-169">Description</span></span>
|:-------------------------------|:--------------------------------------------------------------------------------------
| <span data-ttu-id="a42eb-170">accountVerificationRequired</span><span class="sxs-lookup"><span data-stu-id="a42eb-170">accountVerificationRequired</span></span>    | <span data-ttu-id="a42eb-171">Проверка учетной записи необходима для разблокирования отправки уведомлений.</span><span class="sxs-lookup"><span data-stu-id="a42eb-171">Account verification is required to unblock sending notifications.</span></span>
| <span data-ttu-id="a42eb-172">hipCheckRequired</span><span class="sxs-lookup"><span data-stu-id="a42eb-172">hipCheckRequired</span></span>               | <span data-ttu-id="a42eb-173">Необходимо решить HIP (Host Intrusion Prevention) проверить, чтобы разблокировать отправку уведомлений.</span><span class="sxs-lookup"><span data-stu-id="a42eb-173">Need to solve HIP (Host Intrusion Prevention) check to unblock sending notifications.</span></span>
| <span data-ttu-id="a42eb-174">exchangeInvalidUser</span><span class="sxs-lookup"><span data-stu-id="a42eb-174">exchangeInvalidUser</span></span>            | <span data-ttu-id="a42eb-175">Почтовый ящик текущего пользователя не найден.</span><span class="sxs-lookup"><span data-stu-id="a42eb-175">Current user's mailbox was not found.</span></span>
| <span data-ttu-id="a42eb-176">exchangeOutOfMailboxQuota</span><span class="sxs-lookup"><span data-stu-id="a42eb-176">exchangeOutOfMailboxQuota</span></span>      | <span data-ttu-id="a42eb-177">Вне квоты.</span><span class="sxs-lookup"><span data-stu-id="a42eb-177">Out of quota.</span></span>
| <span data-ttu-id="a42eb-178">ExchangeMaxRecipients</span><span class="sxs-lookup"><span data-stu-id="a42eb-178">exchangeMaxRecipients</span></span>          | <span data-ttu-id="a42eb-179">Превышено максимальное число получателей, которые могут быть отправлены уведомления одновременно.</span><span class="sxs-lookup"><span data-stu-id="a42eb-179">Exceeded maximum number of recipients that can be sent notifications at the same time.</span></span>

><span data-ttu-id="a42eb-180">**Примечание:** Служба может добавлять новые коды ошибок или прекращать возвращать старые в любое время.</span><span class="sxs-lookup"><span data-stu-id="a42eb-180">**Note:** The service can add new error codes or stop returning old ones at any time.</span></span>

## <a name="remarks"></a><span data-ttu-id="a42eb-181">Примечания</span><span class="sxs-lookup"><span data-stu-id="a42eb-181">Remarks</span></span>

* <span data-ttu-id="a42eb-182">[Дискам](../resources/drive.md), у которых параметр **driveType** имеет значение `personal` (OneDrive персональный), не удастся создать или изменить разрешения в корневой папке ресурса DriveItem.</span><span class="sxs-lookup"><span data-stu-id="a42eb-182">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive personal) cannot create or modify permissions on the root DriveItem.</span></span>
* <span data-ttu-id="a42eb-183">Список доступных ролей см. в списке [значений свойств ролей.](../resources/permission.md#roles-property-values)</span><span class="sxs-lookup"><span data-stu-id="a42eb-183">For a list of available roles, see [roles property values](../resources/permission.md#roles-property-values).</span></span>

## <a name="error-responses"></a><span data-ttu-id="a42eb-184">Ответы с ошибками</span><span class="sxs-lookup"><span data-stu-id="a42eb-184">Error responses</span></span>

<span data-ttu-id="a42eb-185">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="a42eb-185">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>


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


