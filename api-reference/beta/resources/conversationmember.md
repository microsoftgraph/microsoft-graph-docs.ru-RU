---
title: Тип ресурса conversationMember
description: Представляет пользователя в беседе.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7f6b24b65a6ae25f8a05bf067659c04d49c06d24
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706068"
---
# <a name="conversationmember-resource-type"></a><span data-ttu-id="93d38-103">Тип ресурса conversationMember</span><span class="sxs-lookup"><span data-stu-id="93d38-103">conversationMember resource type</span></span>

<span data-ttu-id="93d38-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93d38-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93d38-105">Представляет пользователя в [чате](chat.md) или [канале](channel.md).</span><span class="sxs-lookup"><span data-stu-id="93d38-105">Represents a user in a [chat](chat.md) or a [channel](channel.md).</span></span>
<span data-ttu-id="93d38-106">См. [также aadUserConversationMember.](aaduserconversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="93d38-106">See also [aadUserConversationMember](aaduserconversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="93d38-107">Методы</span><span class="sxs-lookup"><span data-stu-id="93d38-107">Methods</span></span>

| <span data-ttu-id="93d38-108">Метод</span><span class="sxs-lookup"><span data-stu-id="93d38-108">Method</span></span>       | <span data-ttu-id="93d38-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="93d38-109">Return Type</span></span>  |<span data-ttu-id="93d38-110">Описание</span><span class="sxs-lookup"><span data-stu-id="93d38-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="93d38-111">Список участников группы</span><span class="sxs-lookup"><span data-stu-id="93d38-111">List team members</span></span>](../api/team-list-members.md)|<span data-ttu-id="93d38-112">Коллекция [conversationMember](../resources/conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="93d38-112">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="93d38-113">Получение списка участников группы.</span><span class="sxs-lookup"><span data-stu-id="93d38-113">Get the list of members in the team.</span></span>|
|[<span data-ttu-id="93d38-114">Получить участника команды</span><span class="sxs-lookup"><span data-stu-id="93d38-114">Get team member</span></span>](../api/team-get-members.md) | <span data-ttu-id="93d38-115">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="93d38-115">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="93d38-116">Получение участника группы.</span><span class="sxs-lookup"><span data-stu-id="93d38-116">Get a member in the team.</span></span>|
|[<span data-ttu-id="93d38-117">Добавление участника группы</span><span class="sxs-lookup"><span data-stu-id="93d38-117">Add team member</span></span>](../api/team-post-members.md)|[<span data-ttu-id="93d38-118">conversationMember</span><span class="sxs-lookup"><span data-stu-id="93d38-118">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="93d38-119">Добавление нового участника в группу.</span><span class="sxs-lookup"><span data-stu-id="93d38-119">Add a new member to the team.</span></span>|
|[<span data-ttu-id="93d38-120">Массовое добавление участников команды</span><span class="sxs-lookup"><span data-stu-id="93d38-120">Add team members in bulk</span></span>](../api/conversationmembers-add.md)|<span data-ttu-id="93d38-121">Коллекция [actionResultPart](../resources/actionresultpart.md)</span><span class="sxs-lookup"><span data-stu-id="93d38-121">[actionResultPart](../resources/actionresultpart.md) collection</span></span>|<span data-ttu-id="93d38-122">Добавление нескольких участников в команду одним запросом.</span><span class="sxs-lookup"><span data-stu-id="93d38-122">Add multiple members to the team in a single request.</span></span>|
|[<span data-ttu-id="93d38-123">Обновление роли участника группы</span><span class="sxs-lookup"><span data-stu-id="93d38-123">Update team member's role</span></span>](../api/team-update-members.md)|[<span data-ttu-id="93d38-124">conversationMember</span><span class="sxs-lookup"><span data-stu-id="93d38-124">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="93d38-125">Перевод пользователя из категории участников в категорию владельцев или наоборот, из категории владельцев в категорию обычных участников.</span><span class="sxs-lookup"><span data-stu-id="93d38-125">Change a member to an owner or back to a regular member.</span></span>|
|[<span data-ttu-id="93d38-126">Удаление участника группы</span><span class="sxs-lookup"><span data-stu-id="93d38-126">Remove team member</span></span>](../api/team-delete-members.md)|<span data-ttu-id="93d38-127">Нет</span><span class="sxs-lookup"><span data-stu-id="93d38-127">None</span></span>|<span data-ttu-id="93d38-128">Удаление существующего участника из группы.</span><span class="sxs-lookup"><span data-stu-id="93d38-128">Remove an existing member from the team.</span></span>|
|[<span data-ttu-id="93d38-129">Перечисление участников канала</span><span class="sxs-lookup"><span data-stu-id="93d38-129">List channel members</span></span>](../api/channel-list-members.md) | <span data-ttu-id="93d38-130">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="93d38-130">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="93d38-131">Получите список всех участников в канале.</span><span class="sxs-lookup"><span data-stu-id="93d38-131">Get the list of all members in a channel.</span></span>|
|[<span data-ttu-id="93d38-132">Получение участника канала</span><span class="sxs-lookup"><span data-stu-id="93d38-132">Get channel member</span></span>](../api/channel-get-members.md) | <span data-ttu-id="93d38-133">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="93d38-133">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="93d38-134">Получение участника канала.</span><span class="sxs-lookup"><span data-stu-id="93d38-134">Get a member in a channel.</span></span>|
|[<span data-ttu-id="93d38-135">Создание участника канала</span><span class="sxs-lookup"><span data-stu-id="93d38-135">Create channel member</span></span>](../api/channel-post-members.md) | [<span data-ttu-id="93d38-136">conversationMember</span><span class="sxs-lookup"><span data-stu-id="93d38-136">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="93d38-137">Добавление участника в канал.</span><span class="sxs-lookup"><span data-stu-id="93d38-137">Add a member to a channel.</span></span> <span data-ttu-id="93d38-138">Поддерживается только для `channel` с типом членства `private`.</span><span class="sxs-lookup"><span data-stu-id="93d38-138">Only supported for `channel`with membershipType of `private`.</span></span>|
|[<span data-ttu-id="93d38-139">Обновление роли участника канала</span><span class="sxs-lookup"><span data-stu-id="93d38-139">Update channel member's role</span></span>](../api/channel-update-members.md) | [<span data-ttu-id="93d38-140">conversationMember</span><span class="sxs-lookup"><span data-stu-id="93d38-140">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="93d38-141">Обновление свойства участника канала.</span><span class="sxs-lookup"><span data-stu-id="93d38-141">Update the properties of a member of the channel.</span></span> <span data-ttu-id="93d38-142">Поддерживается только для канала с типом членства `private`.</span><span class="sxs-lookup"><span data-stu-id="93d38-142">Only supported for channel with membershipType of `private`.</span></span>|
|[<span data-ttu-id="93d38-143">Удаление участника канала</span><span class="sxs-lookup"><span data-stu-id="93d38-143">Remove channel member</span></span>](../api/channel-delete-members.md) | <span data-ttu-id="93d38-144">Нет</span><span class="sxs-lookup"><span data-stu-id="93d38-144">None</span></span> | <span data-ttu-id="93d38-145">Удаление участника канала.</span><span class="sxs-lookup"><span data-stu-id="93d38-145">Delete a member from a channel.</span></span> <span data-ttu-id="93d38-146">Поддерживается, только если параметру `channelType` присвоено значение `private`.</span><span class="sxs-lookup"><span data-stu-id="93d38-146">Only supported for `channelType` of `private`.</span></span>|
|[<span data-ttu-id="93d38-147">Список участников чата</span><span class="sxs-lookup"><span data-stu-id="93d38-147">List chat members</span></span>](../api/chat-list-members.md) | <span data-ttu-id="93d38-148">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="93d38-148">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="93d38-149">Получите список всех участников в чате.</span><span class="sxs-lookup"><span data-stu-id="93d38-149">Get the list of all members in a chat.</span></span>|
|[<span data-ttu-id="93d38-150">Получить участника чата</span><span class="sxs-lookup"><span data-stu-id="93d38-150">Get chat member</span></span>](../api/chat-get-members.md) | [<span data-ttu-id="93d38-151">conversationMember</span><span class="sxs-lookup"><span data-stu-id="93d38-151">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="93d38-152">Получить участника в чате.</span><span class="sxs-lookup"><span data-stu-id="93d38-152">Get a member in a chat.</span></span>|
|[<span data-ttu-id="93d38-153">Добавление участника чата</span><span class="sxs-lookup"><span data-stu-id="93d38-153">Add chat member</span></span>](../api/chat-post-members.md) | <span data-ttu-id="93d38-154">Заголовок Location</span><span class="sxs-lookup"><span data-stu-id="93d38-154">Location header</span></span> | <span data-ttu-id="93d38-155">Добавление участника в чат.</span><span class="sxs-lookup"><span data-stu-id="93d38-155">Add a member to a chat.</span></span>| 

## <a name="properties"></a><span data-ttu-id="93d38-156">Свойства</span><span class="sxs-lookup"><span data-stu-id="93d38-156">Properties</span></span>

| <span data-ttu-id="93d38-157">Свойство</span><span class="sxs-lookup"><span data-stu-id="93d38-157">Property</span></span>   | <span data-ttu-id="93d38-158">Тип</span><span class="sxs-lookup"><span data-stu-id="93d38-158">Type</span></span> |<span data-ttu-id="93d38-159">Описание</span><span class="sxs-lookup"><span data-stu-id="93d38-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="93d38-160">id</span><span class="sxs-lookup"><span data-stu-id="93d38-160">id</span></span>|<span data-ttu-id="93d38-161">String</span><span class="sxs-lookup"><span data-stu-id="93d38-161">String</span></span>| <span data-ttu-id="93d38-162">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="93d38-162">Read-only.</span></span> <span data-ttu-id="93d38-163">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="93d38-163">Unique ID of the user.</span></span>|
|<span data-ttu-id="93d38-164">displayName</span><span class="sxs-lookup"><span data-stu-id="93d38-164">displayName</span></span>| <span data-ttu-id="93d38-165">string</span><span class="sxs-lookup"><span data-stu-id="93d38-165">string</span></span> | <span data-ttu-id="93d38-166">Отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="93d38-166">The display name of the user.</span></span> |
|<span data-ttu-id="93d38-167">roles</span><span class="sxs-lookup"><span data-stu-id="93d38-167">roles</span></span>| <span data-ttu-id="93d38-168">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="93d38-168">string collection</span></span> | <span data-ttu-id="93d38-169">Роли этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="93d38-169">The roles for that user.</span></span> |
|<span data-ttu-id="93d38-170">visibleHistoryStartDateTime</span><span class="sxs-lookup"><span data-stu-id="93d38-170">visibleHistoryStartDateTime</span></span>| <span data-ttu-id="93d38-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93d38-171">DateTimeOffset</span></span> | <span data-ttu-id="93d38-172">Timestamp, обозначающий, как далеко назад история беседы совместно с участником беседы.</span><span class="sxs-lookup"><span data-stu-id="93d38-172">The timestamp denoting how far back a conversation's history is shared with the conversation member.</span></span> <span data-ttu-id="93d38-173">Это свойство можно установить только для участников чата.</span><span class="sxs-lookup"><span data-stu-id="93d38-173">This property is settable only for members of a chat.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="93d38-174">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="93d38-174">JSON representation</span></span>

<span data-ttu-id="93d38-175">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="93d38-175">The following is a JSON representation of the resource.</span></span>

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


