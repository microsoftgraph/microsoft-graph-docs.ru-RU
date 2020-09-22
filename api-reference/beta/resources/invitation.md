---
title: Тип ресурса invitation
description: Представляет приглашение, используемое для добавления внешних пользователей в организацию.
localization_priority: Normal
author: elisolMS
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0e210def9b58a6ff5a9abe295ec869bb6ab88051
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989075"
---
# <a name="invitation-resource-type"></a><span data-ttu-id="03495-103">Тип ресурса invitation</span><span class="sxs-lookup"><span data-stu-id="03495-103">invitation resource type</span></span>

<span data-ttu-id="03495-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03495-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03495-105">Представляет приглашение, используемое для добавления внешних пользователей в организацию.</span><span class="sxs-lookup"><span data-stu-id="03495-105">Represents an invitation that is used to add external users to an organization.</span></span> 

<span data-ttu-id="03495-106">Процесс приглашения:</span><span class="sxs-lookup"><span data-stu-id="03495-106">The invitation process uses the following flow:</span></span>

* <span data-ttu-id="03495-107">Создается приглашение.</span><span class="sxs-lookup"><span data-stu-id="03495-107">An invitation is created</span></span>
* <span data-ttu-id="03495-108">Приглашение с соответствующей ссылкой отправляется пользователю.</span><span class="sxs-lookup"><span data-stu-id="03495-108">An invitation is sent to the invited user (containing an invitation link)</span></span>
* <span data-ttu-id="03495-109">Пользователь щелкает эту ссылку, выполняет вход и активирует приглашение. На этом создание объекта user, представляющего приглашенного пользователя, завершается.</span><span class="sxs-lookup"><span data-stu-id="03495-109">The invited user clicks on the invitation link, signs in and redeems the invitation and creation of the user entity representing the invited user completes</span></span>
* <span data-ttu-id="03495-110">После активации пользователь перенаправляется на определенную страницу.</span><span class="sxs-lookup"><span data-stu-id="03495-110">The user is redirected to a specific page after redemption completes</span></span>

<span data-ttu-id="03495-p101">При создании приглашения возвращается URL-адрес активации (*inviteRedeemUrl*). API создания приглашений может автоматически отправлять приглашенному пользователю письмо с URL-адресом активации, если параметру *sendInvitationMessage* задано значение true. Вы также можете настроить сообщение, которое будет отправлено приглашенному пользователю. Если вы хотите отправить URL-адрес активации другим способом, задайте параметру *sendInvitationMessage* значение false и используйте URL-адрес активации из отклика для создания собственного сообщения. В настоящее время нет API для выполнения процесса активации. Приглашенный пользователь должен щелкнуть ссылку *inviteRedeemUrl* в сообщении, отправка которого описана выше, и пройти интерактивную процедуру активации в браузере. После этого приглашенный пользователь становится внешним пользователем в организации.</span><span class="sxs-lookup"><span data-stu-id="03495-p101">Creating an invitation will return a redemption URL in the response (*inviteRedeemUrl*). The create invitation API can automatically send an email containing the redemption URL to the invited user, by setting the *sendInvitationMessage* to true. You can also customize the message that will be sent to the invited user. Instead, if you wish to send the redemption URL through some other means, you can set the *sendInvitationMessage* to false and use the redeem URL from the response to craft your own communication. Currently, there is no API to perform the redemption process. The invited user has to click on the *inviteRedeemUrl* link sent in the communication in the step above, and go through the interactive redemption process in a browser. Once completed, the invited user becomes an external user in the organization.</span></span>

>[!NOTE]
><span data-ttu-id="03495-118">Состояние приглашения отслеживается с помощью свойств **Свойства** и **екстерналусерстатечанжедатетиме** для ресурса внешнего [пользователя](user.md) , созданного в составе запроса приглашения.</span><span class="sxs-lookup"><span data-stu-id="03495-118">The invitation status is tracked using the **externalUserState** and the **externalUserStateChangeDateTime** properties on the external [user](user.md) resource created as part of the invitation request.</span></span>

## <a name="methods"></a><span data-ttu-id="03495-119">Методы</span><span class="sxs-lookup"><span data-stu-id="03495-119">Methods</span></span>
| <span data-ttu-id="03495-120">Метод</span><span class="sxs-lookup"><span data-stu-id="03495-120">Method</span></span>       | <span data-ttu-id="03495-121">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="03495-121">Return Type</span></span>  |<span data-ttu-id="03495-122">Описание</span><span class="sxs-lookup"><span data-stu-id="03495-122">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="03495-123">Создание приглашений</span><span class="sxs-lookup"><span data-stu-id="03495-123">Create invitation</span></span>](../api/invitation-post.md) | <span data-ttu-id="03495-124">invitation</span><span class="sxs-lookup"><span data-stu-id="03495-124">invitation</span></span> | <span data-ttu-id="03495-125">Запись свойств и отношений объекта приглашения.</span><span class="sxs-lookup"><span data-stu-id="03495-125">Write properties and relationships of invitation object.</span></span>|

## <a name="properties"></a><span data-ttu-id="03495-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="03495-126">Properties</span></span>
| <span data-ttu-id="03495-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="03495-127">Property</span></span>     | <span data-ttu-id="03495-128">Тип</span><span class="sxs-lookup"><span data-stu-id="03495-128">Type</span></span>   |<span data-ttu-id="03495-129">Описание</span><span class="sxs-lookup"><span data-stu-id="03495-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="03495-130">invitedUserDisplayName</span><span class="sxs-lookup"><span data-stu-id="03495-130">invitedUserDisplayName</span></span>|<span data-ttu-id="03495-131">String</span><span class="sxs-lookup"><span data-stu-id="03495-131">String</span></span>|<span data-ttu-id="03495-132">Отображаемое имя приглашаемого пользователя.</span><span class="sxs-lookup"><span data-stu-id="03495-132">The display name of the user being invited.</span></span>|
|<span data-ttu-id="03495-133">invitedUserEmailAddress</span><span class="sxs-lookup"><span data-stu-id="03495-133">invitedUserEmailAddress</span></span>|<span data-ttu-id="03495-134">String</span><span class="sxs-lookup"><span data-stu-id="03495-134">String</span></span>|<span data-ttu-id="03495-135">Адрес электронной почты приглашаемого пользователя.</span><span class="sxs-lookup"><span data-stu-id="03495-135">The email address of the user being invited.</span></span> <span data-ttu-id="03495-136">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="03495-136">Required.</span></span> <span data-ttu-id="03495-137">В адресе электронной почты запрещено использовать следующие специальные символы:</span><span class="sxs-lookup"><span data-stu-id="03495-137">The following special characters are not permitted in the email address:</span></span><br><ul><li><span data-ttu-id="03495-138">Тильда (~)</span><span class="sxs-lookup"><span data-stu-id="03495-138">Tilde (~)</span></span></li><li><span data-ttu-id="03495-139">Восклицательный знак (`!`)</span><span class="sxs-lookup"><span data-stu-id="03495-139">Exclamation point (`!`)</span></span></li><li><span data-ttu-id="03495-140">Знак "собаки" (`@`)</span><span class="sxs-lookup"><span data-stu-id="03495-140">At sign (`@`)</span></span></li><li><span data-ttu-id="03495-141">Решетка (`#`)</span><span class="sxs-lookup"><span data-stu-id="03495-141">Number sign (`#`)</span></span></li><li><span data-ttu-id="03495-142">Знак доллара (`$`)</span><span class="sxs-lookup"><span data-stu-id="03495-142">Dollar sign (`$`)</span></span></li><li><span data-ttu-id="03495-143">Процент (`%`)</span><span class="sxs-lookup"><span data-stu-id="03495-143">Percent (`%`)</span></span></li><li><span data-ttu-id="03495-144">Диакритический знак (`^`)</span><span class="sxs-lookup"><span data-stu-id="03495-144">Circumflex (`^`)</span></span></li><li><span data-ttu-id="03495-145">Амперсанд (`&`)</span><span class="sxs-lookup"><span data-stu-id="03495-145">Ampersand (`&`)</span></span></li><li><span data-ttu-id="03495-146">Звездочка (`*`)</span><span class="sxs-lookup"><span data-stu-id="03495-146">Asterisk (`*`)</span></span></li><li><span data-ttu-id="03495-147">Круглые скобки (`( )`)</span><span class="sxs-lookup"><span data-stu-id="03495-147">Parentheses (`( )`)</span></span></li><li><span data-ttu-id="03495-148">Дефис (`-`)</span><span class="sxs-lookup"><span data-stu-id="03495-148">Hyphen (`-`)</span></span></li><li><span data-ttu-id="03495-149">Знак "плюс" (`+`)</span><span class="sxs-lookup"><span data-stu-id="03495-149">Plus sign (`+`)</span></span></li><li><span data-ttu-id="03495-150">Знак равенства (`=`)</span><span class="sxs-lookup"><span data-stu-id="03495-150">Equal sign (`=`)</span></span></li><li><span data-ttu-id="03495-151">Квадратные скобки (`[ ]`)</span><span class="sxs-lookup"><span data-stu-id="03495-151">Brackets (`[ ]`)</span></span></li><li><span data-ttu-id="03495-152">Фигурные скобки (`{ }`)</span><span class="sxs-lookup"><span data-stu-id="03495-152">Braces (`{ }`)</span></span></li><li><span data-ttu-id="03495-153">Обратная косая черта (`\`)</span><span class="sxs-lookup"><span data-stu-id="03495-153">Backslash (`\`)</span></span></li><li><span data-ttu-id="03495-154">Косая черта (`/`)</span><span class="sxs-lookup"><span data-stu-id="03495-154">Slash mark (`/`)</span></span></li><li><span data-ttu-id="03495-155">Вертикальная черта (`|`)</span><span class="sxs-lookup"><span data-stu-id="03495-155">Pipe (`|`)</span></span></li><li><span data-ttu-id="03495-156">Точка с запятой (`;`)</span><span class="sxs-lookup"><span data-stu-id="03495-156">Semicolon (`;`)</span></span></li><li><span data-ttu-id="03495-157">Двоеточие (`:`)</span><span class="sxs-lookup"><span data-stu-id="03495-157">Colon (`:`)</span></span></li><li><span data-ttu-id="03495-158">Кавычки (`"`)</span><span class="sxs-lookup"><span data-stu-id="03495-158">Quotation marks (`"`)</span></span></li><li><span data-ttu-id="03495-159">Угловые скобки (`< >`)</span><span class="sxs-lookup"><span data-stu-id="03495-159">Angle brackets (`< >`)</span></span></li><li><span data-ttu-id="03495-160">Вопросительный знак (`?`)</span><span class="sxs-lookup"><span data-stu-id="03495-160">Question mark (`?`)</span></span></li><li><span data-ttu-id="03495-161">Запятая (`,`)</span><span class="sxs-lookup"><span data-stu-id="03495-161">Comma (`,`)</span></span></li></ul><br><span data-ttu-id="03495-162">Однако применяются следующие исключения:</span><span class="sxs-lookup"><span data-stu-id="03495-162">However, the following exceptions apply:</span></span><br><ul><li><span data-ttu-id="03495-163">Точка (`.`) и дефис (`-`) разрешены в любом месте имени пользователя, кроме его начала и конца.</span><span class="sxs-lookup"><span data-stu-id="03495-163">A period (`.`) or a hyphen (`-`) is permitted anywhere in the user name, except at the beginning or end of the name.</span></span></li><li><span data-ttu-id="03495-164">Знак подчеркивания (`_`) может находиться в любом месте имени пользователя,</span><span class="sxs-lookup"><span data-stu-id="03495-164">An underscore (`_`) is permitted anywhere in the user name.</span></span> <span data-ttu-id="03495-165">в том числе в начале и в конце имени.</span><span class="sxs-lookup"><span data-stu-id="03495-165">This includes at the beginning or end of the name.</span></span></li></ul>|
|<span data-ttu-id="03495-166">invitedUserMessageInfo</span><span class="sxs-lookup"><span data-stu-id="03495-166">invitedUserMessageInfo</span></span>|[<span data-ttu-id="03495-167">invitedUserMessageInfo</span><span class="sxs-lookup"><span data-stu-id="03495-167">invitedUserMessageInfo</span></span>](invitedusermessageinfo.md)|<span data-ttu-id="03495-168">Дополнительные настройки сообщения, которое отправляется приглашаемому пользователю, в том числе настройка текста, языка и списка получателей копии сообщения.</span><span class="sxs-lookup"><span data-stu-id="03495-168">Additional configuration for the message being sent to the invited user, including customizing message text, language and cc recipient list.</span></span>|
|<span data-ttu-id="03495-169">sendInvitationMessage</span><span class="sxs-lookup"><span data-stu-id="03495-169">sendInvitationMessage</span></span>|<span data-ttu-id="03495-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="03495-170">Boolean</span></span>|<span data-ttu-id="03495-p104">Указывает, следует ли отправлять письмо приглашаемому пользователю. Значение по умолчанию: false.</span><span class="sxs-lookup"><span data-stu-id="03495-p104">Indicates whether an email should be sent to the user being invited or not. The default is false.</span></span>|
|<span data-ttu-id="03495-173">inviteRedirectUrl</span><span class="sxs-lookup"><span data-stu-id="03495-173">inviteRedirectUrl</span></span>|<span data-ttu-id="03495-174">String</span><span class="sxs-lookup"><span data-stu-id="03495-174">String</span></span>|<span data-ttu-id="03495-p105">URL-адрес, на который пользователь перенаправляется после активации приглашения. Указывать обязательно.</span><span class="sxs-lookup"><span data-stu-id="03495-p105">The URL user should be redirected to once the invitation is redeemed. Required.</span></span>|
|<span data-ttu-id="03495-177">inviteRedeemUrl</span><span class="sxs-lookup"><span data-stu-id="03495-177">inviteRedeemUrl</span></span>|<span data-ttu-id="03495-178">String</span><span class="sxs-lookup"><span data-stu-id="03495-178">String</span></span>|<span data-ttu-id="03495-179">URL-адрес, который пользователь может использовать для активации приглашения.</span><span class="sxs-lookup"><span data-stu-id="03495-179">The URL the user can use to redeem their invitation.</span></span> <span data-ttu-id="03495-180">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="03495-180">Read-only.</span></span>|
|<span data-ttu-id="03495-181">invitedUserType</span><span class="sxs-lookup"><span data-stu-id="03495-181">invitedUserType</span></span>|<span data-ttu-id="03495-182">String</span><span class="sxs-lookup"><span data-stu-id="03495-182">String</span></span>|<span data-ttu-id="03495-183">Элемент userType, связанный с приглашаемым пользователем.</span><span class="sxs-lookup"><span data-stu-id="03495-183">The userType of the user being invited.</span></span> <span data-ttu-id="03495-184">Значение по умолчанию: Guest.</span><span class="sxs-lookup"><span data-stu-id="03495-184">By default, this is Guest.</span></span> <span data-ttu-id="03495-185">Вы можете пригласить как участник, если вы являетесь администратором компании.</span><span class="sxs-lookup"><span data-stu-id="03495-185">You can invite as Member if you're are company administrator.</span></span> |
|<span data-ttu-id="03495-186">status</span><span class="sxs-lookup"><span data-stu-id="03495-186">status</span></span>|<span data-ttu-id="03495-187">String</span><span class="sxs-lookup"><span data-stu-id="03495-187">String</span></span>|<span data-ttu-id="03495-p108">Состояние приглашения. Возможные значения: PendingAcceptance, Completed, InProgress и Error</span><span class="sxs-lookup"><span data-stu-id="03495-p108">The status of the invitation. Possible values: PendingAcceptance, Completed, InProgress, and Error</span></span>|

## <a name="relationships"></a><span data-ttu-id="03495-190">Связи</span><span class="sxs-lookup"><span data-stu-id="03495-190">Relationships</span></span>
| <span data-ttu-id="03495-191">Связь</span><span class="sxs-lookup"><span data-stu-id="03495-191">Relationship</span></span> | <span data-ttu-id="03495-192">Тип</span><span class="sxs-lookup"><span data-stu-id="03495-192">Type</span></span>   |<span data-ttu-id="03495-193">Описание</span><span class="sxs-lookup"><span data-stu-id="03495-193">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="03495-194">invitedUser</span><span class="sxs-lookup"><span data-stu-id="03495-194">invitedUser</span></span>|[<span data-ttu-id="03495-195">user</span><span class="sxs-lookup"><span data-stu-id="03495-195">user</span></span>](user.md)|<span data-ttu-id="03495-p109">Пользователь, создаваемый при создании приглашения. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="03495-p109">The user created as part of the invitation creation. Read-Only</span></span>|

## <a name="json-representation"></a><span data-ttu-id="03495-198">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="03495-198">JSON representation</span></span>
<span data-ttu-id="03495-199">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="03495-199">Here is a JSON representation of the resource</span></span>

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


