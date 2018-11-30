---
title: Создание приглашения
description: Используйте этот API для создания приглашения. Приглашение позволяет добавить внешнего пользователя в организацию.
ms.openlocfilehash: 220b90cafdd7825dbb6dff9bb8635a51de2ee267
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082120"
---
# <a name="create-invitation"></a><span data-ttu-id="680ee-104">Создание приглашения</span><span class="sxs-lookup"><span data-stu-id="680ee-104">Create invitation</span></span>

> <span data-ttu-id="680ee-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="680ee-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="680ee-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="680ee-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="680ee-p103">Используйте этот API для создания [приглашения](../resources/invitation.md). Приглашение позволяет добавить внешнего пользователя в организацию.</span><span class="sxs-lookup"><span data-stu-id="680ee-p103">Use this API to create a new [invitation](../resources/invitation.md). Invitation adds an external user to the organization.</span></span>

<span data-ttu-id="680ee-109">При создании приглашения у вас есть несколько вариантов:</span><span class="sxs-lookup"><span data-stu-id="680ee-109">When creating a new invitation you have several options available:</span></span>

1. <span data-ttu-id="680ee-p104">Microsoft Graph может автоматически отправить письмо с приглашением, или ваше приложение может использовать полученное в отклике свойство *inviteRedeemUrl* для отправки специального приглашения выбранным вами способом. Вы можете настроить содержимое и язык письма, отправляемого Microsoft Graph, используя [*invitedUserMessageInfo*](../resources/invitedusermessageinfo.md).</span><span class="sxs-lookup"><span data-stu-id="680ee-p104">On invitation creation, Microsoft Graph can automatically send an invitation email directly to the invited user, or your app can use the *inviteRedeemUrl* returned in the creation response to craft your own invitation (through your communication mechanism of choice) to the invited user. If you decide to have Microsoft Graph send an invitation email automatically, you can control the content and language of the email using [*invitedUserMessageInfo*](../resources/invitedusermessageinfo.md).</span></span>
2. <span data-ttu-id="680ee-p105">Когда приглашается пользователь, создается объект user (userType задано значение Guest), который требуется для управления доступом к ресурсам. Приглашенный пользователь должен пройти процесс активации, чтобы получить доступ к соответствующим ресурсам.</span><span class="sxs-lookup"><span data-stu-id="680ee-p105">When the user is invited, a user entity (of userType Guest) is created and can now be used to control access to resources. The invited user has to go through the redemption process to access any resources he has been invited to.</span></span>

## <a name="permissions"></a><span data-ttu-id="680ee-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="680ee-114">Permissions</span></span>
<span data-ttu-id="680ee-p106">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="680ee-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="680ee-117">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="680ee-117">Permission type</span></span>      | <span data-ttu-id="680ee-118">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="680ee-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="680ee-119">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="680ee-119">Delegated (work or school account)</span></span> | <span data-ttu-id="680ee-120">User.Invite.All, User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="680ee-120">User.Invite.All, User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="680ee-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="680ee-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="680ee-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="680ee-122">Not supported.</span></span>    |
|<span data-ttu-id="680ee-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="680ee-123">Application</span></span> | <span data-ttu-id="680ee-124">User.Invite.All, User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="680ee-124">User.Invite.All, User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="680ee-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="680ee-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /invitations
```
## <a name="request-headers"></a><span data-ttu-id="680ee-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="680ee-126">Request headers</span></span>
| <span data-ttu-id="680ee-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="680ee-127">Header</span></span>       | <span data-ttu-id="680ee-128">Значение</span><span class="sxs-lookup"><span data-stu-id="680ee-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="680ee-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="680ee-129">Authorization</span></span>  | <span data-ttu-id="680ee-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="680ee-p107">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="680ee-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="680ee-132">Content-Type</span></span>  | <span data-ttu-id="680ee-133">application/json</span><span class="sxs-lookup"><span data-stu-id="680ee-133">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="680ee-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="680ee-134">Request body</span></span>
<span data-ttu-id="680ee-135">В теле запроса должно быть представление объекта [invitation](../resources/invitation.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="680ee-135">In the request body, supply a JSON representation of an [invitation](../resources/invitation.md) object.</span></span>

<span data-ttu-id="680ee-136">В приведенной ниже таблице показаны свойства, которые обязательно указывать при создании приглашения.</span><span class="sxs-lookup"><span data-stu-id="680ee-136">The following table shows the properties that are required when you create a invitation.</span></span>

| <span data-ttu-id="680ee-137">Параметр</span><span class="sxs-lookup"><span data-stu-id="680ee-137">Parameter</span></span> | <span data-ttu-id="680ee-138">Тип</span><span class="sxs-lookup"><span data-stu-id="680ee-138">Type</span></span> | <span data-ttu-id="680ee-139">Описание</span><span class="sxs-lookup"><span data-stu-id="680ee-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="680ee-140">invitedUserEmailAddress</span><span class="sxs-lookup"><span data-stu-id="680ee-140">invitedUserEmailAddress</span></span> |<span data-ttu-id="680ee-141">string</span><span class="sxs-lookup"><span data-stu-id="680ee-141">string</span></span> | <span data-ttu-id="680ee-142">Адрес электронной почты приглашаемого пользователя.</span><span class="sxs-lookup"><span data-stu-id="680ee-142">The email address of the user you are inviting.</span></span>|
|<span data-ttu-id="680ee-143">inviteRedirectUrl</span><span class="sxs-lookup"><span data-stu-id="680ee-143">inviteRedirectUrl</span></span> |<span data-ttu-id="680ee-144">string</span><span class="sxs-lookup"><span data-stu-id="680ee-144">string</span></span> |<span data-ttu-id="680ee-145">URL-адрес, на который пользователь перенаправляется после активации.</span><span class="sxs-lookup"><span data-stu-id="680ee-145">The URL that the user will be redirected to after redemption.</span></span>|

## <a name="response"></a><span data-ttu-id="680ee-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="680ee-146">Response</span></span>

<span data-ttu-id="680ee-147">В случае успеха этот метод возвращает код отклика `201 Created` и объект [invitation](../resources/invitation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="680ee-147">If successful, this method returns `201 Created` response code and [invitation](../resources/invitation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="680ee-148">Пример</span><span class="sxs-lookup"><span data-stu-id="680ee-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="680ee-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="680ee-149">Request</span></span>
<span data-ttu-id="680ee-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="680ee-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_user_from_users"
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

##### <a name="response"></a><span data-ttu-id="680ee-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="680ee-151">Response</span></span>
<span data-ttu-id="680ee-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="680ee-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.invitations"
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
