---
title: Диспетчер приглашений
description: 'С помощью диспетчера приглашений можно создать приглашение для добавления внешнего пользователя в организацию. '
ms.openlocfilehash: 3f179df6c11dfc815ffbfc42c39aae5407a66a93
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074607"
---
# <a name="invitation-manager"></a><span data-ttu-id="fc8f5-103">Диспетчер приглашений</span><span class="sxs-lookup"><span data-stu-id="fc8f5-103">invitation manager</span></span>

> <span data-ttu-id="fc8f5-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fc8f5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fc8f5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc8f5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fc8f5-106">С помощью диспетчера приглашений можно создать приглашение для добавления внешнего пользователя в организацию.</span><span class="sxs-lookup"><span data-stu-id="fc8f5-106">Use the invitation manager to create an invite, in order to add an external user to the organization.</span></span> 

<span data-ttu-id="fc8f5-107">Процесс приглашения:</span><span class="sxs-lookup"><span data-stu-id="fc8f5-107">The invitation process uses the following flow:</span></span>

* <span data-ttu-id="fc8f5-108">Создается приглашение.</span><span class="sxs-lookup"><span data-stu-id="fc8f5-108">An invitation is created</span></span>
* <span data-ttu-id="fc8f5-109">Приглашение с соответствующей ссылкой отправляется пользователю.</span><span class="sxs-lookup"><span data-stu-id="fc8f5-109">An invitation is sent to the invited user (containing an invitation link)</span></span>
* <span data-ttu-id="fc8f5-110">Пользователь щелкает эту ссылку, выполняет вход и активирует приглашение. На этом создание объекта user, представляющего приглашенного пользователя, завершается.</span><span class="sxs-lookup"><span data-stu-id="fc8f5-110">The invited user clicks on the invitation link, signs in and redeems the invitation and creation of the user entity representing the invited user completes</span></span>
* <span data-ttu-id="fc8f5-111">После активации пользователь перенаправляется на определенную страницу.</span><span class="sxs-lookup"><span data-stu-id="fc8f5-111">The user is redirected to a specific page after redemption completes</span></span>

<span data-ttu-id="fc8f5-p102">При создании приглашения возвращается URL-адрес активации (*inviteRedeemUrl*). API создания приглашений может автоматически отправлять приглашенному пользователю письмо с URL-адресом активации, если параметру *sendInvitationMessage* задано значение true. Вы также можете настроить сообщение, которое будет отправлено приглашенному пользователю. Если вы хотите отправить URL-адрес активации другим способом, задайте параметру *sendInvitationMessage* значение false и используйте URL-адрес активации из отклика для создания собственного сообщения. В настоящее время нет API для выполнения процесса активации. Приглашенный пользователь должен щелкнуть ссылку *inviteRedeemUrl* в сообщении, отправка которого описана выше, и пройти интерактивную процедуру активации в браузере. После этого приглашенный пользователь становится внешним пользователем в организации.</span><span class="sxs-lookup"><span data-stu-id="fc8f5-p102">Creating an invitation will return a redemption URL in the response (*inviteRedeemUrl*). The create invitation API can automatically send an email containing the redemption URL to the invited user, by setting the *sendInvitationMessage* to true. You can also customize the message that will be sent to the invited user. Instead, if you wish to send the redemption URL through some other means, you can set the *sendInvitationMessage* to false and use the redeem URL from the response to craft your own communication. Currently, there is no API to perform the redemption process. The invited user has to click on the *inviteRedeemUrl* link sent in the communication in the step above, and go through the interactive redemption process in a browser. Once completed, the invited user becomes an external user in the organization.</span></span>


## <a name="methods"></a><span data-ttu-id="fc8f5-119">Методы</span><span class="sxs-lookup"><span data-stu-id="fc8f5-119">Methods</span></span>
| <span data-ttu-id="fc8f5-120">Метод</span><span class="sxs-lookup"><span data-stu-id="fc8f5-120">Method</span></span>       | <span data-ttu-id="fc8f5-121">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fc8f5-121">Return Type</span></span>  |<span data-ttu-id="fc8f5-122">Описание</span><span class="sxs-lookup"><span data-stu-id="fc8f5-122">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fc8f5-123">Создание приглашений</span><span class="sxs-lookup"><span data-stu-id="fc8f5-123">Create invitation</span></span>](../api/invitation-post.md) | <span data-ttu-id="fc8f5-124">invitation</span><span class="sxs-lookup"><span data-stu-id="fc8f5-124">invitation</span></span> | <span data-ttu-id="fc8f5-125">Запись свойств и отношений объекта приглашения.</span><span class="sxs-lookup"><span data-stu-id="fc8f5-125">Write properties and relationships of invitation object.</span></span>|

## <a name="properties"></a><span data-ttu-id="fc8f5-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="fc8f5-126">Properties</span></span>
| <span data-ttu-id="fc8f5-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="fc8f5-127">Property</span></span>     | <span data-ttu-id="fc8f5-128">Тип</span><span class="sxs-lookup"><span data-stu-id="fc8f5-128">Type</span></span>   |<span data-ttu-id="fc8f5-129">Описание</span><span class="sxs-lookup"><span data-stu-id="fc8f5-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fc8f5-130">invitedUserDisplayName</span><span class="sxs-lookup"><span data-stu-id="fc8f5-130">invitedUserDisplayName</span></span>|<span data-ttu-id="fc8f5-131">String</span><span class="sxs-lookup"><span data-stu-id="fc8f5-131">String</span></span>|<span data-ttu-id="fc8f5-132">Отображаемое имя приглашаемого пользователя.</span><span class="sxs-lookup"><span data-stu-id="fc8f5-132">The display name of the user being invited.</span></span>|
|<span data-ttu-id="fc8f5-133">invitedUserEmailAddress</span><span class="sxs-lookup"><span data-stu-id="fc8f5-133">invitedUserEmailAddress</span></span>|<span data-ttu-id="fc8f5-134">String</span><span class="sxs-lookup"><span data-stu-id="fc8f5-134">String</span></span>|<span data-ttu-id="fc8f5-p103">Адрес электронной почты приглашаемого пользователя. Указывать обязательно.</span><span class="sxs-lookup"><span data-stu-id="fc8f5-p103">The email address of the user being invited. Required.</span></span>|
|<span data-ttu-id="fc8f5-137">invitedUserMessageInfo</span><span class="sxs-lookup"><span data-stu-id="fc8f5-137">invitedUserMessageInfo</span></span>|[<span data-ttu-id="fc8f5-138">invitedUserMessageInfo</span><span class="sxs-lookup"><span data-stu-id="fc8f5-138">invitedUserMessageInfo</span></span>](invitedusermessageinfo.md)|<span data-ttu-id="fc8f5-139">Дополнительные настройки сообщения, которое отправляется приглашаемому пользователю, в том числе настройка текста, языка и списка получателей копии сообщения.</span><span class="sxs-lookup"><span data-stu-id="fc8f5-139">Additional configuration for the message being sent to the invited user, including customizing message text, language and cc recipient list.</span></span>|
|<span data-ttu-id="fc8f5-140">sendInvitationMessage</span><span class="sxs-lookup"><span data-stu-id="fc8f5-140">sendInvitationMessage</span></span>|<span data-ttu-id="fc8f5-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc8f5-141">Boolean</span></span>|<span data-ttu-id="fc8f5-p104">Указывает, следует ли отправлять письмо приглашаемому пользователю. Значение по умолчанию: false.</span><span class="sxs-lookup"><span data-stu-id="fc8f5-p104">Indicates whether an email should be sent to the user being invited or not. The default is false.</span></span>|
|<span data-ttu-id="fc8f5-144">inviteRedirectUrl</span><span class="sxs-lookup"><span data-stu-id="fc8f5-144">inviteRedirectUrl</span></span>|<span data-ttu-id="fc8f5-145">String</span><span class="sxs-lookup"><span data-stu-id="fc8f5-145">String</span></span>|<span data-ttu-id="fc8f5-p105">URL-адрес, на который пользователь перенаправляется после активации приглашения. Указывать обязательно.</span><span class="sxs-lookup"><span data-stu-id="fc8f5-p105">The URL user should be redirected to once the invitation is redeemed. Required.</span></span>|
|<span data-ttu-id="fc8f5-148">inviteRedeemUrl</span><span class="sxs-lookup"><span data-stu-id="fc8f5-148">inviteRedeemUrl</span></span>|<span data-ttu-id="fc8f5-149">String</span><span class="sxs-lookup"><span data-stu-id="fc8f5-149">String</span></span>|<span data-ttu-id="fc8f5-p106">URL-адрес для активации приглашения. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fc8f5-p106">The URL user can use to redeem his invitation. Read-Only</span></span>|
|<span data-ttu-id="fc8f5-152">invitedUserType</span><span class="sxs-lookup"><span data-stu-id="fc8f5-152">invitedUserType</span></span>|<span data-ttu-id="fc8f5-153">String</span><span class="sxs-lookup"><span data-stu-id="fc8f5-153">String</span></span>|<span data-ttu-id="fc8f5-p107">Элемент userType, связанный с приглашаемым пользователем. Значение по умолчанию: Guest. Администратор компании может заменить его на Member.</span><span class="sxs-lookup"><span data-stu-id="fc8f5-p107">The userType of the user being invited. By default, this is Guest. You can invite as Member if you're are company administrator.</span></span> |
|<span data-ttu-id="fc8f5-157">status</span><span class="sxs-lookup"><span data-stu-id="fc8f5-157">status</span></span>|<span data-ttu-id="fc8f5-158">String</span><span class="sxs-lookup"><span data-stu-id="fc8f5-158">String</span></span>|<span data-ttu-id="fc8f5-p108">Состояние приглашения. Возможные значения: PendingAcceptance, Completed, InProgress и Error</span><span class="sxs-lookup"><span data-stu-id="fc8f5-p108">The status of the invitation. Possible values: PendingAcceptance, Completed, InProgress, and Error</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc8f5-161">Связи</span><span class="sxs-lookup"><span data-stu-id="fc8f5-161">Relationships</span></span>
| <span data-ttu-id="fc8f5-162">Связь</span><span class="sxs-lookup"><span data-stu-id="fc8f5-162">Relationship</span></span> | <span data-ttu-id="fc8f5-163">Тип</span><span class="sxs-lookup"><span data-stu-id="fc8f5-163">Type</span></span>   |<span data-ttu-id="fc8f5-164">Описание</span><span class="sxs-lookup"><span data-stu-id="fc8f5-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fc8f5-165">invitedUser</span><span class="sxs-lookup"><span data-stu-id="fc8f5-165">invitedUser</span></span>|[<span data-ttu-id="fc8f5-166">User</span><span class="sxs-lookup"><span data-stu-id="fc8f5-166">User</span></span>](user.md)|<span data-ttu-id="fc8f5-p109">Пользователь, создаваемый при создании приглашения. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fc8f5-p109">The user created as part of the invitation creation. Read-Only</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fc8f5-169">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fc8f5-169">JSON representation</span></span>
<span data-ttu-id="fc8f5-170">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fc8f5-170">Here is a JSON representation of the resource</span></span>

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
