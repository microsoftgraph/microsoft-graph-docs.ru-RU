---
title: Тип ресурса invitation
description: Представляет приглашение, используемое для добавления внешних пользователей в организацию.
localization_priority: Normal
author: elisolMS
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2766206dc5a66529a3d8497ef64d2a9202f270d0
ms.sourcegitcommit: ee41ba9ec6001716f1a9d575741bbeef577e2473
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/09/2020
ms.locfileid: "43199743"
---
# <a name="invitation-resource-type"></a><span data-ttu-id="a9553-103">Тип ресурса invitation</span><span class="sxs-lookup"><span data-stu-id="a9553-103">invitation resource type</span></span>

<span data-ttu-id="a9553-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9553-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9553-105">Представляет приглашение, используемое для добавления внешних пользователей в организацию.</span><span class="sxs-lookup"><span data-stu-id="a9553-105">Represents an invitation that is used to add external users to an organization.</span></span> 

<span data-ttu-id="a9553-106">Процесс приглашения:</span><span class="sxs-lookup"><span data-stu-id="a9553-106">The invitation process uses the following flow:</span></span>

* <span data-ttu-id="a9553-107">Создается приглашение.</span><span class="sxs-lookup"><span data-stu-id="a9553-107">An invitation is created</span></span>
* <span data-ttu-id="a9553-108">Приглашение с соответствующей ссылкой отправляется пользователю.</span><span class="sxs-lookup"><span data-stu-id="a9553-108">An invitation is sent to the invited user (containing an invitation link)</span></span>
* <span data-ttu-id="a9553-109">Пользователь щелкает эту ссылку, выполняет вход и активирует приглашение. На этом создание объекта user, представляющего приглашенного пользователя, завершается.</span><span class="sxs-lookup"><span data-stu-id="a9553-109">The invited user clicks on the invitation link, signs in and redeems the invitation and creation of the user entity representing the invited user completes</span></span>
* <span data-ttu-id="a9553-110">После активации пользователь перенаправляется на определенную страницу.</span><span class="sxs-lookup"><span data-stu-id="a9553-110">The user is redirected to a specific page after redemption completes</span></span>

<span data-ttu-id="a9553-p101">При создании приглашения возвращается URL-адрес активации (*inviteRedeemUrl*). API создания приглашений может автоматически отправлять приглашенному пользователю письмо с URL-адресом активации, если параметру *sendInvitationMessage* задано значение true. Вы также можете настроить сообщение, которое будет отправлено приглашенному пользователю. Если вы хотите отправить URL-адрес активации другим способом, задайте параметру *sendInvitationMessage* значение false и используйте URL-адрес активации из отклика для создания собственного сообщения. В настоящее время нет API для выполнения процесса активации. Приглашенный пользователь должен щелкнуть ссылку *inviteRedeemUrl* в сообщении, отправка которого описана выше, и пройти интерактивную процедуру активации в браузере. После этого приглашенный пользователь становится внешним пользователем в организации.</span><span class="sxs-lookup"><span data-stu-id="a9553-p101">Creating an invitation will return a redemption URL in the response (*inviteRedeemUrl*). The create invitation API can automatically send an email containing the redemption URL to the invited user, by setting the *sendInvitationMessage* to true. You can also customize the message that will be sent to the invited user. Instead, if you wish to send the redemption URL through some other means, you can set the *sendInvitationMessage* to false and use the redeem URL from the response to craft your own communication. Currently, there is no API to perform the redemption process. The invited user has to click on the *inviteRedeemUrl* link sent in the communication in the step above, and go through the interactive redemption process in a browser. Once completed, the invited user becomes an external user in the organization.</span></span>

>[!NOTE]
><span data-ttu-id="a9553-118">Состояние приглашения отслеживается с помощью свойств **Свойства** и **екстерналусерстатечанжедатетиме** для ресурса внешнего [пользователя](user.md) , созданного в составе запроса приглашения.</span><span class="sxs-lookup"><span data-stu-id="a9553-118">The invitation status is tracked using the **externalUserState** and the **externalUserStateChangeDateTime** properties on the external [user](user.md) resource created as part of the invitation request.</span></span>

## <a name="methods"></a><span data-ttu-id="a9553-119">Методы</span><span class="sxs-lookup"><span data-stu-id="a9553-119">Methods</span></span>
| <span data-ttu-id="a9553-120">Метод</span><span class="sxs-lookup"><span data-stu-id="a9553-120">Method</span></span>       | <span data-ttu-id="a9553-121">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a9553-121">Return Type</span></span>  |<span data-ttu-id="a9553-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a9553-122">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a9553-123">Создание приглашений</span><span class="sxs-lookup"><span data-stu-id="a9553-123">Create invitation</span></span>](../api/invitation-post.md) | <span data-ttu-id="a9553-124">invitation</span><span class="sxs-lookup"><span data-stu-id="a9553-124">invitation</span></span> | <span data-ttu-id="a9553-125">Запись свойств и отношений объекта приглашения.</span><span class="sxs-lookup"><span data-stu-id="a9553-125">Write properties and relationships of invitation object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a9553-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="a9553-126">Properties</span></span>
| <span data-ttu-id="a9553-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="a9553-127">Property</span></span>     | <span data-ttu-id="a9553-128">Тип</span><span class="sxs-lookup"><span data-stu-id="a9553-128">Type</span></span>   |<span data-ttu-id="a9553-129">Описание</span><span class="sxs-lookup"><span data-stu-id="a9553-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a9553-130">invitedUserDisplayName</span><span class="sxs-lookup"><span data-stu-id="a9553-130">invitedUserDisplayName</span></span>|<span data-ttu-id="a9553-131">String</span><span class="sxs-lookup"><span data-stu-id="a9553-131">String</span></span>|<span data-ttu-id="a9553-132">Отображаемое имя приглашаемого пользователя.</span><span class="sxs-lookup"><span data-stu-id="a9553-132">The display name of the user being invited.</span></span>|
|<span data-ttu-id="a9553-133">invitedUserEmailAddress</span><span class="sxs-lookup"><span data-stu-id="a9553-133">invitedUserEmailAddress</span></span>|<span data-ttu-id="a9553-134">String</span><span class="sxs-lookup"><span data-stu-id="a9553-134">String</span></span>|<span data-ttu-id="a9553-135">Адрес электронной почты приглашаемого пользователя.</span><span class="sxs-lookup"><span data-stu-id="a9553-135">The email address of the user being invited.</span></span> <span data-ttu-id="a9553-136">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="a9553-136">Required.</span></span> <span data-ttu-id="a9553-137">В адресе электронной почты запрещено использовать следующие специальные символы:</span><span class="sxs-lookup"><span data-stu-id="a9553-137">The following special characters are not permitted in the email address:</span></span><br><ul><li><span data-ttu-id="a9553-138">Тильда (~)</span><span class="sxs-lookup"><span data-stu-id="a9553-138">Tilde (~)</span></span></li><li><span data-ttu-id="a9553-139">Восклицательный знак (`!`)</span><span class="sxs-lookup"><span data-stu-id="a9553-139">Exclamation point (`!`)</span></span></li><li><span data-ttu-id="a9553-140">Знак "собаки" (`@`)</span><span class="sxs-lookup"><span data-stu-id="a9553-140">At sign (`@`)</span></span></li><li><span data-ttu-id="a9553-141">Решетка (`#`)</span><span class="sxs-lookup"><span data-stu-id="a9553-141">Number sign (`#`)</span></span></li><li><span data-ttu-id="a9553-142">Знак доллара (`$`)</span><span class="sxs-lookup"><span data-stu-id="a9553-142">Dollar sign (`$`)</span></span></li><li><span data-ttu-id="a9553-143">Процент (`%`)</span><span class="sxs-lookup"><span data-stu-id="a9553-143">Percent (`%`)</span></span></li><li><span data-ttu-id="a9553-144">Диакритический знак (`^`)</span><span class="sxs-lookup"><span data-stu-id="a9553-144">Circumflex (`^`)</span></span></li><li><span data-ttu-id="a9553-145">Амперсанд (`&`)</span><span class="sxs-lookup"><span data-stu-id="a9553-145">Ampersand (`&`)</span></span></li><li><span data-ttu-id="a9553-146">Звездочка (`*`)</span><span class="sxs-lookup"><span data-stu-id="a9553-146">Asterisk (`*`)</span></span></li><li><span data-ttu-id="a9553-147">Круглые скобки (`( )`)</span><span class="sxs-lookup"><span data-stu-id="a9553-147">Parentheses (`( )`)</span></span></li><li><span data-ttu-id="a9553-148">Дефис (`-`)</span><span class="sxs-lookup"><span data-stu-id="a9553-148">Hyphen (`-`)</span></span></li><li><span data-ttu-id="a9553-149">Знак "плюс" (`+`)</span><span class="sxs-lookup"><span data-stu-id="a9553-149">Plus sign (`+`)</span></span></li><li><span data-ttu-id="a9553-150">Знак равенства (`=`)</span><span class="sxs-lookup"><span data-stu-id="a9553-150">Equal sign (`=`)</span></span></li><li><span data-ttu-id="a9553-151">Квадратные скобки (`[ ]`)</span><span class="sxs-lookup"><span data-stu-id="a9553-151">Brackets (`[ ]`)</span></span></li><li><span data-ttu-id="a9553-152">Фигурные скобки (`{ }`)</span><span class="sxs-lookup"><span data-stu-id="a9553-152">Braces (`{ }`)</span></span></li><li><span data-ttu-id="a9553-153">Обратная косая черта (`\`)</span><span class="sxs-lookup"><span data-stu-id="a9553-153">Backslash (`\`)</span></span></li><li><span data-ttu-id="a9553-154">Косая черта (`/`)</span><span class="sxs-lookup"><span data-stu-id="a9553-154">Slash mark (`/`)</span></span></li><li><span data-ttu-id="a9553-155">Вертикальная черта (`|`)</span><span class="sxs-lookup"><span data-stu-id="a9553-155">Pipe (`|`)</span></span></li><li><span data-ttu-id="a9553-156">Точка с запятой (`;`)</span><span class="sxs-lookup"><span data-stu-id="a9553-156">Semicolon (`;`)</span></span></li><li><span data-ttu-id="a9553-157">Двоеточие (`:`)</span><span class="sxs-lookup"><span data-stu-id="a9553-157">Colon (`:`)</span></span></li><li><span data-ttu-id="a9553-158">Кавычки (`"`)</span><span class="sxs-lookup"><span data-stu-id="a9553-158">Quotation marks (`"`)</span></span></li><li><span data-ttu-id="a9553-159">Угловые скобки (`< >`)</span><span class="sxs-lookup"><span data-stu-id="a9553-159">Angle brackets (`< >`)</span></span></li><li><span data-ttu-id="a9553-160">Вопросительный знак (`?`)</span><span class="sxs-lookup"><span data-stu-id="a9553-160">Question mark (`?`)</span></span></li><li><span data-ttu-id="a9553-161">Запятая (`,`)</span><span class="sxs-lookup"><span data-stu-id="a9553-161">Comma (`,`)</span></span></li></ul><br><span data-ttu-id="a9553-162">Однако применяются следующие исключения:</span><span class="sxs-lookup"><span data-stu-id="a9553-162">However, the following exceptions apply:</span></span><br><ul><li><span data-ttu-id="a9553-163">Точка (`.`) и дефис (`-`) разрешены в любом месте имени пользователя, кроме его начала и конца.</span><span class="sxs-lookup"><span data-stu-id="a9553-163">A period (`.`) or a hyphen (`-`) is permitted anywhere in the user name, except at the beginning or end of the name.</span></span></li><li><span data-ttu-id="a9553-164">Знак подчеркивания (`_`) может находиться в любом месте имени пользователя,</span><span class="sxs-lookup"><span data-stu-id="a9553-164">An underscore (`_`) is permitted anywhere in the user name.</span></span> <span data-ttu-id="a9553-165">в том числе в начале и в конце имени.</span><span class="sxs-lookup"><span data-stu-id="a9553-165">This includes at the beginning or end of the name.</span></span></li></ul>|
|<span data-ttu-id="a9553-166">invitedUserMessageInfo</span><span class="sxs-lookup"><span data-stu-id="a9553-166">invitedUserMessageInfo</span></span>|[<span data-ttu-id="a9553-167">invitedUserMessageInfo</span><span class="sxs-lookup"><span data-stu-id="a9553-167">invitedUserMessageInfo</span></span>](invitedusermessageinfo.md)|<span data-ttu-id="a9553-168">Дополнительные настройки сообщения, которое отправляется приглашаемому пользователю, в том числе настройка текста, языка и списка получателей копии сообщения.</span><span class="sxs-lookup"><span data-stu-id="a9553-168">Additional configuration for the message being sent to the invited user, including customizing message text, language and cc recipient list.</span></span>|
|<span data-ttu-id="a9553-169">sendInvitationMessage</span><span class="sxs-lookup"><span data-stu-id="a9553-169">sendInvitationMessage</span></span>|<span data-ttu-id="a9553-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9553-170">Boolean</span></span>|<span data-ttu-id="a9553-p104">Указывает, следует ли отправлять письмо приглашаемому пользователю. Значение по умолчанию: false.</span><span class="sxs-lookup"><span data-stu-id="a9553-p104">Indicates whether an email should be sent to the user being invited or not. The default is false.</span></span>|
|<span data-ttu-id="a9553-173">inviteRedirectUrl</span><span class="sxs-lookup"><span data-stu-id="a9553-173">inviteRedirectUrl</span></span>|<span data-ttu-id="a9553-174">String</span><span class="sxs-lookup"><span data-stu-id="a9553-174">String</span></span>|<span data-ttu-id="a9553-p105">URL-адрес, на который пользователь перенаправляется после активации приглашения. Указывать обязательно.</span><span class="sxs-lookup"><span data-stu-id="a9553-p105">The URL user should be redirected to once the invitation is redeemed. Required.</span></span>|
|<span data-ttu-id="a9553-177">inviteRedeemUrl</span><span class="sxs-lookup"><span data-stu-id="a9553-177">inviteRedeemUrl</span></span>|<span data-ttu-id="a9553-178">String</span><span class="sxs-lookup"><span data-stu-id="a9553-178">String</span></span>|<span data-ttu-id="a9553-p106">URL-адрес для активации приглашения. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a9553-p106">The URL user can use to redeem his invitation. Read-Only</span></span>|
|<span data-ttu-id="a9553-181">invitedUserType</span><span class="sxs-lookup"><span data-stu-id="a9553-181">invitedUserType</span></span>|<span data-ttu-id="a9553-182">String</span><span class="sxs-lookup"><span data-stu-id="a9553-182">String</span></span>|<span data-ttu-id="a9553-183">Элемент userType, связанный с приглашаемым пользователем.</span><span class="sxs-lookup"><span data-stu-id="a9553-183">The userType of the user being invited.</span></span> <span data-ttu-id="a9553-184">Значение по умолчанию: Guest.</span><span class="sxs-lookup"><span data-stu-id="a9553-184">By default, this is Guest.</span></span> <span data-ttu-id="a9553-185">Вы можете пригласить как участник, если вы являетесь администратором компании.</span><span class="sxs-lookup"><span data-stu-id="a9553-185">You can invite as Member if you're are company administrator.</span></span> |
|<span data-ttu-id="a9553-186">status</span><span class="sxs-lookup"><span data-stu-id="a9553-186">status</span></span>|<span data-ttu-id="a9553-187">String</span><span class="sxs-lookup"><span data-stu-id="a9553-187">String</span></span>|<span data-ttu-id="a9553-p108">Состояние приглашения. Возможные значения: PendingAcceptance, Completed, InProgress и Error</span><span class="sxs-lookup"><span data-stu-id="a9553-p108">The status of the invitation. Possible values: PendingAcceptance, Completed, InProgress, and Error</span></span>|

## <a name="relationships"></a><span data-ttu-id="a9553-190">Связи</span><span class="sxs-lookup"><span data-stu-id="a9553-190">Relationships</span></span>
| <span data-ttu-id="a9553-191">Связь</span><span class="sxs-lookup"><span data-stu-id="a9553-191">Relationship</span></span> | <span data-ttu-id="a9553-192">Тип</span><span class="sxs-lookup"><span data-stu-id="a9553-192">Type</span></span>   |<span data-ttu-id="a9553-193">Описание</span><span class="sxs-lookup"><span data-stu-id="a9553-193">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a9553-194">invitedUser</span><span class="sxs-lookup"><span data-stu-id="a9553-194">invitedUser</span></span>|[<span data-ttu-id="a9553-195">user</span><span class="sxs-lookup"><span data-stu-id="a9553-195">user</span></span>](user.md)|<span data-ttu-id="a9553-p109">Пользователь, создаваемый при создании приглашения. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a9553-p109">The user created as part of the invitation creation. Read-Only</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a9553-198">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a9553-198">JSON representation</span></span>
<span data-ttu-id="a9553-199">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a9553-199">Here is a JSON representation of the resource</span></span>

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
