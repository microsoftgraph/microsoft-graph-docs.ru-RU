---
title: Тип ресурса aadUserConversationMember
description: Представляет пользователя Azure Active Directory в чате или канале.
localization_priority: Priority
author: akjo
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 6632dad56f76b4747285eb1df9f69046b1de3cc1
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060298"
---
# <a name="aaduserconversationmember-resource-type"></a><span data-ttu-id="9975d-103">Тип ресурса aadUserConversationMember</span><span class="sxs-lookup"><span data-stu-id="9975d-103">aadUserConversationMember resource type</span></span>

<span data-ttu-id="9975d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9975d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9975d-105">Представляет пользователя Azure Active Directory в [команде](team.md), [канале](channel.md) или [чате](chat.md).</span><span class="sxs-lookup"><span data-stu-id="9975d-105">Represents an Azure Active Directory user in a [team](team.md), a [channel](channel.md), or a [chat](chat.md).</span></span>
<span data-ttu-id="9975d-106">Этот тип наследуется от [conversationMember](conversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="9975d-106">This type inherits from [conversationMember](conversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="9975d-107">Методы</span><span class="sxs-lookup"><span data-stu-id="9975d-107">Methods</span></span>

| <span data-ttu-id="9975d-108">Метод</span><span class="sxs-lookup"><span data-stu-id="9975d-108">Method</span></span>       | <span data-ttu-id="9975d-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9975d-109">Return Type</span></span>  |<span data-ttu-id="9975d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9975d-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9975d-111">Список участников группы</span><span class="sxs-lookup"><span data-stu-id="9975d-111">List team members</span></span>](../api/team-list-members.md)|<span data-ttu-id="9975d-112">Коллекция [conversationMember](../resources/conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="9975d-112">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="9975d-113">Получение списка участников группы.</span><span class="sxs-lookup"><span data-stu-id="9975d-113">Get the list of members in the team.</span></span>|
|[<span data-ttu-id="9975d-114">Добавление участника в команду</span><span class="sxs-lookup"><span data-stu-id="9975d-114">Add team member</span></span>](../api/team-post-members.md)|[<span data-ttu-id="9975d-115">conversationMember</span><span class="sxs-lookup"><span data-stu-id="9975d-115">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="9975d-116">Добавление нового участника в группу.</span><span class="sxs-lookup"><span data-stu-id="9975d-116">Add a new member to the team.</span></span>|
|[<span data-ttu-id="9975d-117">Получение участника группы</span><span class="sxs-lookup"><span data-stu-id="9975d-117">Get team member</span></span>](../api/team-get-members.md) | <span data-ttu-id="9975d-118">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="9975d-118">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="9975d-119">Получение участника группы.</span><span class="sxs-lookup"><span data-stu-id="9975d-119">Get a member in the team.</span></span>|
|[<span data-ttu-id="9975d-120">Обновление роли участника команды</span><span class="sxs-lookup"><span data-stu-id="9975d-120">Update team member's role</span></span>](../api/team-update-members.md)|[<span data-ttu-id="9975d-121">conversationMember</span><span class="sxs-lookup"><span data-stu-id="9975d-121">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="9975d-122">Перевод пользователя из категории участников в категорию владельцев или наоборот, из категории владельцев в категорию обычных участников.</span><span class="sxs-lookup"><span data-stu-id="9975d-122">Change a member to an owner or back to a regular member.</span></span>|
|[<span data-ttu-id="9975d-123">Удаление участника группы</span><span class="sxs-lookup"><span data-stu-id="9975d-123">Remove team member</span></span>](../api/team-delete-members.md)|<span data-ttu-id="9975d-124">Нет</span><span class="sxs-lookup"><span data-stu-id="9975d-124">None</span></span>|<span data-ttu-id="9975d-125">Удаление существующего участника из группы.</span><span class="sxs-lookup"><span data-stu-id="9975d-125">Remove an existing member from the team.</span></span>|
|[<span data-ttu-id="9975d-126">Перечисление участников канала</span><span class="sxs-lookup"><span data-stu-id="9975d-126">List channel members</span></span>](../api/channel-list-members.md) | <span data-ttu-id="9975d-127">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="9975d-127">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="9975d-128">Получение списка всех участников канала.</span><span class="sxs-lookup"><span data-stu-id="9975d-128">Get the list of all members in a channel.</span></span>|
|[<span data-ttu-id="9975d-129">Добавление участника канала</span><span class="sxs-lookup"><span data-stu-id="9975d-129">Add channel member</span></span>](../api/channel-post-members.md) | [<span data-ttu-id="9975d-130">conversationMember</span><span class="sxs-lookup"><span data-stu-id="9975d-130">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="9975d-131">Добавление участника в канал.</span><span class="sxs-lookup"><span data-stu-id="9975d-131">Add a member to a channel.</span></span> <span data-ttu-id="9975d-132">Поддерживается только для `channel` с типом членства `private`.</span><span class="sxs-lookup"><span data-stu-id="9975d-132">Only supported for `channel` with membershipType of `private`.</span></span>|
|[<span data-ttu-id="9975d-133">Получение участника канала</span><span class="sxs-lookup"><span data-stu-id="9975d-133">Get channel member</span></span>](../api/channel-get-members.md) | <span data-ttu-id="9975d-134">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="9975d-134">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="9975d-135">Получение участника канала.</span><span class="sxs-lookup"><span data-stu-id="9975d-135">Get a member in a channel.</span></span>|
|[<span data-ttu-id="9975d-136">Обновление роли участника канала</span><span class="sxs-lookup"><span data-stu-id="9975d-136">Update channel member's role</span></span>](../api/channel-update-members.md) | [<span data-ttu-id="9975d-137">conversationMember</span><span class="sxs-lookup"><span data-stu-id="9975d-137">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="9975d-138">Обновление свойства участника канала.</span><span class="sxs-lookup"><span data-stu-id="9975d-138">Update the properties of a member of the channel.</span></span> <span data-ttu-id="9975d-139">Поддерживается только для канала с типом членства `private`.</span><span class="sxs-lookup"><span data-stu-id="9975d-139">Only supported for channel with membershipType of `private`.</span></span>|
|[<span data-ttu-id="9975d-140">Удаление участника канала</span><span class="sxs-lookup"><span data-stu-id="9975d-140">Remove channel member</span></span>](../api/channel-delete-members.md) | <span data-ttu-id="9975d-141">Нет</span><span class="sxs-lookup"><span data-stu-id="9975d-141">None</span></span> | <span data-ttu-id="9975d-142">Удаление участника канала.</span><span class="sxs-lookup"><span data-stu-id="9975d-142">Delete a member from a channel.</span></span> <span data-ttu-id="9975d-143">Поддерживается, только если параметру `channelType` присвоено значение `private`.</span><span class="sxs-lookup"><span data-stu-id="9975d-143">Only supported for `channelType` of `private`.</span></span>|
|[<span data-ttu-id="9975d-144">Перечисление участников чата</span><span class="sxs-lookup"><span data-stu-id="9975d-144">List chat members</span></span>](../api/chat-list-members.md) | <span data-ttu-id="9975d-145">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="9975d-145">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="9975d-146">Получение списка всех участников чата.</span><span class="sxs-lookup"><span data-stu-id="9975d-146">Get the list of all members in a chat.</span></span>|
|[<span data-ttu-id="9975d-147">Добавление участника в чат</span><span class="sxs-lookup"><span data-stu-id="9975d-147">Add chat member</span></span>](../api/chat-post-members.md) | <span data-ttu-id="9975d-148">Заголовок размещения</span><span class="sxs-lookup"><span data-stu-id="9975d-148">Location header</span></span> | <span data-ttu-id="9975d-149">Добавление участника в чат.</span><span class="sxs-lookup"><span data-stu-id="9975d-149">Add a member to a chat.</span></span>| 
|[<span data-ttu-id="9975d-150">Получение участника чата</span><span class="sxs-lookup"><span data-stu-id="9975d-150">Get chat member</span></span>](../api/chat-get-members.md) | [<span data-ttu-id="9975d-151">conversationMember</span><span class="sxs-lookup"><span data-stu-id="9975d-151">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="9975d-152">Получение участника чата.</span><span class="sxs-lookup"><span data-stu-id="9975d-152">Get a member in a chat.</span></span>|
|[<span data-ttu-id="9975d-153">Удаление участника чата</span><span class="sxs-lookup"><span data-stu-id="9975d-153">Remove chat member</span></span>](../api/chat-delete-members.md) | <span data-ttu-id="9975d-154">Нет</span><span class="sxs-lookup"><span data-stu-id="9975d-154">None</span></span> | <span data-ttu-id="9975d-155">Удаление участника из чата.</span><span class="sxs-lookup"><span data-stu-id="9975d-155">Remove a member from a chat.</span></span>| 

## <a name="properties"></a><span data-ttu-id="9975d-156">Свойства</span><span class="sxs-lookup"><span data-stu-id="9975d-156">Properties</span></span>

| <span data-ttu-id="9975d-157">Свойство</span><span class="sxs-lookup"><span data-stu-id="9975d-157">Property</span></span>   | <span data-ttu-id="9975d-158">Тип</span><span class="sxs-lookup"><span data-stu-id="9975d-158">Type</span></span> |<span data-ttu-id="9975d-159">Описание</span><span class="sxs-lookup"><span data-stu-id="9975d-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9975d-160">id</span><span class="sxs-lookup"><span data-stu-id="9975d-160">id</span></span>|<span data-ttu-id="9975d-161">String</span><span class="sxs-lookup"><span data-stu-id="9975d-161">String</span></span>| <span data-ttu-id="9975d-p105">Только для чтения. Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="9975d-p105">Read-only. Unique ID of the user.</span></span>|
|<span data-ttu-id="9975d-164">displayName</span><span class="sxs-lookup"><span data-stu-id="9975d-164">displayName</span></span>| <span data-ttu-id="9975d-165">string</span><span class="sxs-lookup"><span data-stu-id="9975d-165">string</span></span> | <span data-ttu-id="9975d-166">Отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="9975d-166">The display name of the user.</span></span> |
|<span data-ttu-id="9975d-167">roles</span><span class="sxs-lookup"><span data-stu-id="9975d-167">roles</span></span>| <span data-ttu-id="9975d-168">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9975d-168">string collection</span></span> | <span data-ttu-id="9975d-169">Роли этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="9975d-169">The roles for that user.</span></span> |
|<span data-ttu-id="9975d-170">userId</span><span class="sxs-lookup"><span data-stu-id="9975d-170">userId</span></span>| <span data-ttu-id="9975d-171">строка</span><span class="sxs-lookup"><span data-stu-id="9975d-171">string</span></span> | <span data-ttu-id="9975d-172">GUID пользователя.</span><span class="sxs-lookup"><span data-stu-id="9975d-172">The guid of the user.</span></span> |
|<span data-ttu-id="9975d-173">email</span><span class="sxs-lookup"><span data-stu-id="9975d-173">email</span></span>| <span data-ttu-id="9975d-174">строка</span><span class="sxs-lookup"><span data-stu-id="9975d-174">string</span></span>  | <span data-ttu-id="9975d-175">Электронный адрес пользователя.</span><span class="sxs-lookup"><span data-stu-id="9975d-175">The email address of the user.</span></span> |
|<span data-ttu-id="9975d-176">tenantId</span><span class="sxs-lookup"><span data-stu-id="9975d-176">tenantId</span></span>| <span data-ttu-id="9975d-177">string</span><span class="sxs-lookup"><span data-stu-id="9975d-177">string</span></span>  | <span data-ttu-id="9975d-178">ИД клиента, которому принадлежит пользователь Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9975d-178">TenantId which the Azure AD user belongs to.</span></span> |
|<span data-ttu-id="9975d-179">visibleHistoryStartDateTime</span><span class="sxs-lookup"><span data-stu-id="9975d-179">visibleHistoryStartDateTime</span></span>| <span data-ttu-id="9975d-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9975d-180">DateTimeOffset</span></span>  | <span data-ttu-id="9975d-181">Метка времени, обозначающая, насколько глубоко участник беседы может видеть историю беседы.</span><span class="sxs-lookup"><span data-stu-id="9975d-181">The timestamp denoting how far back a conversation's history is shared with the conversation member.</span></span> <span data-ttu-id="9975d-182">Это свойство можно задать только для участников чата.</span><span class="sxs-lookup"><span data-stu-id="9975d-182">This property is settable only for members of a chat.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9975d-183">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9975d-183">JSON representation</span></span>

<span data-ttu-id="9975d-184">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9975d-184">The following is a JSON representation of the resource.</span></span>

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
  "id": "string (identifier)",
  "displayName" : "string",
  "visibleHistoryStartDateTime": "string (timestamp)",
  "roles" : ["string"],
  "userId" : "string",
  "email" : "string",
  "tenantId": "string"
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

