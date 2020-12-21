---
title: Тип ресурса aadUserConversationMember
description: Представляет пользователя Azure Active Directory в чате или канале.
localization_priority: Priority
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7f19c5a2b711ab6c39069364c641066f1d9c6dbf
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "49705970"
---
# <a name="aaduserconversationmember-resource-type"></a><span data-ttu-id="9fd66-103">Тип ресурса aadUserConversationMember</span><span class="sxs-lookup"><span data-stu-id="9fd66-103">aadUserConversationMember resource type</span></span>

<span data-ttu-id="9fd66-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9fd66-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9fd66-105">Представляет пользователя Azure Active Directory в [чате](chat.md) или [канале](channel.md).</span><span class="sxs-lookup"><span data-stu-id="9fd66-105">Represents an Azure Active Directory user in a [chat](chat.md) or [channel](channel.md).</span></span> <span data-ttu-id="9fd66-106">Этот тип наследуется от [conversationMember](conversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="9fd66-106">This type inherits from [conversationMember](conversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="9fd66-107">Методы</span><span class="sxs-lookup"><span data-stu-id="9fd66-107">Methods</span></span>

| <span data-ttu-id="9fd66-108">Метод</span><span class="sxs-lookup"><span data-stu-id="9fd66-108">Method</span></span>       | <span data-ttu-id="9fd66-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9fd66-109">Return Type</span></span>  |<span data-ttu-id="9fd66-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9fd66-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9fd66-111">Список участников команды</span><span class="sxs-lookup"><span data-stu-id="9fd66-111">List team members</span></span>](../api/team-list-members.md)|<span data-ttu-id="9fd66-112">Коллекция [conversationMember](../resources/conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="9fd66-112">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="9fd66-113">Получение списка участников команды.</span><span class="sxs-lookup"><span data-stu-id="9fd66-113">Get the list of members in the team.</span></span>|
|[<span data-ttu-id="9fd66-114">Получение участника команды</span><span class="sxs-lookup"><span data-stu-id="9fd66-114">Get team member</span></span>](../api/team-get-members.md) | <span data-ttu-id="9fd66-115">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="9fd66-115">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="9fd66-116">Получение участника команды.</span><span class="sxs-lookup"><span data-stu-id="9fd66-116">Get a member in the team.</span></span>|
|[<span data-ttu-id="9fd66-117">Добавление участника в команду</span><span class="sxs-lookup"><span data-stu-id="9fd66-117">Add team member</span></span>](../api/team-post-members.md)|[<span data-ttu-id="9fd66-118">conversationMember</span><span class="sxs-lookup"><span data-stu-id="9fd66-118">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="9fd66-119">Добавление нового участника в команду.</span><span class="sxs-lookup"><span data-stu-id="9fd66-119">Add a new member to the team.</span></span>|
|[<span data-ttu-id="9fd66-120">Массовое добавление участников в команду</span><span class="sxs-lookup"><span data-stu-id="9fd66-120">Add team members in bulk</span></span>](../api/conversationmembers-add.md)|<span data-ttu-id="9fd66-121">Коллекция [actionResultPart](../resources/actionresultpart.md)</span><span class="sxs-lookup"><span data-stu-id="9fd66-121">[actionResultPart](../resources/actionresultpart.md) collection</span></span>|<span data-ttu-id="9fd66-122">Добавление нескольких участников в команду одним запросом.</span><span class="sxs-lookup"><span data-stu-id="9fd66-122">Add multiple members to the team in a single request.</span></span>|
|[<span data-ttu-id="9fd66-123">Обновление роли участника команды</span><span class="sxs-lookup"><span data-stu-id="9fd66-123">Update team member's role</span></span>](../api/team-update-members.md)|[<span data-ttu-id="9fd66-124">conversationMember</span><span class="sxs-lookup"><span data-stu-id="9fd66-124">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="9fd66-125">Перевод пользователя из категории участников в категорию владельцев или наоборот, из категории владельцев в категорию обычных участников.</span><span class="sxs-lookup"><span data-stu-id="9fd66-125">Change a member to an owner or back to a regular member.</span></span>|
|[<span data-ttu-id="9fd66-126">Удаление участника команды</span><span class="sxs-lookup"><span data-stu-id="9fd66-126">Remove team member</span></span>](../api/team-delete-members.md)|<span data-ttu-id="9fd66-127">Нет</span><span class="sxs-lookup"><span data-stu-id="9fd66-127">None</span></span>|<span data-ttu-id="9fd66-128">Удаление существующего участника из группы.</span><span class="sxs-lookup"><span data-stu-id="9fd66-128">Remove an existing member from the team.</span></span>|
|[<span data-ttu-id="9fd66-129">Перечисление участников канала</span><span class="sxs-lookup"><span data-stu-id="9fd66-129">List channel members</span></span>](../api/channel-list-members.md) | <span data-ttu-id="9fd66-130">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="9fd66-130">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="9fd66-131">Получение списка всех участников канала.</span><span class="sxs-lookup"><span data-stu-id="9fd66-131">Get the list of all members in a channel.</span></span>|
|[<span data-ttu-id="9fd66-132">Получение участника канала</span><span class="sxs-lookup"><span data-stu-id="9fd66-132">Get channel member</span></span>](../api/channel-get-members.md) | <span data-ttu-id="9fd66-133">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="9fd66-133">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="9fd66-134">Получение участника канала.</span><span class="sxs-lookup"><span data-stu-id="9fd66-134">Get a member in a channel.</span></span>|
|[<span data-ttu-id="9fd66-135">Создание участника канала</span><span class="sxs-lookup"><span data-stu-id="9fd66-135">Create channel member</span></span>](../api/channel-post-members.md) | [<span data-ttu-id="9fd66-136">conversationMember</span><span class="sxs-lookup"><span data-stu-id="9fd66-136">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="9fd66-137">Добавление участника в канал.</span><span class="sxs-lookup"><span data-stu-id="9fd66-137">Add a member to a channel.</span></span> <span data-ttu-id="9fd66-138">Поддерживается только для `channel` с типом членства `private`.</span><span class="sxs-lookup"><span data-stu-id="9fd66-138">Only supported for `channel`with membershipType of `private`.</span></span>|
|[<span data-ttu-id="9fd66-139">Обновление роли участника канала</span><span class="sxs-lookup"><span data-stu-id="9fd66-139">Update channel member's role</span></span>](../api/channel-update-members.md) | [<span data-ttu-id="9fd66-140">conversationMember</span><span class="sxs-lookup"><span data-stu-id="9fd66-140">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="9fd66-141">Обновление свойства участника канала.</span><span class="sxs-lookup"><span data-stu-id="9fd66-141">Update the properties of a member of the channel.</span></span> <span data-ttu-id="9fd66-142">Поддерживается только для канала с типом членства `private`.</span><span class="sxs-lookup"><span data-stu-id="9fd66-142">Only supported for channel with membershipType of `private`.</span></span>|
|[<span data-ttu-id="9fd66-143">Удаление участника канала</span><span class="sxs-lookup"><span data-stu-id="9fd66-143">Remove channel member</span></span>](../api/channel-delete-members.md) | <span data-ttu-id="9fd66-144">Нет</span><span class="sxs-lookup"><span data-stu-id="9fd66-144">None</span></span> | <span data-ttu-id="9fd66-145">Удаление участника канала.</span><span class="sxs-lookup"><span data-stu-id="9fd66-145">Delete a member from a channel.</span></span> <span data-ttu-id="9fd66-146">Поддерживается, только если параметру `channelType` присвоено значение `private`.</span><span class="sxs-lookup"><span data-stu-id="9fd66-146">Only supported for `channelType` of `private`.</span></span>|
|[<span data-ttu-id="9fd66-147">Перечисление участников чата</span><span class="sxs-lookup"><span data-stu-id="9fd66-147">List chat members</span></span>](../api/chat-list-members.md) | <span data-ttu-id="9fd66-148">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="9fd66-148">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="9fd66-149">Получение списка всех участников чата.</span><span class="sxs-lookup"><span data-stu-id="9fd66-149">Get the list of all members in a chat.</span></span>|
|[<span data-ttu-id="9fd66-150">Получение участника чата</span><span class="sxs-lookup"><span data-stu-id="9fd66-150">Get chat member</span></span>](../api/chat-get-members.md) | [<span data-ttu-id="9fd66-151">conversationMember</span><span class="sxs-lookup"><span data-stu-id="9fd66-151">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="9fd66-152">Получение участника чата.</span><span class="sxs-lookup"><span data-stu-id="9fd66-152">Get a member in a chat.</span></span>|
|[<span data-ttu-id="9fd66-153">Добавление участника в чат</span><span class="sxs-lookup"><span data-stu-id="9fd66-153">Add chat member</span></span>](../api/chat-post-members.md) | <span data-ttu-id="9fd66-154">Заголовок размещения</span><span class="sxs-lookup"><span data-stu-id="9fd66-154">Location header</span></span> | <span data-ttu-id="9fd66-155">Добавление участника в чат.</span><span class="sxs-lookup"><span data-stu-id="9fd66-155">Add a member to a chat.</span></span>| 

## <a name="properties"></a><span data-ttu-id="9fd66-156">Свойства</span><span class="sxs-lookup"><span data-stu-id="9fd66-156">Properties</span></span>

| <span data-ttu-id="9fd66-157">Свойство</span><span class="sxs-lookup"><span data-stu-id="9fd66-157">Property</span></span>   | <span data-ttu-id="9fd66-158">Тип</span><span class="sxs-lookup"><span data-stu-id="9fd66-158">Type</span></span> |<span data-ttu-id="9fd66-159">Описание</span><span class="sxs-lookup"><span data-stu-id="9fd66-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9fd66-160">id</span><span class="sxs-lookup"><span data-stu-id="9fd66-160">id</span></span>| <span data-ttu-id="9fd66-161">String</span><span class="sxs-lookup"><span data-stu-id="9fd66-161">String</span></span> | <span data-ttu-id="9fd66-162">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9fd66-162">Read-only.</span></span> <span data-ttu-id="9fd66-163">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="9fd66-163">Unique ID of the user.</span></span>|
|<span data-ttu-id="9fd66-164">displayName</span><span class="sxs-lookup"><span data-stu-id="9fd66-164">displayName</span></span>| <span data-ttu-id="9fd66-165">String</span><span class="sxs-lookup"><span data-stu-id="9fd66-165">String</span></span> | <span data-ttu-id="9fd66-166">Отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="9fd66-166">The display name of the user.</span></span> |
|<span data-ttu-id="9fd66-167">roles</span><span class="sxs-lookup"><span data-stu-id="9fd66-167">roles</span></span>| <span data-ttu-id="9fd66-168">Набор строк</span><span class="sxs-lookup"><span data-stu-id="9fd66-168">String collection</span></span> | <span data-ttu-id="9fd66-169">Роли этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="9fd66-169">The roles for that user.</span></span> |
|<span data-ttu-id="9fd66-170">userId</span><span class="sxs-lookup"><span data-stu-id="9fd66-170">userId</span></span>| <span data-ttu-id="9fd66-171">String</span><span class="sxs-lookup"><span data-stu-id="9fd66-171">String</span></span> | <span data-ttu-id="9fd66-172">GUID пользователя.</span><span class="sxs-lookup"><span data-stu-id="9fd66-172">The GUID of the user.</span></span> |
|<span data-ttu-id="9fd66-173">email</span><span class="sxs-lookup"><span data-stu-id="9fd66-173">email</span></span>| <span data-ttu-id="9fd66-174">String</span><span class="sxs-lookup"><span data-stu-id="9fd66-174">String</span></span>  | <span data-ttu-id="9fd66-175">Электронный адрес пользователя.</span><span class="sxs-lookup"><span data-stu-id="9fd66-175">The email address of the user.</span></span> |
|<span data-ttu-id="9fd66-176">tenantId</span><span class="sxs-lookup"><span data-stu-id="9fd66-176">tenantId</span></span>| <span data-ttu-id="9fd66-177">string</span><span class="sxs-lookup"><span data-stu-id="9fd66-177">string</span></span>  | <span data-ttu-id="9fd66-178">ИД клиента, которому принадлежит пользователь Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9fd66-178">TenantId which the Azure AD user belongs to.</span></span> |
|<span data-ttu-id="9fd66-179">visibleHistoryStartDateTime</span><span class="sxs-lookup"><span data-stu-id="9fd66-179">visibleHistoryStartDateTime</span></span>| <span data-ttu-id="9fd66-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9fd66-180">DateTimeOffset</span></span>  | <span data-ttu-id="9fd66-181">Метка времени, обозначающая, насколько глубоко участник беседы может видеть историю беседы.</span><span class="sxs-lookup"><span data-stu-id="9fd66-181">The timestamp denoting how far back a conversation's history is shared with the conversation member.</span></span> <span data-ttu-id="9fd66-182">Это свойство можно задать только для участников чата.</span><span class="sxs-lookup"><span data-stu-id="9fd66-182">This property is settable only for members of a chat.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9fd66-183">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9fd66-183">JSON representation</span></span>

<span data-ttu-id="9fd66-184">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9fd66-184">The following is a JSON representation of the resource.</span></span>

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
