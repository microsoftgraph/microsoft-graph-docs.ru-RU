---
title: Создание приглашения
description: Используйте этот API для создания приглашения. Приглашение позволяет добавить внешнего пользователя в организацию.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a39c9d3dc04d4370723f988f7213982a5572507f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350022"
---
# <a name="create-invitation"></a><span data-ttu-id="5a0cb-104">Создание приглашения</span><span class="sxs-lookup"><span data-stu-id="5a0cb-104">Create invitation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a0cb-p102">Используйте этот API для создания [приглашения](../resources/invitation.md). Приглашение позволяет добавить внешнего пользователя в организацию.</span><span class="sxs-lookup"><span data-stu-id="5a0cb-p102">Use this API to create a new [invitation](../resources/invitation.md). Invitation adds an external user to the organization.</span></span>

<span data-ttu-id="5a0cb-107">При создании приглашения у вас есть несколько вариантов:</span><span class="sxs-lookup"><span data-stu-id="5a0cb-107">When creating a new invitation you have several options available:</span></span>

1. <span data-ttu-id="5a0cb-p103">Microsoft Graph может автоматически отправить письмо с приглашением, или ваше приложение может использовать полученное в отклике свойство *inviteRedeemUrl* для отправки специального приглашения выбранным вами способом. Вы можете настроить содержимое и язык письма, отправляемого Microsoft Graph, используя [*invitedUserMessageInfo*](../resources/invitedusermessageinfo.md).</span><span class="sxs-lookup"><span data-stu-id="5a0cb-p103">On invitation creation, Microsoft Graph can automatically send an invitation email directly to the invited user, or your app can use the *inviteRedeemUrl* returned in the creation response to craft your own invitation (through your communication mechanism of choice) to the invited user. If you decide to have Microsoft Graph send an invitation email automatically, you can control the content and language of the email using [*invitedUserMessageInfo*](../resources/invitedusermessageinfo.md).</span></span>
2. <span data-ttu-id="5a0cb-p104">Когда приглашается пользователь, создается объект user (userType задано значение Guest), который требуется для управления доступом к ресурсам. Приглашенный пользователь должен пройти процесс активации, чтобы получить доступ к соответствующим ресурсам.</span><span class="sxs-lookup"><span data-stu-id="5a0cb-p104">When the user is invited, a user entity (of userType Guest) is created and can now be used to control access to resources. The invited user has to go through the redemption process to access any resources he has been invited to.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a0cb-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5a0cb-112">Permissions</span></span>
<span data-ttu-id="5a0cb-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a0cb-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5a0cb-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5a0cb-115">Permission type</span></span>      | <span data-ttu-id="5a0cb-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5a0cb-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5a0cb-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5a0cb-117">Delegated (work or school account)</span></span> | <span data-ttu-id="5a0cb-118">User.Invite.All, User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a0cb-118">User.Invite.All, User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="5a0cb-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5a0cb-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a0cb-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a0cb-120">Not supported.</span></span>    |
|<span data-ttu-id="5a0cb-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5a0cb-121">Application</span></span> | <span data-ttu-id="5a0cb-122">User.Invite.All, User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a0cb-122">User.Invite.All, User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5a0cb-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5a0cb-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /invitations
```
## <a name="request-headers"></a><span data-ttu-id="5a0cb-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5a0cb-124">Request headers</span></span>
| <span data-ttu-id="5a0cb-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5a0cb-125">Header</span></span>       | <span data-ttu-id="5a0cb-126">Значение</span><span class="sxs-lookup"><span data-stu-id="5a0cb-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5a0cb-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5a0cb-127">Authorization</span></span>  | <span data-ttu-id="5a0cb-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5a0cb-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5a0cb-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5a0cb-130">Content-Type</span></span>  | <span data-ttu-id="5a0cb-131">application/json</span><span class="sxs-lookup"><span data-stu-id="5a0cb-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5a0cb-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5a0cb-132">Request body</span></span>
<span data-ttu-id="5a0cb-133">В теле запроса должно быть представление объекта [invitation](../resources/invitation.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5a0cb-133">In the request body, supply a JSON representation of an [invitation](../resources/invitation.md) object.</span></span>

<span data-ttu-id="5a0cb-134">В приведенной ниже таблице показаны свойства, которые обязательно указывать при создании приглашения.</span><span class="sxs-lookup"><span data-stu-id="5a0cb-134">The following table shows the properties that are required when you create a invitation.</span></span>

| <span data-ttu-id="5a0cb-135">Параметр</span><span class="sxs-lookup"><span data-stu-id="5a0cb-135">Parameter</span></span> | <span data-ttu-id="5a0cb-136">Тип</span><span class="sxs-lookup"><span data-stu-id="5a0cb-136">Type</span></span> | <span data-ttu-id="5a0cb-137">Описание</span><span class="sxs-lookup"><span data-stu-id="5a0cb-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5a0cb-138">invitedUserEmailAddress</span><span class="sxs-lookup"><span data-stu-id="5a0cb-138">invitedUserEmailAddress</span></span> |<span data-ttu-id="5a0cb-139">string</span><span class="sxs-lookup"><span data-stu-id="5a0cb-139">string</span></span> | <span data-ttu-id="5a0cb-140">Адрес электронной почты приглашаемого пользователя.</span><span class="sxs-lookup"><span data-stu-id="5a0cb-140">The email address of the user you are inviting.</span></span>|
|<span data-ttu-id="5a0cb-141">inviteRedirectUrl</span><span class="sxs-lookup"><span data-stu-id="5a0cb-141">inviteRedirectUrl</span></span> |<span data-ttu-id="5a0cb-142">string</span><span class="sxs-lookup"><span data-stu-id="5a0cb-142">string</span></span> |<span data-ttu-id="5a0cb-143">URL-адрес, на который пользователь перенаправляется после активации.</span><span class="sxs-lookup"><span data-stu-id="5a0cb-143">The URL that the user will be redirected to after redemption.</span></span>|

## <a name="response"></a><span data-ttu-id="5a0cb-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a0cb-144">Response</span></span>

<span data-ttu-id="5a0cb-145">В случае успеха этот метод возвращает код отклика `201 Created` и объект [invitation](../resources/invitation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5a0cb-145">If successful, this method returns `201 Created` response code and [invitation](../resources/invitation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a0cb-146">Пример</span><span class="sxs-lookup"><span data-stu-id="5a0cb-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5a0cb-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="5a0cb-147">Request</span></span>
<span data-ttu-id="5a0cb-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5a0cb-148">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5a0cb-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="5a0cb-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_invitation_post"
}-->
```http
POST https://graph.microsoft.com/beta/invitations
Content-type: application/json
Content-length: 551

{
  "invitedUserEmailAddress": "yyy@test.com",
  "inviteRedirectUrl": "https://myapp.com"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5a0cb-150">C#</span><span class="sxs-lookup"><span data-stu-id="5a0cb-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-invitation-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5a0cb-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5a0cb-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-invitation-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5a0cb-152">Цель — C</span><span class="sxs-lookup"><span data-stu-id="5a0cb-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-invitation-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5a0cb-153">Java</span><span class="sxs-lookup"><span data-stu-id="5a0cb-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-invitation-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5a0cb-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a0cb-154">Response</span></span>
<span data-ttu-id="5a0cb-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5a0cb-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.invitation"
} -->
```http
HTTP/1.1 201 OK
Content-type: application/json
Content-length: 551

{
  "id": "7b92124c-9fa9-406f-8b8e-225df8376ba9",
  "inviteRedeemUrl": "https://invitations.microsoft.com/redeem/?tenant=04dcc6ab-388a-4559-b527-fbec656300ea&user=7b92124c-9fa9-406f-8b8e-225df8376ba9&ticket=VV9dmiExBsfRIVNFjb9ITj9VXAd07Ypv4gTg%2f8PiuJs%3d&lc=1033&ver=2.0",
  "invitedUserDisplayName": "yyy",
  "invitedUserEmailAddress": "yyy@test.com",
  "sendInvitationMessage": false,
  "invitedUserMessageInfo": {
     "messageLanguage": null,
     "ccRecipients": [
          {
             "emailAddress": {
                 "name": null,
                 "address": null
              }
          }
     ],
     "customizedMessageBody": null
  },
  "inviteRedirectUrl": "https://myapp.com/",
  "status": "Completed",
  "invitedUser":  [ {  "id": "243b1de4-ad9f-421c-a933-d55305fb165d" } ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
