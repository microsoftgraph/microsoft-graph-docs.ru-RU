---
title: Создание приглашения
description: Используйте этот API для создания приглашения. Приглашение позволяет добавить внешнего пользователя в организацию.
localization_priority: Priority
author: elisolMS
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f636ff40878cdf169402625fb9bf437027b35ad6
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292900"
---
# <a name="create-invitation"></a><span data-ttu-id="2d7f6-104">Создание приглашения</span><span class="sxs-lookup"><span data-stu-id="2d7f6-104">Create invitation</span></span>

<span data-ttu-id="2d7f6-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d7f6-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2d7f6-p102">Используйте этот API для создания [приглашения](../resources/invitation.md). Приглашение позволяет добавить внешнего пользователя в организацию.</span><span class="sxs-lookup"><span data-stu-id="2d7f6-p102">Use this API to create a new [invitation](../resources/invitation.md). Invitation adds an external user to the organization.</span></span>

<span data-ttu-id="2d7f6-108">При создании приглашения у вас есть несколько вариантов:</span><span class="sxs-lookup"><span data-stu-id="2d7f6-108">When creating a new invitation you have several options available:</span></span>

1. <span data-ttu-id="2d7f6-p103">Microsoft Graph может автоматически отправить письмо с приглашением, или ваше приложение может использовать полученное в отклике свойство *inviteRedeemUrl* для отправки специального приглашения выбранным вами способом. Вы можете настроить содержимое и язык письма, отправляемого Microsoft Graph, используя [*invitedUserMessageInfo*](../resources/invitedusermessageinfo.md).</span><span class="sxs-lookup"><span data-stu-id="2d7f6-p103">On invitation creation, Microsoft Graph can automatically send an invitation email directly to the invited user, or your app can use the *inviteRedeemUrl* returned in the creation response to craft your own invitation (through your communication mechanism of choice) to the invited user. If you decide to have Microsoft Graph send an invitation email automatically, you can control the content and language of the email using [*invitedUserMessageInfo*](../resources/invitedusermessageinfo.md).</span></span>
2. <span data-ttu-id="2d7f6-p104">Когда приглашается пользователь, создается объект user (userType задано значение Guest), который требуется для управления доступом к ресурсам. Приглашенный пользователь должен пройти процесс активации, чтобы получить доступ к соответствующим ресурсам.</span><span class="sxs-lookup"><span data-stu-id="2d7f6-p104">When the user is invited, a user entity (of userType Guest) is created and can now be used to control access to resources. The invited user has to go through the redemption process to access any resources he has been invited to.</span></span>

## <a name="permissions"></a><span data-ttu-id="2d7f6-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2d7f6-113">Permissions</span></span>
<span data-ttu-id="2d7f6-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d7f6-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2d7f6-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2d7f6-116">Permission type</span></span>      | <span data-ttu-id="2d7f6-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2d7f6-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2d7f6-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2d7f6-118">Delegated (work or school account)</span></span> | <span data-ttu-id="2d7f6-119">User.Invite.All, User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d7f6-119">User.Invite.All, User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="2d7f6-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2d7f6-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d7f6-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d7f6-121">Not supported.</span></span>    |
|<span data-ttu-id="2d7f6-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2d7f6-122">Application</span></span> | <span data-ttu-id="2d7f6-123">User.Invite.All, User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d7f6-123">User.Invite.All, User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2d7f6-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2d7f6-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /invitations
```
## <a name="request-headers"></a><span data-ttu-id="2d7f6-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2d7f6-125">Request headers</span></span>
| <span data-ttu-id="2d7f6-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2d7f6-126">Header</span></span>       | <span data-ttu-id="2d7f6-127">Значение</span><span class="sxs-lookup"><span data-stu-id="2d7f6-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2d7f6-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2d7f6-128">Authorization</span></span>  | <span data-ttu-id="2d7f6-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2d7f6-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2d7f6-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2d7f6-131">Content-Type</span></span>  | <span data-ttu-id="2d7f6-132">application/json</span><span class="sxs-lookup"><span data-stu-id="2d7f6-132">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2d7f6-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2d7f6-133">Request body</span></span>
<span data-ttu-id="2d7f6-134">В теле запроса должно быть представление объекта [invitation](../resources/invitation.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2d7f6-134">In the request body, supply a JSON representation of an [invitation](../resources/invitation.md) object.</span></span>

<span data-ttu-id="2d7f6-135">В приведенной ниже таблице показаны свойства, которые обязательно указывать при создании приглашения.</span><span class="sxs-lookup"><span data-stu-id="2d7f6-135">The following table shows the properties that are required when you create a invitation.</span></span>

| <span data-ttu-id="2d7f6-136">Параметр</span><span class="sxs-lookup"><span data-stu-id="2d7f6-136">Parameter</span></span> | <span data-ttu-id="2d7f6-137">Тип</span><span class="sxs-lookup"><span data-stu-id="2d7f6-137">Type</span></span> | <span data-ttu-id="2d7f6-138">Описание</span><span class="sxs-lookup"><span data-stu-id="2d7f6-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2d7f6-139">invitedUserEmailAddress</span><span class="sxs-lookup"><span data-stu-id="2d7f6-139">invitedUserEmailAddress</span></span> |<span data-ttu-id="2d7f6-140">string</span><span class="sxs-lookup"><span data-stu-id="2d7f6-140">string</span></span> | <span data-ttu-id="2d7f6-141">Адрес электронной почты приглашаемого пользователя.</span><span class="sxs-lookup"><span data-stu-id="2d7f6-141">The email address of the user you are inviting.</span></span>|
|<span data-ttu-id="2d7f6-142">inviteRedirectUrl</span><span class="sxs-lookup"><span data-stu-id="2d7f6-142">inviteRedirectUrl</span></span> |<span data-ttu-id="2d7f6-143">string</span><span class="sxs-lookup"><span data-stu-id="2d7f6-143">string</span></span> |<span data-ttu-id="2d7f6-144">URL-адрес, на который пользователь перенаправляется после активации.</span><span class="sxs-lookup"><span data-stu-id="2d7f6-144">The URL that the user will be redirected to after redemption.</span></span>|

## <a name="response"></a><span data-ttu-id="2d7f6-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d7f6-145">Response</span></span>

<span data-ttu-id="2d7f6-146">В случае успеха этот метод возвращает код отклика `201 Created` и объект [invitation](../resources/invitation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2d7f6-146">If successful, this method returns `201 Created` response code and [invitation](../resources/invitation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d7f6-147">Пример</span><span class="sxs-lookup"><span data-stu-id="2d7f6-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2d7f6-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="2d7f6-148">Request</span></span>
<span data-ttu-id="2d7f6-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2d7f6-149">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2d7f6-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="2d7f6-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_invitation_post"
}-->
```http
POST https://graph.microsoft.com/v1.0/invitations
Content-type: application/json
Content-length: 551

{
  "invitedUserEmailAddress": "yyy@test.com",
  "inviteRedirectUrl": "https://myapp.contoso.com"
}
```
# <a name="c"></a>[<span data-ttu-id="2d7f6-151">C#</span><span class="sxs-lookup"><span data-stu-id="2d7f6-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-invitation-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2d7f6-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2d7f6-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-invitation-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2d7f6-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2d7f6-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-invitation-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2d7f6-154">Java</span><span class="sxs-lookup"><span data-stu-id="2d7f6-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-invitation-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2d7f6-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d7f6-155">Response</span></span>
<span data-ttu-id="2d7f6-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2d7f6-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "inviteRedirectUrl": "https://myapp.contoso.com",
  "status": "Completed",
  "invitedUser": { "id": "243b1de4-ad9f-421c-a933-d55305fb165d" }
}
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [
  ]
}-->

