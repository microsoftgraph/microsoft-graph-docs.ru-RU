---
title: Тип ресурса conversationMember
description: Представляет пользователя в беседе.
localization_priority: Normal
author: laujan
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 14a70fcc6492ec143fa2f4e892438805d3526d60
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777722"
---
# <a name="conversationmember-resource-type"></a><span data-ttu-id="d2d70-103">Тип ресурса conversationMember</span><span class="sxs-lookup"><span data-stu-id="d2d70-103">conversationMember resource type</span></span>

<span data-ttu-id="d2d70-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2d70-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d2d70-105">Представляет пользователя в [команде,](team.md) [канале](channel.md)или [чате.](chat.md)</span><span class="sxs-lookup"><span data-stu-id="d2d70-105">Represents a user in a [team](team.md), a [channel](channel.md), or a [chat](chat.md).</span></span>
<span data-ttu-id="d2d70-106">См. [также aadUserConversationMember](aaduserconversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="d2d70-106">See also [aadUserConversationMember](aaduserconversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="d2d70-107">Методы</span><span class="sxs-lookup"><span data-stu-id="d2d70-107">Methods</span></span>

| <span data-ttu-id="d2d70-108">Метод</span><span class="sxs-lookup"><span data-stu-id="d2d70-108">Method</span></span>       | <span data-ttu-id="d2d70-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d2d70-109">Return Type</span></span>  |<span data-ttu-id="d2d70-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d2d70-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d2d70-111">Список участников группы</span><span class="sxs-lookup"><span data-stu-id="d2d70-111">List team members</span></span>](../api/team-list-members.md)|<span data-ttu-id="d2d70-112">Коллекция [conversationMember](../resources/conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="d2d70-112">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="d2d70-113">Получение списка участников группы.</span><span class="sxs-lookup"><span data-stu-id="d2d70-113">Get the list of members in the team.</span></span>|
|[<span data-ttu-id="d2d70-114">Добавление участника в команду</span><span class="sxs-lookup"><span data-stu-id="d2d70-114">Add team member</span></span>](../api/team-post-members.md)|[<span data-ttu-id="d2d70-115">conversationMember</span><span class="sxs-lookup"><span data-stu-id="d2d70-115">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="d2d70-116">Добавление нового участника в группу.</span><span class="sxs-lookup"><span data-stu-id="d2d70-116">Add a new member to the team.</span></span>|
|[<span data-ttu-id="d2d70-117">Получение участника группы</span><span class="sxs-lookup"><span data-stu-id="d2d70-117">Get team member</span></span>](../api/team-get-members.md) | <span data-ttu-id="d2d70-118">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="d2d70-118">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="d2d70-119">Получение участника группы.</span><span class="sxs-lookup"><span data-stu-id="d2d70-119">Get a member in the team.</span></span>|
|[<span data-ttu-id="d2d70-120">Обновление роли участника команды</span><span class="sxs-lookup"><span data-stu-id="d2d70-120">Update team member's role</span></span>](../api/team-update-members.md)|[<span data-ttu-id="d2d70-121">conversationMember</span><span class="sxs-lookup"><span data-stu-id="d2d70-121">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="d2d70-122">Перевод пользователя из категории участников в категорию владельцев или наоборот, из категории владельцев в категорию обычных участников.</span><span class="sxs-lookup"><span data-stu-id="d2d70-122">Change a member to an owner or back to a regular member.</span></span>|
|[<span data-ttu-id="d2d70-123">Удаление участника группы</span><span class="sxs-lookup"><span data-stu-id="d2d70-123">Remove team member</span></span>](../api/team-delete-members.md)|<span data-ttu-id="d2d70-124">Нет</span><span class="sxs-lookup"><span data-stu-id="d2d70-124">None</span></span>|<span data-ttu-id="d2d70-125">Удаление существующего участника из группы.</span><span class="sxs-lookup"><span data-stu-id="d2d70-125">Remove an existing member from the team.</span></span>|
|[<span data-ttu-id="d2d70-126">Перечисление участников канала</span><span class="sxs-lookup"><span data-stu-id="d2d70-126">List channel members</span></span>](../api/channel-list-members.md) | <span data-ttu-id="d2d70-127">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="d2d70-127">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="d2d70-128">Получение списка всех участников канала.</span><span class="sxs-lookup"><span data-stu-id="d2d70-128">Get the list of all members in a channel.</span></span>|
|[<span data-ttu-id="d2d70-129">Добавление участника канала</span><span class="sxs-lookup"><span data-stu-id="d2d70-129">Add channel member</span></span>](../api/channel-post-members.md) | [<span data-ttu-id="d2d70-130">conversationMember</span><span class="sxs-lookup"><span data-stu-id="d2d70-130">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="d2d70-131">Добавление участника в канал.</span><span class="sxs-lookup"><span data-stu-id="d2d70-131">Add a member to a channel.</span></span> <span data-ttu-id="d2d70-132">Поддерживается только для `channel` с типом членства `private`.</span><span class="sxs-lookup"><span data-stu-id="d2d70-132">Only supported for `channel` with membershipType of `private`.</span></span>|
|[<span data-ttu-id="d2d70-133">Получение участника канала</span><span class="sxs-lookup"><span data-stu-id="d2d70-133">Get channel member</span></span>](../api/channel-get-members.md) | <span data-ttu-id="d2d70-134">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="d2d70-134">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="d2d70-135">Получение участника канала.</span><span class="sxs-lookup"><span data-stu-id="d2d70-135">Get a member in a channel.</span></span>|
|[<span data-ttu-id="d2d70-136">Обновление роли участника канала</span><span class="sxs-lookup"><span data-stu-id="d2d70-136">Update channel member's role</span></span>](../api/channel-update-members.md) | [<span data-ttu-id="d2d70-137">conversationMember</span><span class="sxs-lookup"><span data-stu-id="d2d70-137">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="d2d70-138">Обновление свойства участника канала.</span><span class="sxs-lookup"><span data-stu-id="d2d70-138">Update the properties of a member of the channel.</span></span> <span data-ttu-id="d2d70-139">Поддерживается только для канала с типом членства `private`.</span><span class="sxs-lookup"><span data-stu-id="d2d70-139">Only supported for channel with membershipType of `private`.</span></span>|
|[<span data-ttu-id="d2d70-140">Удаление участника канала</span><span class="sxs-lookup"><span data-stu-id="d2d70-140">Remove channel member</span></span>](../api/channel-delete-members.md) | <span data-ttu-id="d2d70-141">Нет</span><span class="sxs-lookup"><span data-stu-id="d2d70-141">None</span></span> | <span data-ttu-id="d2d70-142">Удаление участника канала.</span><span class="sxs-lookup"><span data-stu-id="d2d70-142">Delete a member from a channel.</span></span> <span data-ttu-id="d2d70-143">Поддерживается, только если параметру `channelType` присвоено значение `private`.</span><span class="sxs-lookup"><span data-stu-id="d2d70-143">Only supported for `channelType` of `private`.</span></span>|
|[<span data-ttu-id="d2d70-144">Перечисление участников чата</span><span class="sxs-lookup"><span data-stu-id="d2d70-144">List chat members</span></span>](../api/chat-list-members.md) | <span data-ttu-id="d2d70-145">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="d2d70-145">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="d2d70-146">Получение списка всех участников чата.</span><span class="sxs-lookup"><span data-stu-id="d2d70-146">Get the list of all members in a chat.</span></span>|
|[<span data-ttu-id="d2d70-147">Добавление участника в чат</span><span class="sxs-lookup"><span data-stu-id="d2d70-147">Add chat member</span></span>](../api/chat-post-members.md) | <span data-ttu-id="d2d70-148">Заголовок размещения</span><span class="sxs-lookup"><span data-stu-id="d2d70-148">Location header</span></span> | <span data-ttu-id="d2d70-149">Добавление участника в чат.</span><span class="sxs-lookup"><span data-stu-id="d2d70-149">Add a member to a chat.</span></span>| 
|[<span data-ttu-id="d2d70-150">Получение участника чата</span><span class="sxs-lookup"><span data-stu-id="d2d70-150">Get chat member</span></span>](../api/chat-get-members.md) | [<span data-ttu-id="d2d70-151">conversationMember</span><span class="sxs-lookup"><span data-stu-id="d2d70-151">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="d2d70-152">Получение участника чата.</span><span class="sxs-lookup"><span data-stu-id="d2d70-152">Get a member in a chat.</span></span>|
|[<span data-ttu-id="d2d70-153">Удаление участника чата</span><span class="sxs-lookup"><span data-stu-id="d2d70-153">Remove chat member</span></span>](../api/chat-delete-members.md) | <span data-ttu-id="d2d70-154">Нет</span><span class="sxs-lookup"><span data-stu-id="d2d70-154">None</span></span> | <span data-ttu-id="d2d70-155">Удаление участника из чата.</span><span class="sxs-lookup"><span data-stu-id="d2d70-155">Remove a member from a chat.</span></span>| 

## <a name="properties"></a><span data-ttu-id="d2d70-156">Свойства</span><span class="sxs-lookup"><span data-stu-id="d2d70-156">Properties</span></span>

| <span data-ttu-id="d2d70-157">Свойство</span><span class="sxs-lookup"><span data-stu-id="d2d70-157">Property</span></span>   | <span data-ttu-id="d2d70-158">Тип</span><span class="sxs-lookup"><span data-stu-id="d2d70-158">Type</span></span> |<span data-ttu-id="d2d70-159">Описание</span><span class="sxs-lookup"><span data-stu-id="d2d70-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d2d70-160">id</span><span class="sxs-lookup"><span data-stu-id="d2d70-160">id</span></span>|<span data-ttu-id="d2d70-161">String</span><span class="sxs-lookup"><span data-stu-id="d2d70-161">String</span></span>| <span data-ttu-id="d2d70-162">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d2d70-162">Read-only.</span></span> <span data-ttu-id="d2d70-163">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="d2d70-163">Unique ID of the user.</span></span>|
|<span data-ttu-id="d2d70-164">displayName</span><span class="sxs-lookup"><span data-stu-id="d2d70-164">displayName</span></span>| <span data-ttu-id="d2d70-165">string</span><span class="sxs-lookup"><span data-stu-id="d2d70-165">string</span></span> | <span data-ttu-id="d2d70-166">Отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="d2d70-166">The display name of the user.</span></span> |
|<span data-ttu-id="d2d70-167">roles</span><span class="sxs-lookup"><span data-stu-id="d2d70-167">roles</span></span>| <span data-ttu-id="d2d70-168">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d2d70-168">string collection</span></span> | <span data-ttu-id="d2d70-169">Роли этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="d2d70-169">The roles for that user.</span></span> |
|<span data-ttu-id="d2d70-170">visibleHistoryStartDateTime</span><span class="sxs-lookup"><span data-stu-id="d2d70-170">visibleHistoryStartDateTime</span></span>| <span data-ttu-id="d2d70-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2d70-171">DateTimeOffset</span></span> | <span data-ttu-id="d2d70-172">Метка времени, обозначающая, насколько глубоко участник беседы может видеть историю беседы.</span><span class="sxs-lookup"><span data-stu-id="d2d70-172">The timestamp denoting how far back a conversation's history is shared with the conversation member.</span></span> <span data-ttu-id="d2d70-173">Это свойство можно задать только для участников чата.</span><span class="sxs-lookup"><span data-stu-id="d2d70-173">This property is settable only for members of a chat.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d2d70-174">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d2d70-174">JSON representation</span></span>

<span data-ttu-id="d2d70-175">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d2d70-175">The following is a JSON representation of the resource.</span></span>

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

