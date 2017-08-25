# <a name="create-invitation"></a><span data-ttu-id="bb9b6-101">Создание приглашения</span><span class="sxs-lookup"><span data-stu-id="bb9b6-101">Create invitation</span></span>

<span data-ttu-id="bb9b6-p101">Используйте этот API для создания [приглашения](../resources/invitation.md). Приглашение позволяет добавить внешнего пользователя в организацию.</span><span class="sxs-lookup"><span data-stu-id="bb9b6-p101">Use this API to create a new [invitation](../resources/invitation.md). Invitation adds an external user to the organization.</span></span>

<span data-ttu-id="bb9b6-104">При создании приглашения у вас есть несколько вариантов:</span><span class="sxs-lookup"><span data-stu-id="bb9b6-104">When creating a new invitation you have several options available:</span></span>

1. <span data-ttu-id="bb9b6-p102">Microsoft Graph может автоматически отправить письмо с приглашением, или ваше приложение может использовать полученное в отклике свойство *inviteRedeemUrl* для отправки специального приглашения выбранным вами способом. Вы можете настроить содержимое и язык письма, отправляемого Microsoft Graph, используя [*invitedUserMessageInfo*](../resources/invitedusermessageinfo.md).</span><span class="sxs-lookup"><span data-stu-id="bb9b6-p102">On invitation creation, Microsoft Graph can automatically send an invitation email directly to the invited user, or your app can use the *inviteRedeemUrl* returned in the creation response to craft your own invitation (through your communication mechanism of choice) to the invited user. If you decide to have Microsoft Graph send an invitation email automatically, you can control the content and language of the email using [*invitedUserMessageInfo*](../resources/invitedusermessageinfo.md).</span></span>
2. <span data-ttu-id="bb9b6-p103">Когда приглашается пользователь, создается объект user (userType задано значение Guest), который требуется для управления доступом к ресурсам. Приглашенный пользователь должен пройти процесс активации, чтобы получить доступ к соответствующим ресурсам.</span><span class="sxs-lookup"><span data-stu-id="bb9b6-p103">When the user is invited, a user entity (of userType Guest) is created and can now be used to control access to resources. The invited user has to go through the redemption process to access any resources he has been invited to.</span></span>

## <a name="permissions"></a><span data-ttu-id="bb9b6-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bb9b6-109">Permissions</span></span>
<span data-ttu-id="bb9b6-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bb9b6-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="bb9b6-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bb9b6-112">Permission type</span></span>      | <span data-ttu-id="bb9b6-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bb9b6-113">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="bb9b6-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bb9b6-114">Delegated (work or school account)</span></span> | <span data-ttu-id="bb9b6-115">User.Invite.All, User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb9b6-115">User.Invite.All, User.ReadWrite.All, Directory.ReadWrite.All</span></span>    | 
|<span data-ttu-id="bb9b6-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bb9b6-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb9b6-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb9b6-117">Not supported.</span></span>    | 
|<span data-ttu-id="bb9b6-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bb9b6-118">Application</span></span> | <span data-ttu-id="bb9b6-119">User.Invite.All, User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb9b6-119">User.Invite.All, User.ReadWrite.All, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="bb9b6-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bb9b6-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /invitations
```
## <a name="request-headers"></a><span data-ttu-id="bb9b6-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bb9b6-121">Request headers</span></span>
| <span data-ttu-id="bb9b6-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bb9b6-122">Header</span></span>       | <span data-ttu-id="bb9b6-123">Значение</span><span class="sxs-lookup"><span data-stu-id="bb9b6-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bb9b6-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bb9b6-124">Authorization</span></span>  | <span data-ttu-id="bb9b6-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb9b6-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bb9b6-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bb9b6-127">Content-Type</span></span>  | <span data-ttu-id="bb9b6-128">application/json</span><span class="sxs-lookup"><span data-stu-id="bb9b6-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bb9b6-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bb9b6-129">Request body</span></span>
<span data-ttu-id="bb9b6-130">В теле запроса должно быть представление объекта [invitation](../resources/invitation.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bb9b6-130">In the request body, supply a JSON representation of an [invitation](../resources/invitation.md) object.</span></span>

<span data-ttu-id="bb9b6-131">В приведенной ниже таблице показаны свойства, которые обязательно указывать при создании приглашения.</span><span class="sxs-lookup"><span data-stu-id="bb9b6-131">The following table shows the properties that are required when you create a invitation.</span></span>

| <span data-ttu-id="bb9b6-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="bb9b6-132">Parameter</span></span> | <span data-ttu-id="bb9b6-133">Тип</span><span class="sxs-lookup"><span data-stu-id="bb9b6-133">Type</span></span> | <span data-ttu-id="bb9b6-134">Описание</span><span class="sxs-lookup"><span data-stu-id="bb9b6-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bb9b6-135">invitedUserEmailAddress</span><span class="sxs-lookup"><span data-stu-id="bb9b6-135">invitedUserEmailAddress</span></span> |<span data-ttu-id="bb9b6-136">string</span><span class="sxs-lookup"><span data-stu-id="bb9b6-136">string</span></span> | <span data-ttu-id="bb9b6-137">Адрес электронной почты приглашаемого пользователя.</span><span class="sxs-lookup"><span data-stu-id="bb9b6-137">The email address of the user you are inviting.</span></span>|
|<span data-ttu-id="bb9b6-138">inviteRedirectUrl</span><span class="sxs-lookup"><span data-stu-id="bb9b6-138">inviteRedirectUrl</span></span> |<span data-ttu-id="bb9b6-139">string</span><span class="sxs-lookup"><span data-stu-id="bb9b6-139">string</span></span> |<span data-ttu-id="bb9b6-140">URL-адрес, на который пользователь перенаправляется после активации.</span><span class="sxs-lookup"><span data-stu-id="bb9b6-140">The URL that the user will be redirected to after redemption.</span></span>|

## <a name="response"></a><span data-ttu-id="bb9b6-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb9b6-141">Response</span></span>

<span data-ttu-id="bb9b6-142">В случае успеха этот метод возвращает код отклика `201, Created` и объект [invitation](../resources/invitation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="bb9b6-142">If successful, this method returns `201, Created` response code and [invitation](../resources/invitation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb9b6-143">Пример</span><span class="sxs-lookup"><span data-stu-id="bb9b6-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bb9b6-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="bb9b6-144">Request</span></span>
<span data-ttu-id="bb9b6-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bb9b6-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_user_from_users"
}-->
```http
POST https://graph.microsoft.com/v1.0/invitations
Content-type: application/json
Content-length: 551

{
  "invitedUserEmailAddress": "yyy@test.com",
  "inviteRedirectUrl": "https://myapp.com"
}
```

##### <a name="response"></a><span data-ttu-id="bb9b6-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="bb9b6-146">Response</span></span>
<span data-ttu-id="bb9b6-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="bb9b6-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
