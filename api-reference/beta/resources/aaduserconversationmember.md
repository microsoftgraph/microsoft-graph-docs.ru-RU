---
title: Тип ресурса aadUserConversationMember
description: Представляет пользователя Azure Active Directory в чате или канале.
localization_priority: Priority
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 4cd7b6ac208c719663eb04adf91a98ae6fa7da39
ms.sourcegitcommit: 0d4377b0153bc339ab7b3b1a6ee4d52848b622d4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2020
ms.locfileid: "49714342"
---
# <a name="aaduserconversationmember-resource-type"></a><span data-ttu-id="ff526-103">Тип ресурса aadUserConversationMember</span><span class="sxs-lookup"><span data-stu-id="ff526-103">aadUserConversationMember resource type</span></span>

<span data-ttu-id="ff526-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff526-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff526-105">Представляет пользователя Azure Active Directory в [команде](team.md), [канале](channel.md) или [чате](chat.md).</span><span class="sxs-lookup"><span data-stu-id="ff526-105">Represents an Azure Active Directory user in a [team](team.md) or a [channel](channel.md) or a [chat](chat.md).</span></span> <span data-ttu-id="ff526-106">Этот тип наследуется от [conversationMember](conversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="ff526-106">This type inherits from [conversationMember](conversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="ff526-107">Методы</span><span class="sxs-lookup"><span data-stu-id="ff526-107">Methods</span></span>

| <span data-ttu-id="ff526-108">Метод</span><span class="sxs-lookup"><span data-stu-id="ff526-108">Method</span></span>       | <span data-ttu-id="ff526-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ff526-109">Return Type</span></span>  |<span data-ttu-id="ff526-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ff526-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ff526-111">Список участников группы</span><span class="sxs-lookup"><span data-stu-id="ff526-111">List team members</span></span>](../api/team-list-members.md)|<span data-ttu-id="ff526-112">Коллекция [conversationMember](../resources/conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="ff526-112">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="ff526-113">Получение списка участников группы.</span><span class="sxs-lookup"><span data-stu-id="ff526-113">Get the list of members in the team.</span></span>|
|[<span data-ttu-id="ff526-114">Добавление участника в команду</span><span class="sxs-lookup"><span data-stu-id="ff526-114">Add team member</span></span>](../api/team-post-members.md)|[<span data-ttu-id="ff526-115">conversationMember</span><span class="sxs-lookup"><span data-stu-id="ff526-115">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="ff526-116">Добавление нового участника в группу.</span><span class="sxs-lookup"><span data-stu-id="ff526-116">Add a new member to the team.</span></span>|
|[<span data-ttu-id="ff526-117">Массовое добавление участников в группу</span><span class="sxs-lookup"><span data-stu-id="ff526-117">Add team members in bulk</span></span>](../api/conversationmembers-add.md)|<span data-ttu-id="ff526-118">Коллекция [actionResultPart](../resources/actionresultpart.md)</span><span class="sxs-lookup"><span data-stu-id="ff526-118">[actionResultPart](../resources/actionresultpart.md) collection</span></span>|<span data-ttu-id="ff526-119">Добавление нескольких участников в команду одним запросом.</span><span class="sxs-lookup"><span data-stu-id="ff526-119">Add multiple members to the team in a single request.</span></span>|
|[<span data-ttu-id="ff526-120">Получение участника группы</span><span class="sxs-lookup"><span data-stu-id="ff526-120">Get team member</span></span>](../api/team-get-members.md) | <span data-ttu-id="ff526-121">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="ff526-121">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="ff526-122">Получение участника группы.</span><span class="sxs-lookup"><span data-stu-id="ff526-122">Get a member in the team.</span></span>|
|[<span data-ttu-id="ff526-123">Обновление роли участника команды</span><span class="sxs-lookup"><span data-stu-id="ff526-123">Update team member's role</span></span>](../api/team-update-members.md)|[<span data-ttu-id="ff526-124">conversationMember</span><span class="sxs-lookup"><span data-stu-id="ff526-124">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="ff526-125">Перевод пользователя из категории участников в категорию владельцев или наоборот, из категории владельцев в категорию обычных участников.</span><span class="sxs-lookup"><span data-stu-id="ff526-125">Change a member to an owner or back to a regular member.</span></span>|
|[<span data-ttu-id="ff526-126">Удаление участника группы</span><span class="sxs-lookup"><span data-stu-id="ff526-126">Remove team member</span></span>](../api/team-delete-members.md)|<span data-ttu-id="ff526-127">Нет</span><span class="sxs-lookup"><span data-stu-id="ff526-127">None</span></span>|<span data-ttu-id="ff526-128">Удаление существующего участника из группы.</span><span class="sxs-lookup"><span data-stu-id="ff526-128">Remove an existing member from the team.</span></span>|
|[<span data-ttu-id="ff526-129">Перечисление участников канала</span><span class="sxs-lookup"><span data-stu-id="ff526-129">List channel members</span></span>](../api/channel-list-members.md) | <span data-ttu-id="ff526-130">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="ff526-130">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="ff526-131">Получение списка всех участников канала.</span><span class="sxs-lookup"><span data-stu-id="ff526-131">Get the list of all members in a channel.</span></span>|
|[<span data-ttu-id="ff526-132">Добавление участника канала</span><span class="sxs-lookup"><span data-stu-id="ff526-132">Add channel member</span></span>](../api/channel-post-members.md) | [<span data-ttu-id="ff526-133">conversationMember</span><span class="sxs-lookup"><span data-stu-id="ff526-133">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="ff526-134">Добавление участника в канал.</span><span class="sxs-lookup"><span data-stu-id="ff526-134">Add a member to a channel.</span></span> <span data-ttu-id="ff526-135">Поддерживается только для `channel` с типом членства `private`.</span><span class="sxs-lookup"><span data-stu-id="ff526-135">Only supported for `channel`with membershipType of `private`.</span></span>|
|[<span data-ttu-id="ff526-136">Получение участника канала</span><span class="sxs-lookup"><span data-stu-id="ff526-136">Get channel member</span></span>](../api/channel-get-members.md) | <span data-ttu-id="ff526-137">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="ff526-137">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="ff526-138">Получение участника канала.</span><span class="sxs-lookup"><span data-stu-id="ff526-138">Get a member in a channel.</span></span>|
|[<span data-ttu-id="ff526-139">Обновление роли участника канала</span><span class="sxs-lookup"><span data-stu-id="ff526-139">Update channel member's role</span></span>](../api/channel-update-members.md) | [<span data-ttu-id="ff526-140">conversationMember</span><span class="sxs-lookup"><span data-stu-id="ff526-140">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="ff526-141">Обновление свойства участника канала.</span><span class="sxs-lookup"><span data-stu-id="ff526-141">Update the properties of a member of the channel.</span></span> <span data-ttu-id="ff526-142">Поддерживается только для канала с типом членства `private`.</span><span class="sxs-lookup"><span data-stu-id="ff526-142">Only supported for channel with membershipType of `private`.</span></span>|
|[<span data-ttu-id="ff526-143">Удаление участника канала</span><span class="sxs-lookup"><span data-stu-id="ff526-143">Remove channel member</span></span>](../api/channel-delete-members.md) | <span data-ttu-id="ff526-144">Нет</span><span class="sxs-lookup"><span data-stu-id="ff526-144">None</span></span> | <span data-ttu-id="ff526-145">Удаление участника канала.</span><span class="sxs-lookup"><span data-stu-id="ff526-145">Delete a member from a channel.</span></span> <span data-ttu-id="ff526-146">Поддерживается, только если параметру `channelType` присвоено значение `private`.</span><span class="sxs-lookup"><span data-stu-id="ff526-146">Only supported for `channelType` of `private`.</span></span>|
|[<span data-ttu-id="ff526-147">Перечисление участников чата</span><span class="sxs-lookup"><span data-stu-id="ff526-147">List chat members</span></span>](../api/chat-list-members.md) | <span data-ttu-id="ff526-148">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="ff526-148">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="ff526-149">Получение списка всех участников чата.</span><span class="sxs-lookup"><span data-stu-id="ff526-149">Get the list of all members in a chat.</span></span>|
|[<span data-ttu-id="ff526-150">Добавление участника в чат</span><span class="sxs-lookup"><span data-stu-id="ff526-150">Add chat member</span></span>](../api/chat-post-members.md) | <span data-ttu-id="ff526-151">Заголовок размещения</span><span class="sxs-lookup"><span data-stu-id="ff526-151">Location header</span></span> | <span data-ttu-id="ff526-152">Добавление участника в чат.</span><span class="sxs-lookup"><span data-stu-id="ff526-152">Add a member to a chat.</span></span>| 
|[<span data-ttu-id="ff526-153">Получение участника чата</span><span class="sxs-lookup"><span data-stu-id="ff526-153">Get chat member</span></span>](../api/chat-get-members.md) | [<span data-ttu-id="ff526-154">conversationMember</span><span class="sxs-lookup"><span data-stu-id="ff526-154">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="ff526-155">Получение участника чата.</span><span class="sxs-lookup"><span data-stu-id="ff526-155">Get a member in a chat.</span></span>|
|[<span data-ttu-id="ff526-156">Удаление участника чата</span><span class="sxs-lookup"><span data-stu-id="ff526-156">Remove chat member</span></span>](../api/chat-delete-members.md) | <span data-ttu-id="ff526-157">Нет</span><span class="sxs-lookup"><span data-stu-id="ff526-157">None</span></span> | <span data-ttu-id="ff526-158">Удаление участника из чата.</span><span class="sxs-lookup"><span data-stu-id="ff526-158">Remove a member from a chat.</span></span>| 

## <a name="properties"></a><span data-ttu-id="ff526-159">Свойства</span><span class="sxs-lookup"><span data-stu-id="ff526-159">Properties</span></span>

| <span data-ttu-id="ff526-160">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff526-160">Property</span></span>   | <span data-ttu-id="ff526-161">Тип</span><span class="sxs-lookup"><span data-stu-id="ff526-161">Type</span></span> |<span data-ttu-id="ff526-162">Описание</span><span class="sxs-lookup"><span data-stu-id="ff526-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff526-163">id</span><span class="sxs-lookup"><span data-stu-id="ff526-163">id</span></span>| <span data-ttu-id="ff526-164">String</span><span class="sxs-lookup"><span data-stu-id="ff526-164">String</span></span> | <span data-ttu-id="ff526-165">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ff526-165">Read-only.</span></span> <span data-ttu-id="ff526-166">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="ff526-166">Unique ID of the user.</span></span>|
|<span data-ttu-id="ff526-167">displayName</span><span class="sxs-lookup"><span data-stu-id="ff526-167">displayName</span></span>| <span data-ttu-id="ff526-168">String</span><span class="sxs-lookup"><span data-stu-id="ff526-168">String</span></span> | <span data-ttu-id="ff526-169">Отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="ff526-169">The display name of the user.</span></span> |
|<span data-ttu-id="ff526-170">roles</span><span class="sxs-lookup"><span data-stu-id="ff526-170">roles</span></span>| <span data-ttu-id="ff526-171">Набор строк</span><span class="sxs-lookup"><span data-stu-id="ff526-171">String collection</span></span> | <span data-ttu-id="ff526-172">Роли этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="ff526-172">The roles for that user.</span></span> |
|<span data-ttu-id="ff526-173">userId</span><span class="sxs-lookup"><span data-stu-id="ff526-173">userId</span></span>| <span data-ttu-id="ff526-174">String</span><span class="sxs-lookup"><span data-stu-id="ff526-174">String</span></span> | <span data-ttu-id="ff526-175">GUID пользователя.</span><span class="sxs-lookup"><span data-stu-id="ff526-175">The GUID of the user.</span></span> |
|<span data-ttu-id="ff526-176">email</span><span class="sxs-lookup"><span data-stu-id="ff526-176">email</span></span>| <span data-ttu-id="ff526-177">String</span><span class="sxs-lookup"><span data-stu-id="ff526-177">String</span></span>  | <span data-ttu-id="ff526-178">Электронный адрес пользователя.</span><span class="sxs-lookup"><span data-stu-id="ff526-178">The email address of the user.</span></span> |
|<span data-ttu-id="ff526-179">tenantId</span><span class="sxs-lookup"><span data-stu-id="ff526-179">tenantId</span></span>| <span data-ttu-id="ff526-180">string</span><span class="sxs-lookup"><span data-stu-id="ff526-180">string</span></span>  | <span data-ttu-id="ff526-181">ИД клиента, которому принадлежит пользователь Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ff526-181">TenantId which the Azure AD user belongs to.</span></span> |
|<span data-ttu-id="ff526-182">visibleHistoryStartDateTime</span><span class="sxs-lookup"><span data-stu-id="ff526-182">visibleHistoryStartDateTime</span></span>| <span data-ttu-id="ff526-183">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff526-183">DateTimeOffset</span></span>  | <span data-ttu-id="ff526-184">Метка времени, обозначающая, насколько глубоко участник беседы может видеть историю беседы.</span><span class="sxs-lookup"><span data-stu-id="ff526-184">The timestamp denoting how far back a conversation's history is shared with the conversation member.</span></span> <span data-ttu-id="ff526-185">Это свойство можно задать только для участников чата.</span><span class="sxs-lookup"><span data-stu-id="ff526-185">This property is settable only for members of a chat.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ff526-186">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ff526-186">JSON representation</span></span>

<span data-ttu-id="ff526-187">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ff526-187">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.aadUserConversationMember",
  "baseType": "microsoft.graph.conversationMember",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "id": "String (identifier)",
  "roles": [
    "String"
  ],
  "displayName": "String",
  "visibleHistoryStartDateTime": "String (timestamp)",
  "userId": "String",
  "email": "String",
  "tenantId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "aadUserConversationMember",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
