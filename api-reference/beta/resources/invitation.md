---
title: Тип ресурса invitation
description: Представляет приглашение, используемое для добавления внешних пользователей в организацию.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3eeeadf3ed27087051c7bf6945920466d60b9469
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2019
ms.locfileid: "39844995"
---
# <a name="invitation-resource-type"></a><span data-ttu-id="a91f7-103">Тип ресурса invitation</span><span class="sxs-lookup"><span data-stu-id="a91f7-103">invitation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a91f7-104">Представляет приглашение, используемое для добавления внешних пользователей в организацию.</span><span class="sxs-lookup"><span data-stu-id="a91f7-104">Represents an invitation that is used to add external users to an organization.</span></span> 

<span data-ttu-id="a91f7-105">Процесс приглашения:</span><span class="sxs-lookup"><span data-stu-id="a91f7-105">The invitation process uses the following flow:</span></span>

* <span data-ttu-id="a91f7-106">Создается приглашение.</span><span class="sxs-lookup"><span data-stu-id="a91f7-106">An invitation is created</span></span>
* <span data-ttu-id="a91f7-107">Приглашение с соответствующей ссылкой отправляется пользователю.</span><span class="sxs-lookup"><span data-stu-id="a91f7-107">An invitation is sent to the invited user (containing an invitation link)</span></span>
* <span data-ttu-id="a91f7-108">Пользователь щелкает эту ссылку, выполняет вход и активирует приглашение. На этом создание объекта user, представляющего приглашенного пользователя, завершается.</span><span class="sxs-lookup"><span data-stu-id="a91f7-108">The invited user clicks on the invitation link, signs in and redeems the invitation and creation of the user entity representing the invited user completes</span></span>
* <span data-ttu-id="a91f7-109">После активации пользователь перенаправляется на определенную страницу.</span><span class="sxs-lookup"><span data-stu-id="a91f7-109">The user is redirected to a specific page after redemption completes</span></span>

<span data-ttu-id="a91f7-p101">При создании приглашения возвращается URL-адрес активации (*inviteRedeemUrl*). API создания приглашений может автоматически отправлять приглашенному пользователю письмо с URL-адресом активации, если параметру *sendInvitationMessage* задано значение true. Вы также можете настроить сообщение, которое будет отправлено приглашенному пользователю. Если вы хотите отправить URL-адрес активации другим способом, задайте параметру *sendInvitationMessage* значение false и используйте URL-адрес активации из отклика для создания собственного сообщения. В настоящее время нет API для выполнения процесса активации. Приглашенный пользователь должен щелкнуть ссылку *inviteRedeemUrl* в сообщении, отправка которого описана выше, и пройти интерактивную процедуру активации в браузере. После этого приглашенный пользователь становится внешним пользователем в организации.</span><span class="sxs-lookup"><span data-stu-id="a91f7-p101">Creating an invitation will return a redemption URL in the response (*inviteRedeemUrl*). The create invitation API can automatically send an email containing the redemption URL to the invited user, by setting the *sendInvitationMessage* to true. You can also customize the message that will be sent to the invited user. Instead, if you wish to send the redemption URL through some other means, you can set the *sendInvitationMessage* to false and use the redeem URL from the response to craft your own communication. Currently, there is no API to perform the redemption process. The invited user has to click on the *inviteRedeemUrl* link sent in the communication in the step above, and go through the interactive redemption process in a browser. Once completed, the invited user becomes an external user in the organization.</span></span>

>[!NOTE]
><span data-ttu-id="a91f7-117">Состояние приглашения отслеживается с помощью свойств **Свойства** и **екстерналусерстатечанжедатетиме** для ресурса внешнего [пользователя](user.md) , созданного в составе запроса приглашения.</span><span class="sxs-lookup"><span data-stu-id="a91f7-117">The invitation status is tracked using the **externalUserState** and the **externalUserStateChangeDateTime** properties on the external [user](user.md) resource created as part of the invitation request.</span></span>

## <a name="methods"></a><span data-ttu-id="a91f7-118">Методы</span><span class="sxs-lookup"><span data-stu-id="a91f7-118">Methods</span></span>
| <span data-ttu-id="a91f7-119">Метод</span><span class="sxs-lookup"><span data-stu-id="a91f7-119">Method</span></span>       | <span data-ttu-id="a91f7-120">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a91f7-120">Return Type</span></span>  |<span data-ttu-id="a91f7-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a91f7-121">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a91f7-122">Создание приглашений</span><span class="sxs-lookup"><span data-stu-id="a91f7-122">Create invitation</span></span>](../api/invitation-post.md) | <span data-ttu-id="a91f7-123">invitation</span><span class="sxs-lookup"><span data-stu-id="a91f7-123">invitation</span></span> | <span data-ttu-id="a91f7-124">Запись свойств и отношений объекта приглашения.</span><span class="sxs-lookup"><span data-stu-id="a91f7-124">Write properties and relationships of invitation object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a91f7-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="a91f7-125">Properties</span></span>
| <span data-ttu-id="a91f7-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="a91f7-126">Property</span></span>     | <span data-ttu-id="a91f7-127">Тип</span><span class="sxs-lookup"><span data-stu-id="a91f7-127">Type</span></span>   |<span data-ttu-id="a91f7-128">Описание</span><span class="sxs-lookup"><span data-stu-id="a91f7-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a91f7-129">invitedUserDisplayName</span><span class="sxs-lookup"><span data-stu-id="a91f7-129">invitedUserDisplayName</span></span>|<span data-ttu-id="a91f7-130">String</span><span class="sxs-lookup"><span data-stu-id="a91f7-130">String</span></span>|<span data-ttu-id="a91f7-131">Отображаемое имя приглашаемого пользователя.</span><span class="sxs-lookup"><span data-stu-id="a91f7-131">The display name of the user being invited.</span></span>|
|<span data-ttu-id="a91f7-132">invitedUserEmailAddress</span><span class="sxs-lookup"><span data-stu-id="a91f7-132">invitedUserEmailAddress</span></span>|<span data-ttu-id="a91f7-133">String</span><span class="sxs-lookup"><span data-stu-id="a91f7-133">String</span></span>|<span data-ttu-id="a91f7-134">Адрес электронной почты приглашаемого пользователя.</span><span class="sxs-lookup"><span data-stu-id="a91f7-134">The email address of the user being invited.</span></span> <span data-ttu-id="a91f7-135">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="a91f7-135">Required.</span></span> <span data-ttu-id="a91f7-136">Следующие специальные символы не разрешены в адресе электронной почты:</span><span class="sxs-lookup"><span data-stu-id="a91f7-136">The following special characters are not permitted in the email address:</span></span><br><ul><li><span data-ttu-id="a91f7-137">Тильда (~)</span><span class="sxs-lookup"><span data-stu-id="a91f7-137">Tilde (~)</span></span></li><li><span data-ttu-id="a91f7-138">Восклицательный знак`!`()</span><span class="sxs-lookup"><span data-stu-id="a91f7-138">Exclamation point (`!`)</span></span></li><li><span data-ttu-id="a91f7-139">Знак (`@`)</span><span class="sxs-lookup"><span data-stu-id="a91f7-139">At sign (`@`)</span></span></li><li><span data-ttu-id="a91f7-140">Знак номера (`#`)</span><span class="sxs-lookup"><span data-stu-id="a91f7-140">Number sign (`#`)</span></span></li><li><span data-ttu-id="a91f7-141">Знак доллара`$`()</span><span class="sxs-lookup"><span data-stu-id="a91f7-141">Dollar sign (`$`)</span></span></li><li><span data-ttu-id="a91f7-142">Процент (`%`)</span><span class="sxs-lookup"><span data-stu-id="a91f7-142">Percent (`%`)</span></span></li><li><span data-ttu-id="a91f7-143">С циркумфлексом`^`()</span><span class="sxs-lookup"><span data-stu-id="a91f7-143">Circumflex (`^`)</span></span></li><li><span data-ttu-id="a91f7-144">амперсанд (`&`);</span><span class="sxs-lookup"><span data-stu-id="a91f7-144">Ampersand (`&`)</span></span></li><li><span data-ttu-id="a91f7-145">Звездочка`*`()</span><span class="sxs-lookup"><span data-stu-id="a91f7-145">Asterisk (`*`)</span></span></li><li><span data-ttu-id="a91f7-146">Круглые скобки`( )`()</span><span class="sxs-lookup"><span data-stu-id="a91f7-146">Parentheses (`( )`)</span></span></li><li><span data-ttu-id="a91f7-147">Дефис (`-`)</span><span class="sxs-lookup"><span data-stu-id="a91f7-147">Hyphen (`-`)</span></span></li><li><span data-ttu-id="a91f7-148">Знак "плюс`+`" ()</span><span class="sxs-lookup"><span data-stu-id="a91f7-148">Plus sign (`+`)</span></span></li><li><span data-ttu-id="a91f7-149">Знак равенства (`=`);</span><span class="sxs-lookup"><span data-stu-id="a91f7-149">Equal sign (`=`)</span></span></li><li><span data-ttu-id="a91f7-150">Квадратные`[ ]`скобки ()</span><span class="sxs-lookup"><span data-stu-id="a91f7-150">Brackets (`[ ]`)</span></span></li><li><span data-ttu-id="a91f7-151">Скобки (`{ }`)</span><span class="sxs-lookup"><span data-stu-id="a91f7-151">Braces (`{ }`)</span></span></li><li><span data-ttu-id="a91f7-152">Обратная`\`косая черта ()</span><span class="sxs-lookup"><span data-stu-id="a91f7-152">Backslash (`\`)</span></span></li><li><span data-ttu-id="a91f7-153">Косая черта (`/`)</span><span class="sxs-lookup"><span data-stu-id="a91f7-153">Slash mark (`/`)</span></span></li><li><span data-ttu-id="a91f7-154">Pipe (`|`)</span><span class="sxs-lookup"><span data-stu-id="a91f7-154">Pipe (`|`)</span></span></li><li><span data-ttu-id="a91f7-155">Точка с`;`запятой ()</span><span class="sxs-lookup"><span data-stu-id="a91f7-155">Semicolon (`;`)</span></span></li><li><span data-ttu-id="a91f7-156">Двоеточие`:`()</span><span class="sxs-lookup"><span data-stu-id="a91f7-156">Colon (`:`)</span></span></li><li><span data-ttu-id="a91f7-157">Кавычки (`"`)</span><span class="sxs-lookup"><span data-stu-id="a91f7-157">Quotation marks (`"`)</span></span></li><li><span data-ttu-id="a91f7-158">Угловые скобки (`< >`)</span><span class="sxs-lookup"><span data-stu-id="a91f7-158">Angle brackets (`< >`)</span></span></li><li><span data-ttu-id="a91f7-159">Вопросительный знак`?`()</span><span class="sxs-lookup"><span data-stu-id="a91f7-159">Question mark (`?`)</span></span></li><li><span data-ttu-id="a91f7-160">Запятая (`,`)</span><span class="sxs-lookup"><span data-stu-id="a91f7-160">Comma (`,`)</span></span></li></ul><br><span data-ttu-id="a91f7-161">Тем не менее применяются следующие исключения:</span><span class="sxs-lookup"><span data-stu-id="a91f7-161">However, the following exceptions apply:</span></span><br><ul><li><span data-ttu-id="a91f7-162">Точка (`.`) или дефис (`-`) может находиться в любом месте имени пользователя, за исключением начала или конца имени.</span><span class="sxs-lookup"><span data-stu-id="a91f7-162">A period (`.`) or a hyphen (`-`) is permitted anywhere in the user name, except at the beginning or end of the name.</span></span></li><li><span data-ttu-id="a91f7-163">Знак подчеркивания (`_`) разрешается в любом месте имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="a91f7-163">An underscore (`_`) is permitted anywhere in the user name.</span></span> <span data-ttu-id="a91f7-164">Это относится к началу или концу имени.</span><span class="sxs-lookup"><span data-stu-id="a91f7-164">This includes at the beginning or end of the name.</span></span></li></ul>|
|<span data-ttu-id="a91f7-165">invitedUserMessageInfo</span><span class="sxs-lookup"><span data-stu-id="a91f7-165">invitedUserMessageInfo</span></span>|[<span data-ttu-id="a91f7-166">invitedUserMessageInfo</span><span class="sxs-lookup"><span data-stu-id="a91f7-166">invitedUserMessageInfo</span></span>](invitedusermessageinfo.md)|<span data-ttu-id="a91f7-167">Дополнительные настройки сообщения, которое отправляется приглашаемому пользователю, в том числе настройка текста, языка и списка получателей копии сообщения.</span><span class="sxs-lookup"><span data-stu-id="a91f7-167">Additional configuration for the message being sent to the invited user, including customizing message text, language and cc recipient list.</span></span>|
|<span data-ttu-id="a91f7-168">sendInvitationMessage</span><span class="sxs-lookup"><span data-stu-id="a91f7-168">sendInvitationMessage</span></span>|<span data-ttu-id="a91f7-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="a91f7-169">Boolean</span></span>|<span data-ttu-id="a91f7-p104">Указывает, следует ли отправлять письмо приглашаемому пользователю. Значение по умолчанию: false.</span><span class="sxs-lookup"><span data-stu-id="a91f7-p104">Indicates whether an email should be sent to the user being invited or not. The default is false.</span></span>|
|<span data-ttu-id="a91f7-172">inviteRedirectUrl</span><span class="sxs-lookup"><span data-stu-id="a91f7-172">inviteRedirectUrl</span></span>|<span data-ttu-id="a91f7-173">String</span><span class="sxs-lookup"><span data-stu-id="a91f7-173">String</span></span>|<span data-ttu-id="a91f7-p105">URL-адрес, на который пользователь перенаправляется после активации приглашения. Указывать обязательно.</span><span class="sxs-lookup"><span data-stu-id="a91f7-p105">The URL user should be redirected to once the invitation is redeemed. Required.</span></span>|
|<span data-ttu-id="a91f7-176">inviteRedeemUrl</span><span class="sxs-lookup"><span data-stu-id="a91f7-176">inviteRedeemUrl</span></span>|<span data-ttu-id="a91f7-177">String</span><span class="sxs-lookup"><span data-stu-id="a91f7-177">String</span></span>|<span data-ttu-id="a91f7-p106">URL-адрес для активации приглашения. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a91f7-p106">The URL user can use to redeem his invitation. Read-Only</span></span>|
|<span data-ttu-id="a91f7-180">invitedUserType</span><span class="sxs-lookup"><span data-stu-id="a91f7-180">invitedUserType</span></span>|<span data-ttu-id="a91f7-181">String</span><span class="sxs-lookup"><span data-stu-id="a91f7-181">String</span></span>|<span data-ttu-id="a91f7-182">Элемент userType, связанный с приглашаемым пользователем.</span><span class="sxs-lookup"><span data-stu-id="a91f7-182">The userType of the user being invited.</span></span> <span data-ttu-id="a91f7-183">Значение по умолчанию: Guest.</span><span class="sxs-lookup"><span data-stu-id="a91f7-183">By default, this is Guest.</span></span> <span data-ttu-id="a91f7-184">Вы можете пригласить как участник, если вы являетесь администратором компании.</span><span class="sxs-lookup"><span data-stu-id="a91f7-184">You can invite as Member if you're are company administrator.</span></span> |
|<span data-ttu-id="a91f7-185">status</span><span class="sxs-lookup"><span data-stu-id="a91f7-185">status</span></span>|<span data-ttu-id="a91f7-186">String</span><span class="sxs-lookup"><span data-stu-id="a91f7-186">String</span></span>|<span data-ttu-id="a91f7-p108">Состояние приглашения. Возможные значения: PendingAcceptance, Completed, InProgress и Error</span><span class="sxs-lookup"><span data-stu-id="a91f7-p108">The status of the invitation. Possible values: PendingAcceptance, Completed, InProgress, and Error</span></span>|

## <a name="relationships"></a><span data-ttu-id="a91f7-189">Связи</span><span class="sxs-lookup"><span data-stu-id="a91f7-189">Relationships</span></span>
| <span data-ttu-id="a91f7-190">Связь</span><span class="sxs-lookup"><span data-stu-id="a91f7-190">Relationship</span></span> | <span data-ttu-id="a91f7-191">Тип</span><span class="sxs-lookup"><span data-stu-id="a91f7-191">Type</span></span>   |<span data-ttu-id="a91f7-192">Описание</span><span class="sxs-lookup"><span data-stu-id="a91f7-192">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a91f7-193">invitedUser</span><span class="sxs-lookup"><span data-stu-id="a91f7-193">invitedUser</span></span>|[<span data-ttu-id="a91f7-194">user</span><span class="sxs-lookup"><span data-stu-id="a91f7-194">user</span></span>](user.md)|<span data-ttu-id="a91f7-p109">Пользователь, создаваемый при создании приглашения. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a91f7-p109">The user created as part of the invitation creation. Read-Only</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a91f7-197">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a91f7-197">JSON representation</span></span>
<span data-ttu-id="a91f7-198">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a91f7-198">Here is a JSON representation of the resource</span></span>

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
