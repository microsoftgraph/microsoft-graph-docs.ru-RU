---
title: Тип ресурса conversationMember
description: Представляет пользователя в беседе.
localization_priority: Normal
author: akjo
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c82f7e1ec927c73ad41771fc00e013dda1755a80
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060303"
---
# <a name="conversationmember-resource-type"></a><span data-ttu-id="91f8e-103">Тип ресурса conversationMember</span><span class="sxs-lookup"><span data-stu-id="91f8e-103">conversationMember resource type</span></span>

<span data-ttu-id="91f8e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91f8e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="91f8e-105">Представляет пользователя в [команде,](team.md) [канале](channel.md)или [чате.](chat.md)</span><span class="sxs-lookup"><span data-stu-id="91f8e-105">Represents a user in a [team](team.md), a [channel](channel.md), or a [chat](chat.md).</span></span>
<span data-ttu-id="91f8e-106">См. [также aadUserConversationMember](aaduserconversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="91f8e-106">See also [aadUserConversationMember](aaduserconversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="91f8e-107">Методы</span><span class="sxs-lookup"><span data-stu-id="91f8e-107">Methods</span></span>

| <span data-ttu-id="91f8e-108">Метод</span><span class="sxs-lookup"><span data-stu-id="91f8e-108">Method</span></span>       | <span data-ttu-id="91f8e-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="91f8e-109">Return Type</span></span>  |<span data-ttu-id="91f8e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="91f8e-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="91f8e-111">Список участников группы</span><span class="sxs-lookup"><span data-stu-id="91f8e-111">List team members</span></span>](../api/team-list-members.md)|<span data-ttu-id="91f8e-112">Коллекция [conversationMember](../resources/conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="91f8e-112">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="91f8e-113">Получение списка участников группы.</span><span class="sxs-lookup"><span data-stu-id="91f8e-113">Get the list of members in the team.</span></span>|
|[<span data-ttu-id="91f8e-114">Добавление участника в команду</span><span class="sxs-lookup"><span data-stu-id="91f8e-114">Add team member</span></span>](../api/team-post-members.md)|[<span data-ttu-id="91f8e-115">conversationMember</span><span class="sxs-lookup"><span data-stu-id="91f8e-115">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="91f8e-116">Добавление нового участника в группу.</span><span class="sxs-lookup"><span data-stu-id="91f8e-116">Add a new member to the team.</span></span>|
|[<span data-ttu-id="91f8e-117">Получение участника группы</span><span class="sxs-lookup"><span data-stu-id="91f8e-117">Get team member</span></span>](../api/team-get-members.md) | <span data-ttu-id="91f8e-118">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="91f8e-118">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="91f8e-119">Получение участника группы.</span><span class="sxs-lookup"><span data-stu-id="91f8e-119">Get a member in the team.</span></span>|
|[<span data-ttu-id="91f8e-120">Обновление роли участника команды</span><span class="sxs-lookup"><span data-stu-id="91f8e-120">Update team member's role</span></span>](../api/team-update-members.md)|[<span data-ttu-id="91f8e-121">conversationMember</span><span class="sxs-lookup"><span data-stu-id="91f8e-121">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="91f8e-122">Перевод пользователя из категории участников в категорию владельцев или наоборот, из категории владельцев в категорию обычных участников.</span><span class="sxs-lookup"><span data-stu-id="91f8e-122">Change a member to an owner or back to a regular member.</span></span>|
|[<span data-ttu-id="91f8e-123">Удаление участника группы</span><span class="sxs-lookup"><span data-stu-id="91f8e-123">Remove team member</span></span>](../api/team-delete-members.md)|<span data-ttu-id="91f8e-124">Нет</span><span class="sxs-lookup"><span data-stu-id="91f8e-124">None</span></span>|<span data-ttu-id="91f8e-125">Удаление существующего участника из группы.</span><span class="sxs-lookup"><span data-stu-id="91f8e-125">Remove an existing member from the team.</span></span>|
|[<span data-ttu-id="91f8e-126">Перечисление участников канала</span><span class="sxs-lookup"><span data-stu-id="91f8e-126">List channel members</span></span>](../api/channel-list-members.md) | <span data-ttu-id="91f8e-127">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="91f8e-127">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="91f8e-128">Получение списка всех участников канала.</span><span class="sxs-lookup"><span data-stu-id="91f8e-128">Get the list of all members in a channel.</span></span>|
|[<span data-ttu-id="91f8e-129">Добавление участника канала</span><span class="sxs-lookup"><span data-stu-id="91f8e-129">Add channel member</span></span>](../api/channel-post-members.md) | [<span data-ttu-id="91f8e-130">conversationMember</span><span class="sxs-lookup"><span data-stu-id="91f8e-130">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="91f8e-131">Добавление участника в канал.</span><span class="sxs-lookup"><span data-stu-id="91f8e-131">Add a member to a channel.</span></span> <span data-ttu-id="91f8e-132">Поддерживается только для `channel` с типом членства `private`.</span><span class="sxs-lookup"><span data-stu-id="91f8e-132">Only supported for `channel` with membershipType of `private`.</span></span>|
|[<span data-ttu-id="91f8e-133">Получение участника канала</span><span class="sxs-lookup"><span data-stu-id="91f8e-133">Get channel member</span></span>](../api/channel-get-members.md) | <span data-ttu-id="91f8e-134">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="91f8e-134">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="91f8e-135">Получение участника канала.</span><span class="sxs-lookup"><span data-stu-id="91f8e-135">Get a member in a channel.</span></span>|
|[<span data-ttu-id="91f8e-136">Обновление роли участника канала</span><span class="sxs-lookup"><span data-stu-id="91f8e-136">Update channel member's role</span></span>](../api/channel-update-members.md) | [<span data-ttu-id="91f8e-137">conversationMember</span><span class="sxs-lookup"><span data-stu-id="91f8e-137">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="91f8e-138">Обновление свойства участника канала.</span><span class="sxs-lookup"><span data-stu-id="91f8e-138">Update the properties of a member of the channel.</span></span> <span data-ttu-id="91f8e-139">Поддерживается только для канала с типом членства `private`.</span><span class="sxs-lookup"><span data-stu-id="91f8e-139">Only supported for channel with membershipType of `private`.</span></span>|
|[<span data-ttu-id="91f8e-140">Удаление участника канала</span><span class="sxs-lookup"><span data-stu-id="91f8e-140">Remove channel member</span></span>](../api/channel-delete-members.md) | <span data-ttu-id="91f8e-141">Нет</span><span class="sxs-lookup"><span data-stu-id="91f8e-141">None</span></span> | <span data-ttu-id="91f8e-142">Удаление участника канала.</span><span class="sxs-lookup"><span data-stu-id="91f8e-142">Delete a member from a channel.</span></span> <span data-ttu-id="91f8e-143">Поддерживается, только если параметру `channelType` присвоено значение `private`.</span><span class="sxs-lookup"><span data-stu-id="91f8e-143">Only supported for `channelType` of `private`.</span></span>|
|[<span data-ttu-id="91f8e-144">Перечисление участников чата</span><span class="sxs-lookup"><span data-stu-id="91f8e-144">List chat members</span></span>](../api/chat-list-members.md) | <span data-ttu-id="91f8e-145">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="91f8e-145">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="91f8e-146">Получение списка всех участников чата.</span><span class="sxs-lookup"><span data-stu-id="91f8e-146">Get the list of all members in a chat.</span></span>|
|[<span data-ttu-id="91f8e-147">Добавление участника в чат</span><span class="sxs-lookup"><span data-stu-id="91f8e-147">Add chat member</span></span>](../api/chat-post-members.md) | <span data-ttu-id="91f8e-148">Заголовок размещения</span><span class="sxs-lookup"><span data-stu-id="91f8e-148">Location header</span></span> | <span data-ttu-id="91f8e-149">Добавление участника в чат.</span><span class="sxs-lookup"><span data-stu-id="91f8e-149">Add a member to a chat.</span></span>| 
|[<span data-ttu-id="91f8e-150">Получение участника чата</span><span class="sxs-lookup"><span data-stu-id="91f8e-150">Get chat member</span></span>](../api/chat-get-members.md) | [<span data-ttu-id="91f8e-151">conversationMember</span><span class="sxs-lookup"><span data-stu-id="91f8e-151">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="91f8e-152">Получение участника чата.</span><span class="sxs-lookup"><span data-stu-id="91f8e-152">Get a member in a chat.</span></span>|
|[<span data-ttu-id="91f8e-153">Удаление участника чата</span><span class="sxs-lookup"><span data-stu-id="91f8e-153">Remove chat member</span></span>](../api/chat-delete-members.md) | <span data-ttu-id="91f8e-154">Нет</span><span class="sxs-lookup"><span data-stu-id="91f8e-154">None</span></span> | <span data-ttu-id="91f8e-155">Удаление участника из чата.</span><span class="sxs-lookup"><span data-stu-id="91f8e-155">Remove a member from a chat.</span></span>| 

## <a name="properties"></a><span data-ttu-id="91f8e-156">Свойства</span><span class="sxs-lookup"><span data-stu-id="91f8e-156">Properties</span></span>

| <span data-ttu-id="91f8e-157">Свойство</span><span class="sxs-lookup"><span data-stu-id="91f8e-157">Property</span></span>   | <span data-ttu-id="91f8e-158">Тип</span><span class="sxs-lookup"><span data-stu-id="91f8e-158">Type</span></span> |<span data-ttu-id="91f8e-159">Описание</span><span class="sxs-lookup"><span data-stu-id="91f8e-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="91f8e-160">id</span><span class="sxs-lookup"><span data-stu-id="91f8e-160">id</span></span>|<span data-ttu-id="91f8e-161">String</span><span class="sxs-lookup"><span data-stu-id="91f8e-161">String</span></span>| <span data-ttu-id="91f8e-162">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="91f8e-162">Read-only.</span></span> <span data-ttu-id="91f8e-163">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="91f8e-163">Unique ID of the user.</span></span>|
|<span data-ttu-id="91f8e-164">displayName</span><span class="sxs-lookup"><span data-stu-id="91f8e-164">displayName</span></span>| <span data-ttu-id="91f8e-165">string</span><span class="sxs-lookup"><span data-stu-id="91f8e-165">string</span></span> | <span data-ttu-id="91f8e-166">Отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="91f8e-166">The display name of the user.</span></span> |
|<span data-ttu-id="91f8e-167">roles</span><span class="sxs-lookup"><span data-stu-id="91f8e-167">roles</span></span>| <span data-ttu-id="91f8e-168">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="91f8e-168">string collection</span></span> | <span data-ttu-id="91f8e-169">Роли этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="91f8e-169">The roles for that user.</span></span> |
|<span data-ttu-id="91f8e-170">visibleHistoryStartDateTime</span><span class="sxs-lookup"><span data-stu-id="91f8e-170">visibleHistoryStartDateTime</span></span>| <span data-ttu-id="91f8e-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91f8e-171">DateTimeOffset</span></span> | <span data-ttu-id="91f8e-172">Метка времени, обозначающая, насколько глубоко участник беседы может видеть историю беседы.</span><span class="sxs-lookup"><span data-stu-id="91f8e-172">The timestamp denoting how far back a conversation's history is shared with the conversation member.</span></span> <span data-ttu-id="91f8e-173">Это свойство можно задать только для участников чата.</span><span class="sxs-lookup"><span data-stu-id="91f8e-173">This property is settable only for members of a chat.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="91f8e-174">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="91f8e-174">JSON representation</span></span>

<span data-ttu-id="91f8e-175">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="91f8e-175">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.conversationMember",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.conversationMember",
  "id": "String (identifier)",
  "roles": [
    "String"
  ],
  "displayName": "String",
  "visibleHistoryStartDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversationMember resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

