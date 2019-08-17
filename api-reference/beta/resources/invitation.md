---
title: Тип ресурса приглашения
description: Представляет приглашение, используемое для добавления внешних пользователей в организацию.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a6a009640b47ce02b1719d6e5535813d365dc9e6
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450643"
---
# <a name="invitation-resource-type"></a><span data-ttu-id="bf2c0-103">Тип ресурса приглашения</span><span class="sxs-lookup"><span data-stu-id="bf2c0-103">invitation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf2c0-104">Представляет приглашение, используемое для добавления внешних пользователей в организацию.</span><span class="sxs-lookup"><span data-stu-id="bf2c0-104">Represents an invitation that is used to add external users to an organization.</span></span> 

<span data-ttu-id="bf2c0-105">Процесс приглашения:</span><span class="sxs-lookup"><span data-stu-id="bf2c0-105">The invitation process uses the following flow:</span></span>

* <span data-ttu-id="bf2c0-106">Создается приглашение.</span><span class="sxs-lookup"><span data-stu-id="bf2c0-106">An invitation is created</span></span>
* <span data-ttu-id="bf2c0-107">Приглашение с соответствующей ссылкой отправляется пользователю.</span><span class="sxs-lookup"><span data-stu-id="bf2c0-107">An invitation is sent to the invited user (containing an invitation link)</span></span>
* <span data-ttu-id="bf2c0-108">Пользователь щелкает эту ссылку, выполняет вход и активирует приглашение. На этом создание объекта user, представляющего приглашенного пользователя, завершается.</span><span class="sxs-lookup"><span data-stu-id="bf2c0-108">The invited user clicks on the invitation link, signs in and redeems the invitation and creation of the user entity representing the invited user completes</span></span>
* <span data-ttu-id="bf2c0-109">После активации пользователь перенаправляется на определенную страницу.</span><span class="sxs-lookup"><span data-stu-id="bf2c0-109">The user is redirected to a specific page after redemption completes</span></span>

<span data-ttu-id="bf2c0-p101">При создании приглашения возвращается URL-адрес активации (*inviteRedeemUrl*). API создания приглашений может автоматически отправлять приглашенному пользователю письмо с URL-адресом активации, если параметру *sendInvitationMessage* задано значение true. Вы также можете настроить сообщение, которое будет отправлено приглашенному пользователю. Если вы хотите отправить URL-адрес активации другим способом, задайте параметру *sendInvitationMessage* значение false и используйте URL-адрес активации из отклика для создания собственного сообщения. В настоящее время нет API для выполнения процесса активации. Приглашенный пользователь должен щелкнуть ссылку *inviteRedeemUrl* в сообщении, отправка которого описана выше, и пройти интерактивную процедуру активации в браузере. После этого приглашенный пользователь становится внешним пользователем в организации.</span><span class="sxs-lookup"><span data-stu-id="bf2c0-p101">Creating an invitation will return a redemption URL in the response (*inviteRedeemUrl*). The create invitation API can automatically send an email containing the redemption URL to the invited user, by setting the *sendInvitationMessage* to true. You can also customize the message that will be sent to the invited user. Instead, if you wish to send the redemption URL through some other means, you can set the *sendInvitationMessage* to false and use the redeem URL from the response to craft your own communication. Currently, there is no API to perform the redemption process. The invited user has to click on the *inviteRedeemUrl* link sent in the communication in the step above, and go through the interactive redemption process in a browser. Once completed, the invited user becomes an external user in the organization.</span></span>

>[!NOTE]
><span data-ttu-id="bf2c0-117">Состояние приглашения отслеживается с помощью свойств **Свойства** и **екстерналусерстатечанжедатетиме** для ресурса внешнего [пользователя](user.md) , созданного в составе запроса приглашения.</span><span class="sxs-lookup"><span data-stu-id="bf2c0-117">The invitation status is tracked using the **externalUserState** and the **externalUserStateChangeDateTime** properties on the external [user](user.md) resource created as part of the invitation request.</span></span>

## <a name="methods"></a><span data-ttu-id="bf2c0-118">Методы</span><span class="sxs-lookup"><span data-stu-id="bf2c0-118">Methods</span></span>
| <span data-ttu-id="bf2c0-119">Метод</span><span class="sxs-lookup"><span data-stu-id="bf2c0-119">Method</span></span>       | <span data-ttu-id="bf2c0-120">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bf2c0-120">Return Type</span></span>  |<span data-ttu-id="bf2c0-121">Описание</span><span class="sxs-lookup"><span data-stu-id="bf2c0-121">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bf2c0-122">Создание приглашений</span><span class="sxs-lookup"><span data-stu-id="bf2c0-122">Create invitation</span></span>](../api/invitation-post.md) | <span data-ttu-id="bf2c0-123">invitation</span><span class="sxs-lookup"><span data-stu-id="bf2c0-123">invitation</span></span> | <span data-ttu-id="bf2c0-124">Запись свойств и отношений объекта приглашения.</span><span class="sxs-lookup"><span data-stu-id="bf2c0-124">Write properties and relationships of invitation object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bf2c0-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="bf2c0-125">Properties</span></span>
| <span data-ttu-id="bf2c0-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="bf2c0-126">Property</span></span>     | <span data-ttu-id="bf2c0-127">Тип</span><span class="sxs-lookup"><span data-stu-id="bf2c0-127">Type</span></span>   |<span data-ttu-id="bf2c0-128">Описание</span><span class="sxs-lookup"><span data-stu-id="bf2c0-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bf2c0-129">invitedUserDisplayName</span><span class="sxs-lookup"><span data-stu-id="bf2c0-129">invitedUserDisplayName</span></span>|<span data-ttu-id="bf2c0-130">String</span><span class="sxs-lookup"><span data-stu-id="bf2c0-130">String</span></span>|<span data-ttu-id="bf2c0-131">Отображаемое имя приглашаемого пользователя.</span><span class="sxs-lookup"><span data-stu-id="bf2c0-131">The display name of the user being invited.</span></span>|
|<span data-ttu-id="bf2c0-132">invitedUserEmailAddress</span><span class="sxs-lookup"><span data-stu-id="bf2c0-132">invitedUserEmailAddress</span></span>|<span data-ttu-id="bf2c0-133">String</span><span class="sxs-lookup"><span data-stu-id="bf2c0-133">String</span></span>|<span data-ttu-id="bf2c0-p102">Адрес электронной почты приглашаемого пользователя. Указывать обязательно.</span><span class="sxs-lookup"><span data-stu-id="bf2c0-p102">The email address of the user being invited. Required.</span></span>|
|<span data-ttu-id="bf2c0-136">invitedUserMessageInfo</span><span class="sxs-lookup"><span data-stu-id="bf2c0-136">invitedUserMessageInfo</span></span>|[<span data-ttu-id="bf2c0-137">invitedUserMessageInfo</span><span class="sxs-lookup"><span data-stu-id="bf2c0-137">invitedUserMessageInfo</span></span>](invitedusermessageinfo.md)|<span data-ttu-id="bf2c0-138">Дополнительные настройки сообщения, которое отправляется приглашаемому пользователю, в том числе настройка текста, языка и списка получателей копии сообщения.</span><span class="sxs-lookup"><span data-stu-id="bf2c0-138">Additional configuration for the message being sent to the invited user, including customizing message text, language and cc recipient list.</span></span>|
|<span data-ttu-id="bf2c0-139">sendInvitationMessage</span><span class="sxs-lookup"><span data-stu-id="bf2c0-139">sendInvitationMessage</span></span>|<span data-ttu-id="bf2c0-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf2c0-140">Boolean</span></span>|<span data-ttu-id="bf2c0-p103">Указывает, следует ли отправлять письмо приглашаемому пользователю. Значение по умолчанию: false.</span><span class="sxs-lookup"><span data-stu-id="bf2c0-p103">Indicates whether an email should be sent to the user being invited or not. The default is false.</span></span>|
|<span data-ttu-id="bf2c0-143">inviteRedirectUrl</span><span class="sxs-lookup"><span data-stu-id="bf2c0-143">inviteRedirectUrl</span></span>|<span data-ttu-id="bf2c0-144">String</span><span class="sxs-lookup"><span data-stu-id="bf2c0-144">String</span></span>|<span data-ttu-id="bf2c0-p104">URL-адрес, на который пользователь перенаправляется после активации приглашения. Указывать обязательно.</span><span class="sxs-lookup"><span data-stu-id="bf2c0-p104">The URL user should be redirected to once the invitation is redeemed. Required.</span></span>|
|<span data-ttu-id="bf2c0-147">inviteRedeemUrl</span><span class="sxs-lookup"><span data-stu-id="bf2c0-147">inviteRedeemUrl</span></span>|<span data-ttu-id="bf2c0-148">String</span><span class="sxs-lookup"><span data-stu-id="bf2c0-148">String</span></span>|<span data-ttu-id="bf2c0-p105">URL-адрес для активации приглашения. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bf2c0-p105">The URL user can use to redeem his invitation. Read-Only</span></span>|
|<span data-ttu-id="bf2c0-151">invitedUserType</span><span class="sxs-lookup"><span data-stu-id="bf2c0-151">invitedUserType</span></span>|<span data-ttu-id="bf2c0-152">String</span><span class="sxs-lookup"><span data-stu-id="bf2c0-152">String</span></span>|<span data-ttu-id="bf2c0-153">Элемент userType, связанный с приглашаемым пользователем.</span><span class="sxs-lookup"><span data-stu-id="bf2c0-153">The userType of the user being invited.</span></span> <span data-ttu-id="bf2c0-154">Значение по умолчанию: Guest.</span><span class="sxs-lookup"><span data-stu-id="bf2c0-154">By default, this is Guest.</span></span> <span data-ttu-id="bf2c0-155">Вы можете пригласить как участник, если вы являетесь администратором компании.</span><span class="sxs-lookup"><span data-stu-id="bf2c0-155">You can invite as Member if you're are company administrator.</span></span> |
|<span data-ttu-id="bf2c0-156">status</span><span class="sxs-lookup"><span data-stu-id="bf2c0-156">status</span></span>|<span data-ttu-id="bf2c0-157">String</span><span class="sxs-lookup"><span data-stu-id="bf2c0-157">String</span></span>|<span data-ttu-id="bf2c0-p107">Состояние приглашения. Возможные значения: PendingAcceptance, Completed, InProgress и Error</span><span class="sxs-lookup"><span data-stu-id="bf2c0-p107">The status of the invitation. Possible values: PendingAcceptance, Completed, InProgress, and Error</span></span>|

## <a name="relationships"></a><span data-ttu-id="bf2c0-160">Связи</span><span class="sxs-lookup"><span data-stu-id="bf2c0-160">Relationships</span></span>
| <span data-ttu-id="bf2c0-161">Отношение</span><span class="sxs-lookup"><span data-stu-id="bf2c0-161">Relationship</span></span> | <span data-ttu-id="bf2c0-162">Тип</span><span class="sxs-lookup"><span data-stu-id="bf2c0-162">Type</span></span>   |<span data-ttu-id="bf2c0-163">Описание</span><span class="sxs-lookup"><span data-stu-id="bf2c0-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bf2c0-164">invitedUser</span><span class="sxs-lookup"><span data-stu-id="bf2c0-164">invitedUser</span></span>|[<span data-ttu-id="bf2c0-165">user</span><span class="sxs-lookup"><span data-stu-id="bf2c0-165">user</span></span>](user.md)|<span data-ttu-id="bf2c0-p108">Пользователь, создаваемый при создании приглашения. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bf2c0-p108">The user created as part of the invitation creation. Read-Only</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bf2c0-168">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bf2c0-168">JSON representation</span></span>
<span data-ttu-id="bf2c0-169">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bf2c0-169">Here is a JSON representation of the resource</span></span>

<!-- 
{ 
    "blockType": "resource",
    "keyProperty":"id",
    "@odata.type": "microsoft.graph.invitation", 
    "optionalProperties": [
        "invitedUser"
     ],
    "baseType": "microsoft.graph.entity"
} 
-->
```json
{
  "id": "string",
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
<!--
{
  "type": "#page.annotation",
  "description": "invitation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
