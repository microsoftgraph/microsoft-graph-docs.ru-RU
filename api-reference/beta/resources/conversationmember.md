---
title: Тип ресурса conversationMember
description: Представляет пользователя в беседе.
localization_priority: Normal
author: akjo
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 679ab696c0f5752d8e59a2cb9de560c11bcc4ca9
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060036"
---
# <a name="conversationmember-resource-type"></a><span data-ttu-id="bc4a4-103">Тип ресурса conversationMember</span><span class="sxs-lookup"><span data-stu-id="bc4a4-103">conversationMember resource type</span></span>

<span data-ttu-id="bc4a4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc4a4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc4a4-105">Представляет пользователя в [команде,](team.md) [канале или](channel.md) [чате.](chat.md)</span><span class="sxs-lookup"><span data-stu-id="bc4a4-105">Represents a user in a [team](team.md) or a [channel](channel.md) or a [chat](chat.md).</span></span>
<span data-ttu-id="bc4a4-106">См. [также aadUserConversationMember](aaduserconversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="bc4a4-106">See also [aadUserConversationMember](aaduserconversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="bc4a4-107">Методы</span><span class="sxs-lookup"><span data-stu-id="bc4a4-107">Methods</span></span>

| <span data-ttu-id="bc4a4-108">Метод</span><span class="sxs-lookup"><span data-stu-id="bc4a4-108">Method</span></span>       | <span data-ttu-id="bc4a4-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bc4a4-109">Return Type</span></span>  |<span data-ttu-id="bc4a4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bc4a4-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bc4a4-111">Список участников группы</span><span class="sxs-lookup"><span data-stu-id="bc4a4-111">List team members</span></span>](../api/team-list-members.md)|<span data-ttu-id="bc4a4-112">Коллекция [conversationMember](../resources/conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="bc4a4-112">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="bc4a4-113">Получение списка участников группы.</span><span class="sxs-lookup"><span data-stu-id="bc4a4-113">Get the list of members in the team.</span></span>|
|[<span data-ttu-id="bc4a4-114">Добавление участника в команду</span><span class="sxs-lookup"><span data-stu-id="bc4a4-114">Add team member</span></span>](../api/team-post-members.md)|[<span data-ttu-id="bc4a4-115">conversationMember</span><span class="sxs-lookup"><span data-stu-id="bc4a4-115">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="bc4a4-116">Добавление нового участника в группу.</span><span class="sxs-lookup"><span data-stu-id="bc4a4-116">Add a new member to the team.</span></span>|
|[<span data-ttu-id="bc4a4-117">Массовое добавление участников в группу</span><span class="sxs-lookup"><span data-stu-id="bc4a4-117">Add team members in bulk</span></span>](../api/conversationmembers-add.md)|<span data-ttu-id="bc4a4-118">Коллекция [actionResultPart](../resources/actionresultpart.md)</span><span class="sxs-lookup"><span data-stu-id="bc4a4-118">[actionResultPart](../resources/actionresultpart.md) collection</span></span>|<span data-ttu-id="bc4a4-119">Добавление нескольких участников в команду одним запросом.</span><span class="sxs-lookup"><span data-stu-id="bc4a4-119">Add multiple members to the team in a single request.</span></span>|
|[<span data-ttu-id="bc4a4-120">Получение участника группы</span><span class="sxs-lookup"><span data-stu-id="bc4a4-120">Get team member</span></span>](../api/team-get-members.md) | <span data-ttu-id="bc4a4-121">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="bc4a4-121">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="bc4a4-122">Получение участника группы.</span><span class="sxs-lookup"><span data-stu-id="bc4a4-122">Get a member in the team.</span></span>|
|[<span data-ttu-id="bc4a4-123">Обновление роли участника команды</span><span class="sxs-lookup"><span data-stu-id="bc4a4-123">Update team member's role</span></span>](../api/team-update-members.md)|[<span data-ttu-id="bc4a4-124">conversationMember</span><span class="sxs-lookup"><span data-stu-id="bc4a4-124">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="bc4a4-125">Перевод пользователя из категории участников в категорию владельцев или наоборот, из категории владельцев в категорию обычных участников.</span><span class="sxs-lookup"><span data-stu-id="bc4a4-125">Change a member to an owner or back to a regular member.</span></span>|
|[<span data-ttu-id="bc4a4-126">Удаление участника группы</span><span class="sxs-lookup"><span data-stu-id="bc4a4-126">Remove team member</span></span>](../api/team-delete-members.md)|<span data-ttu-id="bc4a4-127">Нет</span><span class="sxs-lookup"><span data-stu-id="bc4a4-127">None</span></span>|<span data-ttu-id="bc4a4-128">Удаление существующего участника из группы.</span><span class="sxs-lookup"><span data-stu-id="bc4a4-128">Remove an existing member from the team.</span></span>|
|[<span data-ttu-id="bc4a4-129">Перечисление участников канала</span><span class="sxs-lookup"><span data-stu-id="bc4a4-129">List channel members</span></span>](../api/channel-list-members.md) | <span data-ttu-id="bc4a4-130">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="bc4a4-130">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="bc4a4-131">Получение списка всех участников канала.</span><span class="sxs-lookup"><span data-stu-id="bc4a4-131">Get the list of all members in a channel.</span></span>|
|[<span data-ttu-id="bc4a4-132">Добавление участника канала</span><span class="sxs-lookup"><span data-stu-id="bc4a4-132">Add channel member</span></span>](../api/channel-post-members.md) | [<span data-ttu-id="bc4a4-133">conversationMember</span><span class="sxs-lookup"><span data-stu-id="bc4a4-133">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="bc4a4-134">Добавление участника в канал.</span><span class="sxs-lookup"><span data-stu-id="bc4a4-134">Add a member to a channel.</span></span> <span data-ttu-id="bc4a4-135">Поддерживается только для `channel` с типом членства `private`.</span><span class="sxs-lookup"><span data-stu-id="bc4a4-135">Only supported for `channel` with membershipType of `private`.</span></span>|
|[<span data-ttu-id="bc4a4-136">Получение участника канала</span><span class="sxs-lookup"><span data-stu-id="bc4a4-136">Get channel member</span></span>](../api/channel-get-members.md) | <span data-ttu-id="bc4a4-137">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="bc4a4-137">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="bc4a4-138">Получение участника канала.</span><span class="sxs-lookup"><span data-stu-id="bc4a4-138">Get a member in a channel.</span></span>|
|[<span data-ttu-id="bc4a4-139">Обновление роли участника канала</span><span class="sxs-lookup"><span data-stu-id="bc4a4-139">Update channel member's role</span></span>](../api/channel-update-members.md) | [<span data-ttu-id="bc4a4-140">conversationMember</span><span class="sxs-lookup"><span data-stu-id="bc4a4-140">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="bc4a4-141">Обновление свойства участника канала.</span><span class="sxs-lookup"><span data-stu-id="bc4a4-141">Update the properties of a member of the channel.</span></span> <span data-ttu-id="bc4a4-142">Поддерживается только для канала с типом членства `private`.</span><span class="sxs-lookup"><span data-stu-id="bc4a4-142">Only supported for channel with membershipType of `private`.</span></span>|
|[<span data-ttu-id="bc4a4-143">Удаление участника канала</span><span class="sxs-lookup"><span data-stu-id="bc4a4-143">Remove channel member</span></span>](../api/channel-delete-members.md) | <span data-ttu-id="bc4a4-144">Нет</span><span class="sxs-lookup"><span data-stu-id="bc4a4-144">None</span></span> | <span data-ttu-id="bc4a4-145">Удаление участника канала.</span><span class="sxs-lookup"><span data-stu-id="bc4a4-145">Delete a member from a channel.</span></span> <span data-ttu-id="bc4a4-146">Поддерживается, только если параметру `channelType` присвоено значение `private`.</span><span class="sxs-lookup"><span data-stu-id="bc4a4-146">Only supported for `channelType` of `private`.</span></span>|
|[<span data-ttu-id="bc4a4-147">Перечисление участников чата</span><span class="sxs-lookup"><span data-stu-id="bc4a4-147">List chat members</span></span>](../api/chat-list-members.md) | <span data-ttu-id="bc4a4-148">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="bc4a4-148">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="bc4a4-149">Получение списка всех участников чата.</span><span class="sxs-lookup"><span data-stu-id="bc4a4-149">Get the list of all members in a chat.</span></span>|
|[<span data-ttu-id="bc4a4-150">Добавление участника в чат</span><span class="sxs-lookup"><span data-stu-id="bc4a4-150">Add chat member</span></span>](../api/chat-post-members.md) | <span data-ttu-id="bc4a4-151">Заголовок размещения</span><span class="sxs-lookup"><span data-stu-id="bc4a4-151">Location header</span></span> | <span data-ttu-id="bc4a4-152">Добавление участника в чат.</span><span class="sxs-lookup"><span data-stu-id="bc4a4-152">Add a member to a chat.</span></span>| 
|[<span data-ttu-id="bc4a4-153">Получение участника чата</span><span class="sxs-lookup"><span data-stu-id="bc4a4-153">Get chat member</span></span>](../api/chat-get-members.md) | [<span data-ttu-id="bc4a4-154">conversationMember</span><span class="sxs-lookup"><span data-stu-id="bc4a4-154">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="bc4a4-155">Получение участника чата.</span><span class="sxs-lookup"><span data-stu-id="bc4a4-155">Get a member in a chat.</span></span>|
|[<span data-ttu-id="bc4a4-156">Удаление участника чата</span><span class="sxs-lookup"><span data-stu-id="bc4a4-156">Remove chat member</span></span>](../api/chat-delete-members.md) | <span data-ttu-id="bc4a4-157">Нет</span><span class="sxs-lookup"><span data-stu-id="bc4a4-157">None</span></span> | <span data-ttu-id="bc4a4-158">Удаление участника из чата.</span><span class="sxs-lookup"><span data-stu-id="bc4a4-158">Remove a member from a chat.</span></span>| 

## <a name="properties"></a><span data-ttu-id="bc4a4-159">Свойства</span><span class="sxs-lookup"><span data-stu-id="bc4a4-159">Properties</span></span>

| <span data-ttu-id="bc4a4-160">Свойство</span><span class="sxs-lookup"><span data-stu-id="bc4a4-160">Property</span></span>   | <span data-ttu-id="bc4a4-161">Тип</span><span class="sxs-lookup"><span data-stu-id="bc4a4-161">Type</span></span> |<span data-ttu-id="bc4a4-162">Описание</span><span class="sxs-lookup"><span data-stu-id="bc4a4-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bc4a4-163">id</span><span class="sxs-lookup"><span data-stu-id="bc4a4-163">id</span></span>|<span data-ttu-id="bc4a4-164">String</span><span class="sxs-lookup"><span data-stu-id="bc4a4-164">String</span></span>| <span data-ttu-id="bc4a4-165">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bc4a4-165">Read-only.</span></span> <span data-ttu-id="bc4a4-166">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="bc4a4-166">Unique ID of the user.</span></span>|
|<span data-ttu-id="bc4a4-167">displayName</span><span class="sxs-lookup"><span data-stu-id="bc4a4-167">displayName</span></span>| <span data-ttu-id="bc4a4-168">string</span><span class="sxs-lookup"><span data-stu-id="bc4a4-168">string</span></span> | <span data-ttu-id="bc4a4-169">Отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="bc4a4-169">The display name of the user.</span></span> |
|<span data-ttu-id="bc4a4-170">roles</span><span class="sxs-lookup"><span data-stu-id="bc4a4-170">roles</span></span>| <span data-ttu-id="bc4a4-171">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="bc4a4-171">string collection</span></span> | <span data-ttu-id="bc4a4-172">Роли этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="bc4a4-172">The roles for that user.</span></span> |
|<span data-ttu-id="bc4a4-173">visibleHistoryStartDateTime</span><span class="sxs-lookup"><span data-stu-id="bc4a4-173">visibleHistoryStartDateTime</span></span>| <span data-ttu-id="bc4a4-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc4a4-174">DateTimeOffset</span></span> | <span data-ttu-id="bc4a4-175">Метка времени, обозначающая, насколько глубоко участник беседы может видеть историю беседы.</span><span class="sxs-lookup"><span data-stu-id="bc4a4-175">The timestamp denoting how far back a conversation's history is shared with the conversation member.</span></span> <span data-ttu-id="bc4a4-176">Это свойство можно задать только для участников чата.</span><span class="sxs-lookup"><span data-stu-id="bc4a4-176">This property is settable only for members of a chat.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bc4a4-177">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bc4a4-177">JSON representation</span></span>

<span data-ttu-id="bc4a4-178">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bc4a4-178">The following is a JSON representation of the resource.</span></span>

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


