---
title: Диспетчер приглашений
description: 'С помощью диспетчера приглашений можно создать приглашение для добавления внешнего пользователя в организацию. '
localization_priority: Priority
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0a0ee3ba23cb0c323a660b9afd26fa044a50897c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976739"
---
# <a name="invitation-manager"></a><span data-ttu-id="405dd-103">Диспетчер приглашений</span><span class="sxs-lookup"><span data-stu-id="405dd-103">invitation manager</span></span>

<span data-ttu-id="405dd-104">С помощью диспетчера приглашений можно создать приглашение для добавления внешнего пользователя в организацию.</span><span class="sxs-lookup"><span data-stu-id="405dd-104">Use the invitation manager to create an invite, in order to add an external user to the organization.</span></span> 

<span data-ttu-id="405dd-105">Процесс приглашения:</span><span class="sxs-lookup"><span data-stu-id="405dd-105">The invitation process uses the following flow:</span></span>

* <span data-ttu-id="405dd-106">Создается приглашение.</span><span class="sxs-lookup"><span data-stu-id="405dd-106">An invitation is created</span></span>
* <span data-ttu-id="405dd-107">Приглашение с соответствующей ссылкой отправляется пользователю.</span><span class="sxs-lookup"><span data-stu-id="405dd-107">An invitation is sent to the invited user (containing an invitation link)</span></span>
* <span data-ttu-id="405dd-108">Пользователь щелкает эту ссылку, выполняет вход и активирует приглашение. На этом создание объекта user, представляющего приглашенного пользователя, завершается.</span><span class="sxs-lookup"><span data-stu-id="405dd-108">The invited user clicks on the invitation link, signs in and redeems the invitation and creation of the user entity representing the invited user completes</span></span>
* <span data-ttu-id="405dd-109">После активации пользователь перенаправляется на определенную страницу.</span><span class="sxs-lookup"><span data-stu-id="405dd-109">The user is redirected to a specific page after redemption completes</span></span>

<span data-ttu-id="405dd-p101">При создании приглашения возвращается URL-адрес активации (*inviteRedeemUrl*). API создания приглашений может автоматически отправлять приглашенному пользователю письмо с URL-адресом активации, если параметру *sendInvitationMessage* задано значение true. Вы также можете настроить сообщение, которое будет отправлено приглашенному пользователю. Если вы хотите отправить URL-адрес активации другим способом, задайте параметру *sendInvitationMessage* значение false и используйте URL-адрес активации из отклика для создания собственного сообщения. В настоящее время нет API для выполнения процесса активации. Приглашенный пользователь должен щелкнуть ссылку *inviteRedeemUrl* в сообщении, отправка которого описана выше, и пройти интерактивную процедуру активации в браузере. После этого приглашенный пользователь становится внешним пользователем в организации.</span><span class="sxs-lookup"><span data-stu-id="405dd-p101">Creating an invitation will return a redemption URL in the response (*inviteRedeemUrl*). The create invitation API can automatically send an email containing the redemption URL to the invited user, by setting the *sendInvitationMessage* to true. You can also customize the message that will be sent to the invited user. Instead, if you wish to send the redemption URL through some other means, you can set the *sendInvitationMessage* to false and use the redeem URL from the response to craft your own communication. Currently, there is no API to perform the redemption process. The invited user has to click on the *inviteRedeemUrl* link sent in the communication in the step above, and go through the interactive redemption process in a browser. Once completed, the invited user becomes an external user in the organization.</span></span>


## <a name="methods"></a><span data-ttu-id="405dd-117">Методы</span><span class="sxs-lookup"><span data-stu-id="405dd-117">Methods</span></span>
| <span data-ttu-id="405dd-118">Метод</span><span class="sxs-lookup"><span data-stu-id="405dd-118">Method</span></span>       | <span data-ttu-id="405dd-119">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="405dd-119">Return Type</span></span>  |<span data-ttu-id="405dd-120">Описание</span><span class="sxs-lookup"><span data-stu-id="405dd-120">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="405dd-121">Создание приглашений</span><span class="sxs-lookup"><span data-stu-id="405dd-121">Create invitation</span></span>](../api/invitation-post.md) | <span data-ttu-id="405dd-122">invitation</span><span class="sxs-lookup"><span data-stu-id="405dd-122">invitation</span></span> | <span data-ttu-id="405dd-123">Запись свойств и отношений объекта приглашения.</span><span class="sxs-lookup"><span data-stu-id="405dd-123">Write properties and relationships of invitation object.</span></span>|

## <a name="properties"></a><span data-ttu-id="405dd-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="405dd-124">Properties</span></span>
| <span data-ttu-id="405dd-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="405dd-125">Property</span></span>     | <span data-ttu-id="405dd-126">Тип</span><span class="sxs-lookup"><span data-stu-id="405dd-126">Type</span></span>   |<span data-ttu-id="405dd-127">Описание</span><span class="sxs-lookup"><span data-stu-id="405dd-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="405dd-128">invitedUserDisplayName</span><span class="sxs-lookup"><span data-stu-id="405dd-128">invitedUserDisplayName</span></span>|<span data-ttu-id="405dd-129">String</span><span class="sxs-lookup"><span data-stu-id="405dd-129">String</span></span>|<span data-ttu-id="405dd-130">Отображаемое имя приглашаемого пользователя.</span><span class="sxs-lookup"><span data-stu-id="405dd-130">The display name of the user being invited.</span></span>|
|<span data-ttu-id="405dd-131">invitedUserEmailAddress</span><span class="sxs-lookup"><span data-stu-id="405dd-131">invitedUserEmailAddress</span></span>|<span data-ttu-id="405dd-132">String</span><span class="sxs-lookup"><span data-stu-id="405dd-132">String</span></span>|<span data-ttu-id="405dd-p102">Адрес электронной почты приглашаемого пользователя. Указывать обязательно.</span><span class="sxs-lookup"><span data-stu-id="405dd-p102">The email address of the user being invited. Required.</span></span>|
|<span data-ttu-id="405dd-135">invitedUserMessageInfo</span><span class="sxs-lookup"><span data-stu-id="405dd-135">invitedUserMessageInfo</span></span>|[<span data-ttu-id="405dd-136">invitedUserMessageInfo</span><span class="sxs-lookup"><span data-stu-id="405dd-136">invitedUserMessageInfo</span></span>](invitedusermessageinfo.md)|<span data-ttu-id="405dd-137">Дополнительные настройки сообщения, которое отправляется приглашаемому пользователю, в том числе настройка текста, языка и списка получателей копии сообщения.</span><span class="sxs-lookup"><span data-stu-id="405dd-137">Additional configuration for the message being sent to the invited user, including customizing message text, language and cc recipient list.</span></span>|
|<span data-ttu-id="405dd-138">sendInvitationMessage</span><span class="sxs-lookup"><span data-stu-id="405dd-138">sendInvitationMessage</span></span>|<span data-ttu-id="405dd-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="405dd-139">Boolean</span></span>|<span data-ttu-id="405dd-p103">Указывает, следует ли отправлять письмо приглашаемому пользователю. Значение по умолчанию: false.</span><span class="sxs-lookup"><span data-stu-id="405dd-p103">Indicates whether an email should be sent to the user being invited or not. The default is false.</span></span>|
|<span data-ttu-id="405dd-142">inviteRedirectUrl</span><span class="sxs-lookup"><span data-stu-id="405dd-142">inviteRedirectUrl</span></span>|<span data-ttu-id="405dd-143">String</span><span class="sxs-lookup"><span data-stu-id="405dd-143">String</span></span>|<span data-ttu-id="405dd-p104">URL-адрес, на который пользователь перенаправляется после активации приглашения. Указывать обязательно.</span><span class="sxs-lookup"><span data-stu-id="405dd-p104">The URL user should be redirected to once the invitation is redeemed. Required.</span></span>|
|<span data-ttu-id="405dd-146">inviteRedeemUrl</span><span class="sxs-lookup"><span data-stu-id="405dd-146">inviteRedeemUrl</span></span>|<span data-ttu-id="405dd-147">String</span><span class="sxs-lookup"><span data-stu-id="405dd-147">String</span></span>|<span data-ttu-id="405dd-p105">URL-адрес для активации приглашения. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="405dd-p105">The URL user can use to redeem his invitation. Read-Only</span></span>|
|<span data-ttu-id="405dd-150">invitedUserType</span><span class="sxs-lookup"><span data-stu-id="405dd-150">invitedUserType</span></span>|<span data-ttu-id="405dd-151">String</span><span class="sxs-lookup"><span data-stu-id="405dd-151">String</span></span>|<span data-ttu-id="405dd-152">Элемент userType, связанный с приглашаемым пользователем.</span><span class="sxs-lookup"><span data-stu-id="405dd-152">The userType of the user being invited.</span></span> <span data-ttu-id="405dd-153">Значение по умолчанию: Guest.</span><span class="sxs-lookup"><span data-stu-id="405dd-153">By default, this is Guest.</span></span> <span data-ttu-id="405dd-154">Администратор компании может заменить его на Member.</span><span class="sxs-lookup"><span data-stu-id="405dd-154">You can invite as Member if you are a company administrator.</span></span> |
|<span data-ttu-id="405dd-155">status</span><span class="sxs-lookup"><span data-stu-id="405dd-155">status</span></span>|<span data-ttu-id="405dd-156">String</span><span class="sxs-lookup"><span data-stu-id="405dd-156">String</span></span>|<span data-ttu-id="405dd-p107">Состояние приглашения. Возможные значения: PendingAcceptance, Completed, InProgress и Error</span><span class="sxs-lookup"><span data-stu-id="405dd-p107">The status of the invitation. Possible values: PendingAcceptance, Completed, InProgress, and Error</span></span>|

## <a name="relationships"></a><span data-ttu-id="405dd-159">Связи</span><span class="sxs-lookup"><span data-stu-id="405dd-159">Relationships</span></span>
| <span data-ttu-id="405dd-160">Связь</span><span class="sxs-lookup"><span data-stu-id="405dd-160">Relationship</span></span> | <span data-ttu-id="405dd-161">Тип</span><span class="sxs-lookup"><span data-stu-id="405dd-161">Type</span></span>   |<span data-ttu-id="405dd-162">Описание</span><span class="sxs-lookup"><span data-stu-id="405dd-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="405dd-163">invitedUser</span><span class="sxs-lookup"><span data-stu-id="405dd-163">invitedUser</span></span>|[<span data-ttu-id="405dd-164">User</span><span class="sxs-lookup"><span data-stu-id="405dd-164">User</span></span>](user.md)|<span data-ttu-id="405dd-p108">Пользователь, создаваемый при создании приглашения. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="405dd-p108">The user created as part of the invitation creation. Read-Only</span></span>|

## <a name="json-representation"></a><span data-ttu-id="405dd-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="405dd-167">JSON representation</span></span>
<span data-ttu-id="405dd-168">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="405dd-168">Here is a JSON representation of the resource</span></span>

<!-- { "blockType": "resource", "baseType": "microsoft.graph.entity", "@odata.type": "microsoft.graph.invitation" } -->
```json
{
  "invitedUserDisplayName": "string",
  "invitedUserEmailAddress": "string",
  "invitedUserMessageInfo": {"@odata.type": "microsoft.graph.invitedUserMessageInfo"},
  "sendInvitationMessage": false,
  "inviteRedirectUrl": "string",
  "inviteRedeemUrl": "string",
  "status": "string",
  "invitedUser": {"@odata.type": "microsoft.graph.user"},
  "invitedUserType": "string"
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
