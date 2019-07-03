---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Отправка приглашения на доступ к элементу
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 73c26d009e53803d64d957b9cf2ee8e99d749d82
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35436349"
---
# <a name="send-a-sharing-invitation"></a><span data-ttu-id="53b27-102">Отправка приглашения к совместному использованию</span><span class="sxs-lookup"><span data-stu-id="53b27-102">Send a sharing invitation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53b27-p101">Отправляет приглашение к совместному использованию ресурса **DriveItem**. Приглашение к совместному использованию предоставляет получателям разрешения и при необходимости отправляет им на электронную почту уведомления, что к элементу был предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="53b27-p101">Sends a sharing invitation for a **DriveItem**. A sharing invitation provides permissions to the recipients and optionally sends an email to the recipients to notify them the item was shared.</span></span>

## <a name="permissions"></a><span data-ttu-id="53b27-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="53b27-105">Permissions</span></span>

<span data-ttu-id="53b27-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53b27-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53b27-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53b27-108">Permission type</span></span>      | <span data-ttu-id="53b27-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="53b27-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53b27-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53b27-110">Delegated (work or school account)</span></span> | <span data-ttu-id="53b27-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53b27-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="53b27-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53b27-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53b27-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53b27-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="53b27-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="53b27-114">Application</span></span> | <span data-ttu-id="53b27-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53b27-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="53b27-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53b27-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
POST /me/drive/items/{item-id}/invite
POST /sites/{siteId}/drive/items/{itemId}/invite
POST /users/{userId}/drive/items/{itemId}/invite
```

## <a name="request-body"></a><span data-ttu-id="53b27-117">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="53b27-117">Request body</span></span>

<span data-ttu-id="53b27-118">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="53b27-118">In the request body, provide a JSON object with the following parameters.</span></span>

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

| <span data-ttu-id="53b27-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="53b27-119">Parameter</span></span>        | <span data-ttu-id="53b27-120">Тип</span><span class="sxs-lookup"><span data-stu-id="53b27-120">Type</span></span>                                            | <span data-ttu-id="53b27-121">Описание</span><span class="sxs-lookup"><span data-stu-id="53b27-121">Description</span></span>                                                                                                |
|:-----------------|:------------------------------------------------|:-----------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="53b27-122">recipients</span><span class="sxs-lookup"><span data-stu-id="53b27-122">recipients</span></span>       | <span data-ttu-id="53b27-123">Collection([DriveRecipient](../resources/driverecipient.md))</span><span class="sxs-lookup"><span data-stu-id="53b27-123">Collection([DriveRecipient](../resources/driverecipient.md))</span></span> | <span data-ttu-id="53b27-124">Коллекция получателей, которые будут получать доступ и приглашение к совместному использованию.</span><span class="sxs-lookup"><span data-stu-id="53b27-124">A collection of recipients who will receive access and the sharing invitation.</span></span>                                            |
| <span data-ttu-id="53b27-125">message</span><span class="sxs-lookup"><span data-stu-id="53b27-125">message</span></span>          | <span data-ttu-id="53b27-126">String</span><span class="sxs-lookup"><span data-stu-id="53b27-126">String</span></span>                                          | <span data-ttu-id="53b27-p103">Сообщение с обычным форматированным текстом, включенное в приглашение на доступ. Максимальная длина составляет 2000 символов.</span><span class="sxs-lookup"><span data-stu-id="53b27-p103">A plain text formatted message that is included in the sharing invitation. Maximum length 2000 characters.</span></span> |
| <span data-ttu-id="53b27-129">requireSignIn</span><span class="sxs-lookup"><span data-stu-id="53b27-129">requireSignIn</span></span>    | <span data-ttu-id="53b27-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="53b27-130">Boolean</span></span>                                         | <span data-ttu-id="53b27-131">Указывает, куда должен зайти получатель приглашения, чтобы просмотреть элемент, к которому предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="53b27-131">Specifies where the recipient of the invitation is required to sign-in to view the shared item.</span></span>            |
| <span data-ttu-id="53b27-132">sendInvitation</span><span class="sxs-lookup"><span data-stu-id="53b27-132">sendInvitation</span></span>   | <span data-ttu-id="53b27-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="53b27-133">Boolean</span></span>                                         | <span data-ttu-id="53b27-134">Указывает, создано ли электронное письмо или запись (false) или разрешение (true).</span><span class="sxs-lookup"><span data-stu-id="53b27-134">Specifies if an email or post is generated (false) or if the permission is just created (true).</span></span>            |
| <span data-ttu-id="53b27-135">roles</span><span class="sxs-lookup"><span data-stu-id="53b27-135">roles</span></span>            | <span data-ttu-id="53b27-136">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="53b27-136">Collection(String)</span></span>                              | <span data-ttu-id="53b27-137">Указывают роли, которые предоставляются получателям приглашения на доступ.</span><span class="sxs-lookup"><span data-stu-id="53b27-137">Specify the roles that are be granted to the recipients of the sharing invitation.</span></span>                         |
| <span data-ttu-id="53b27-138">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="53b27-138">expirationDateTime</span></span> | <span data-ttu-id="53b27-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53b27-139">DateTimeOffset</span></span>                       | <span data-ttu-id="53b27-140">Укажите значение даты и времени, после которого истечет срок действия разрешения.</span><span class="sxs-lookup"><span data-stu-id="53b27-140">Specify the DateTime after which the permission expires.</span></span> <span data-ttu-id="53b27-141">Доступно в OneDrive для бизнеса, SharePoint и в личных учетных записях OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="53b27-141">Available on OneDrive for Business, SharePoint, and premium personal OneDrive accounts.</span></span>
| <span data-ttu-id="53b27-142">password</span><span class="sxs-lookup"><span data-stu-id="53b27-142">password</span></span>           | <span data-ttu-id="53b27-143">Строка</span><span class="sxs-lookup"><span data-stu-id="53b27-143">String</span></span>                         | <span data-ttu-id="53b27-144">Пароль, установленный в приглашении создателем.</span><span class="sxs-lookup"><span data-stu-id="53b27-144">The password set on the invite by the creator.</span></span> <span data-ttu-id="53b27-145">Только необязательные и OneDrive персональный</span><span class="sxs-lookup"><span data-stu-id="53b27-145">Optional and OneDrive Personal only</span></span>

## <a name="example"></a><span data-ttu-id="53b27-146">Пример</span><span class="sxs-lookup"><span data-stu-id="53b27-146">Example</span></span>

<span data-ttu-id="53b27-147">В этом примере показано, как отправить приглашение к совместному использованию пользователю с электронным адресом ryan@contoso.org и добавить сообщение о файле, над которым ведется совместная работа.</span><span class="sxs-lookup"><span data-stu-id="53b27-147">This example sends a sharing invitation to a user with email address "ryan@contoso.org" with a message about a file being collaborated on.</span></span>
<span data-ttu-id="53b27-148">Приглашение предоставляет пользователю Ryan доступ для чтения и записи к файлу.</span><span class="sxs-lookup"><span data-stu-id="53b27-148">The invitation grants Ryan read-write access to the file.</span></span>

### <a name="http-request"></a><span data-ttu-id="53b27-149">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53b27-149">HTTP request</span></span>

<span data-ttu-id="53b27-150">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект коллекции [permission](../resources/permission.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="53b27-150">If successful, this method returns `200 OK` response code and [permission](../resources/permission.md) collection object in the response body.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="53b27-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="53b27-151">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="53b27-152">C#</span><span class="sxs-lookup"><span data-stu-id="53b27-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/send-sharing-invite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="53b27-153">Javascript</span><span class="sxs-lookup"><span data-stu-id="53b27-153">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/send-sharing-invite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="53b27-154">Цель — C</span><span class="sxs-lookup"><span data-stu-id="53b27-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/send-sharing-invite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="53b27-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="53b27-155">Response</span></span>

<span data-ttu-id="53b27-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="53b27-156">Here is an example of the response.</span></span>

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
### <a name="partial-success-response"></a><span data-ttu-id="53b27-157">Частичный отклик об успешном выполнении</span><span class="sxs-lookup"><span data-stu-id="53b27-157">Partial success response</span></span>

<span data-ttu-id="53b27-158">При приглашении нескольких получателей уведомление может завершиться успешно для некоторых и не для других.</span><span class="sxs-lookup"><span data-stu-id="53b27-158">When inviting multiple recipients, it's possible for the notification to succeed for some and fail for others.</span></span>
<span data-ttu-id="53b27-159">В этом случае служба возвращает частичный отклик об успешном выполнении с кодом состояния HTTP 207.</span><span class="sxs-lookup"><span data-stu-id="53b27-159">In this case, the service returns a partial success response with an HTTP status code of 207.</span></span>
<span data-ttu-id="53b27-160">Когда возвращается частичный успех, ответ для каждого неудачного получателя будет содержать `error` объект со сведениями о том, что пошло не так, и как исправить его.</span><span class="sxs-lookup"><span data-stu-id="53b27-160">When partial success is returned, the response for each failed recipient will contain an `error` object with information about what went wrong and how to fix it.</span></span>

<span data-ttu-id="53b27-161">Ниже приведен пример частичного ответа.</span><span class="sxs-lookup"><span data-stu-id="53b27-161">Here is an example of the partial response.</span></span>  

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
### <a name="sendnotification-errors"></a><span data-ttu-id="53b27-162">Ошибки Сенднотификатион</span><span class="sxs-lookup"><span data-stu-id="53b27-162">SendNotification errors</span></span>
<span data-ttu-id="53b27-163">Ниже приведены некоторые дополнительные ошибки, которые приложение может столкнуть во вложенных `innererror` объектах при сбое отправки уведомления.</span><span class="sxs-lookup"><span data-stu-id="53b27-163">The following are some additional errors that your app might encounter within the nested `innererror` objects when sending notification fails.</span></span> <span data-ttu-id="53b27-164">Приложения не обязаны обрабатывать эти приложения.</span><span class="sxs-lookup"><span data-stu-id="53b27-164">Apps are not required to handle these.</span></span>

| <span data-ttu-id="53b27-165">Код</span><span class="sxs-lookup"><span data-stu-id="53b27-165">Code</span></span>                           | <span data-ttu-id="53b27-166">Описание</span><span class="sxs-lookup"><span data-stu-id="53b27-166">Description</span></span>
|:-------------------------------|:--------------------------------------------------------------------------------------
| <span data-ttu-id="53b27-167">Аккаунтверификатионрекуиред</span><span class="sxs-lookup"><span data-stu-id="53b27-167">accountVerificationRequired</span></span>    | <span data-ttu-id="53b27-168">Для разблокировки уведомлений об отправке требуется проверка учетной записи.</span><span class="sxs-lookup"><span data-stu-id="53b27-168">Account verification is required to unblock sending notifications.</span></span>
| <span data-ttu-id="53b27-169">Хипчеккрекуиред</span><span class="sxs-lookup"><span data-stu-id="53b27-169">hipCheckRequired</span></span>               | <span data-ttu-id="53b27-170">Необходимо выполнить разрешение ГИП (предотвращение проникновения на узел) — разрешить отправку уведомлений об отправке.</span><span class="sxs-lookup"><span data-stu-id="53b27-170">Need to solve HIP (Host Intrusion Prevention) check to unblock sending notifications.</span></span>
| <span data-ttu-id="53b27-171">Ексчанжеинвалидусер</span><span class="sxs-lookup"><span data-stu-id="53b27-171">exchangeInvalidUser</span></span>            | <span data-ttu-id="53b27-172">Не найден почтовый ящик текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="53b27-172">Current user's mailbox was not found.</span></span>
| <span data-ttu-id="53b27-173">Ексчанжеаутофмаилбокскуота</span><span class="sxs-lookup"><span data-stu-id="53b27-173">exchangeOutOfMailboxQuota</span></span>      | <span data-ttu-id="53b27-174">Недостаточно квоты.</span><span class="sxs-lookup"><span data-stu-id="53b27-174">Out of quota.</span></span>
| <span data-ttu-id="53b27-175">ЕксчанжемаксреЦипиентс</span><span class="sxs-lookup"><span data-stu-id="53b27-175">exchangeMaxRecipients</span></span>          | <span data-ttu-id="53b27-176">Превышено максимальное количество получателей, которые могут быть отправлены в одно и то же время.</span><span class="sxs-lookup"><span data-stu-id="53b27-176">Exceeded maximum number of recipients that can be sent notifications at the same time.</span></span>

><span data-ttu-id="53b27-177">**Примечание:** В любой момент служба может добавить новые коды ошибок или прекратить возврат старых.</span><span class="sxs-lookup"><span data-stu-id="53b27-177">**Note:** The service can add new error codes or stop returning old ones at any time.</span></span>

## <a name="remarks"></a><span data-ttu-id="53b27-178">Замечания</span><span class="sxs-lookup"><span data-stu-id="53b27-178">Remarks</span></span>

* <span data-ttu-id="53b27-179">[Дискам](../resources/drive.md), у которых параметр **driveType** имеет значение `personal` (OneDrive персональный), не удастся создать или изменить разрешения в корневой папке ресурса DriveItem.</span><span class="sxs-lookup"><span data-stu-id="53b27-179">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive personal) cannot create or modify permissions on the root DriveItem.</span></span>
* <span data-ttu-id="53b27-180">Список доступных ролей см. в разделе [Перечисление ролей](../resources/permission.md#roles-enumeration-values).</span><span class="sxs-lookup"><span data-stu-id="53b27-180">For a list of available roles, see [Roles enumeration](../resources/permission.md#roles-enumeration-values).</span></span>

## <a name="error-responses"></a><span data-ttu-id="53b27-181">Ответы с ошибками</span><span class="sxs-lookup"><span data-stu-id="53b27-181">Error responses</span></span>

<span data-ttu-id="53b27-182">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="53b27-182">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>


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
