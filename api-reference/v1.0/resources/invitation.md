# <a name="invitation-manager"></a><span data-ttu-id="f7d9e-101">Диспетчер приглашений</span><span class="sxs-lookup"><span data-stu-id="f7d9e-101">invitation manager</span></span>

<span data-ttu-id="f7d9e-102">С помощью диспетчера приглашений можно создать приглашение для добавления внешнего пользователя в организацию.</span><span class="sxs-lookup"><span data-stu-id="f7d9e-102">Use the invitation manager to create an invite, in order to add an external user to the organization.</span></span> 

<span data-ttu-id="f7d9e-103">Процесс приглашения:</span><span class="sxs-lookup"><span data-stu-id="f7d9e-103">The invitation process uses the following flow:</span></span>

* <span data-ttu-id="f7d9e-104">Создается приглашение.</span><span class="sxs-lookup"><span data-stu-id="f7d9e-104">An invitation is created</span></span>
* <span data-ttu-id="f7d9e-105">Приглашение с соответствующей ссылкой отправляется пользователю.</span><span class="sxs-lookup"><span data-stu-id="f7d9e-105">An invitation is sent to the invited user (containing an invitation link)</span></span>
* <span data-ttu-id="f7d9e-106">Пользователь щелкает эту ссылку, выполняет вход и активирует приглашение. На этом создание объекта user, представляющего приглашенного пользователя, завершается.</span><span class="sxs-lookup"><span data-stu-id="f7d9e-106">The invited user clicks on the invitation link, signs in and redeems the invitation and creation of the user entity representing the invited user completes</span></span>
* <span data-ttu-id="f7d9e-107">После активации пользователь перенаправляется на определенную страницу.</span><span class="sxs-lookup"><span data-stu-id="f7d9e-107">The user is redirected to a specific page after redemption completes</span></span>

<span data-ttu-id="f7d9e-p101">При создании приглашения возвращается URL-адрес активации (*inviteRedeemUrl*). API создания приглашений может автоматически отправлять приглашенному пользователю письмо с URL-адресом активации, если параметру *sendInvitationMessage* задано значение true. Вы также можете настроить сообщение, которое будет отправлено приглашенному пользователю. Если вы хотите отправить URL-адрес активации другим способом, задайте параметру *sendInvitationMessage* значение false и используйте URL-адрес активации из отклика для создания собственного сообщения. В настоящее время нет API для выполнения процесса активации. Приглашенный пользователь должен щелкнуть ссылку *inviteRedeemUrl* в сообщении, отправка которого описана выше, и пройти интерактивную процедуру активации в браузере. После этого приглашенный пользователь становится внешним пользователем в организации.</span><span class="sxs-lookup"><span data-stu-id="f7d9e-p101">Creating an invitation will return a redemption URL in the response (*inviteRedeemUrl*). The create invitation API can automatically send an email containing the redemption URL to the invited user, by setting the *sendInvitationMessage* to true. You can also customize the message that will be sent to the invited user. Instead, if you wish to send the redemption URL through some other means, you can set the *sendInvitationMessage* to false and use the redeem URL from the response to craft your own communication. Currently, there is no API to perform the redemption process. The invited user has to click on the *inviteRedeemUrl* link sent in the communication in the step above, and go through the interactive redemption process in a browser. Once completed, the invited user becomes an external user in the organization.</span></span>


## <a name="methods"></a><span data-ttu-id="f7d9e-115">Методы</span><span class="sxs-lookup"><span data-stu-id="f7d9e-115">Methods</span></span>
| <span data-ttu-id="f7d9e-116">Метод</span><span class="sxs-lookup"><span data-stu-id="f7d9e-116">Method</span></span>       | <span data-ttu-id="f7d9e-117">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f7d9e-117">Return Type</span></span>  |<span data-ttu-id="f7d9e-118">Описание</span><span class="sxs-lookup"><span data-stu-id="f7d9e-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f7d9e-119">Создание приглашений</span><span class="sxs-lookup"><span data-stu-id="f7d9e-119">Create invitation</span></span>](../api/invitation_post.md) | <span data-ttu-id="f7d9e-120">invitation</span><span class="sxs-lookup"><span data-stu-id="f7d9e-120">invitation</span></span> | <span data-ttu-id="f7d9e-121">Запись свойств и отношений объекта приглашения.</span><span class="sxs-lookup"><span data-stu-id="f7d9e-121">Write properties and relationships of invitation object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f7d9e-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="f7d9e-122">Properties</span></span>
| <span data-ttu-id="f7d9e-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="f7d9e-123">Property</span></span>     | <span data-ttu-id="f7d9e-124">Тип</span><span class="sxs-lookup"><span data-stu-id="f7d9e-124">Type</span></span>   |<span data-ttu-id="f7d9e-125">Описание</span><span class="sxs-lookup"><span data-stu-id="f7d9e-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f7d9e-126">invitedUserDisplayName</span><span class="sxs-lookup"><span data-stu-id="f7d9e-126">invitedUserDisplayName</span></span>|<span data-ttu-id="f7d9e-127">String</span><span class="sxs-lookup"><span data-stu-id="f7d9e-127">String</span></span>|<span data-ttu-id="f7d9e-128">Отображаемое имя приглашаемого пользователя.</span><span class="sxs-lookup"><span data-stu-id="f7d9e-128">The display name of the user being invited.</span></span>|
|<span data-ttu-id="f7d9e-129">invitedUserEmailAddress</span><span class="sxs-lookup"><span data-stu-id="f7d9e-129">invitedUserEmailAddress</span></span>|<span data-ttu-id="f7d9e-130">String</span><span class="sxs-lookup"><span data-stu-id="f7d9e-130">String</span></span>|<span data-ttu-id="f7d9e-p102">Адрес электронной почты приглашаемого пользователя. Указывать обязательно.</span><span class="sxs-lookup"><span data-stu-id="f7d9e-p102">The email address of the user being invited. Required.</span></span>|
|<span data-ttu-id="f7d9e-133">invitedUserMessageInfo</span><span class="sxs-lookup"><span data-stu-id="f7d9e-133">invitedUserMessageInfo</span></span>|[<span data-ttu-id="f7d9e-134">invitedUserMessageInfo</span><span class="sxs-lookup"><span data-stu-id="f7d9e-134">invitedUserMessageInfo</span></span>](invitedusermessageinfo.md)|<span data-ttu-id="f7d9e-135">Дополнительные настройки сообщения, которое отправляется приглашаемому пользователю, в том числе настройка текста, языка и списка получателей копии сообщения.</span><span class="sxs-lookup"><span data-stu-id="f7d9e-135">Additional configuration for the message being sent to the invited user, including customizing message text, language and cc recipient list.</span></span>|
|<span data-ttu-id="f7d9e-136">sendInvitationMessage</span><span class="sxs-lookup"><span data-stu-id="f7d9e-136">sendInvitationMessage</span></span>|<span data-ttu-id="f7d9e-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="f7d9e-137">Boolean</span></span>|<span data-ttu-id="f7d9e-p103">Указывает, следует ли отправлять письмо приглашаемому пользователю. Значение по умолчанию: false.</span><span class="sxs-lookup"><span data-stu-id="f7d9e-p103">Indicates whether an email should be sent to the user being invited or not. The default is false.</span></span>|
|<span data-ttu-id="f7d9e-140">inviteRedirectUrl</span><span class="sxs-lookup"><span data-stu-id="f7d9e-140">inviteRedirectUrl</span></span>|<span data-ttu-id="f7d9e-141">String</span><span class="sxs-lookup"><span data-stu-id="f7d9e-141">String</span></span>|<span data-ttu-id="f7d9e-p104">URL-адрес, на который пользователь перенаправляется после активации приглашения. Указывать обязательно.</span><span class="sxs-lookup"><span data-stu-id="f7d9e-p104">The URL user should be redirected to once the invitation is redeemed. Required.</span></span>|
|<span data-ttu-id="f7d9e-144">inviteRedeemUrl</span><span class="sxs-lookup"><span data-stu-id="f7d9e-144">inviteRedeemUrl</span></span>|<span data-ttu-id="f7d9e-145">String</span><span class="sxs-lookup"><span data-stu-id="f7d9e-145">String</span></span>|<span data-ttu-id="f7d9e-p105">URL-адрес для активации приглашения. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f7d9e-p105">The URL user can use to redeem his invitation. Read-Only</span></span>|
|<span data-ttu-id="f7d9e-148">invitedUserType</span><span class="sxs-lookup"><span data-stu-id="f7d9e-148">invitedUserType</span></span>|<span data-ttu-id="f7d9e-149">String</span><span class="sxs-lookup"><span data-stu-id="f7d9e-149">String</span></span>|<span data-ttu-id="f7d9e-150">Элемент userType, связанный с приглашаемым пользователем.</span><span class="sxs-lookup"><span data-stu-id="f7d9e-150">The display name of the user being invited.</span></span> <span data-ttu-id="f7d9e-151">Значение по умолчанию: Guest.</span><span class="sxs-lookup"><span data-stu-id="f7d9e-151">By default, this is Guest.</span></span> <span data-ttu-id="f7d9e-152">Администратор компании может заменить его на Member.</span><span class="sxs-lookup"><span data-stu-id="f7d9e-152">You can invite as Member if you are a company administrator.</span></span> |
|<span data-ttu-id="f7d9e-153">status</span><span class="sxs-lookup"><span data-stu-id="f7d9e-153">status</span></span>|<span data-ttu-id="f7d9e-154">String</span><span class="sxs-lookup"><span data-stu-id="f7d9e-154">String</span></span>|<span data-ttu-id="f7d9e-p107">Состояние приглашения. Возможные значения: PendingAcceptance, Completed, InProgress и Error</span><span class="sxs-lookup"><span data-stu-id="f7d9e-p107">The status of the invitation. Possible values: PendingAcceptance, Completed, InProgress, and Error</span></span>|

## <a name="relationships"></a><span data-ttu-id="f7d9e-157">Связи</span><span class="sxs-lookup"><span data-stu-id="f7d9e-157">Relationships</span></span>
| <span data-ttu-id="f7d9e-158">Связь</span><span class="sxs-lookup"><span data-stu-id="f7d9e-158">Relationship</span></span> | <span data-ttu-id="f7d9e-159">Тип</span><span class="sxs-lookup"><span data-stu-id="f7d9e-159">Type</span></span>   |<span data-ttu-id="f7d9e-160">Описание</span><span class="sxs-lookup"><span data-stu-id="f7d9e-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f7d9e-161">invitedUser</span><span class="sxs-lookup"><span data-stu-id="f7d9e-161">invitedUser</span></span>|[<span data-ttu-id="f7d9e-162">User</span><span class="sxs-lookup"><span data-stu-id="f7d9e-162">User</span></span>](user.md)|<span data-ttu-id="f7d9e-p108">Пользователь, создаваемый при создании приглашения. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f7d9e-p108">The user created as part of the invitation creation. Read-Only</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f7d9e-165">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f7d9e-165">JSON representation</span></span>
<span data-ttu-id="f7d9e-166">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f7d9e-166">Here is a JSON representation of the resource</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.invitations" } -->
```json
{
  "invitedUserDisplayName": "string",
  "invitedUserEmailAddress": "string",
  "invitedUserMessageInfo": {"@odata.type": "microsoft.graph.invitedUserMessageInfo"},
  "sendInvitationMessage": false,
  "inviteRedirectUrl": "string",
  "inviteRedeemUrl": "string",
  "status": "string",

  "invitedUser": [{"@odata.type": "microsoft.graph.user"}]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2016-22-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "invitation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
