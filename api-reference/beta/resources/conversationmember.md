---
title: Тип ресурса conversationMember
description: Представляет пользователя в беседе.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2a8e4c94681065d9686e9f17888d3abf35885a65
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49658044"
---
# <a name="conversationmember-resource-type"></a><span data-ttu-id="73289-103">Тип ресурса conversationMember</span><span class="sxs-lookup"><span data-stu-id="73289-103">conversationMember resource type</span></span>

<span data-ttu-id="73289-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73289-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73289-105">Представляет пользователя в [чате](chat.md) или [канале](channel.md).</span><span class="sxs-lookup"><span data-stu-id="73289-105">Represents a user in a [chat](chat.md) or a [channel](channel.md).</span></span>
<span data-ttu-id="73289-106">См. [также aadUserConversationMember.](aaduserconversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="73289-106">See also [aadUserConversationMember](aaduserconversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="73289-107">Методы</span><span class="sxs-lookup"><span data-stu-id="73289-107">Methods</span></span>

| <span data-ttu-id="73289-108">Метод</span><span class="sxs-lookup"><span data-stu-id="73289-108">Method</span></span>       | <span data-ttu-id="73289-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="73289-109">Return Type</span></span>  |<span data-ttu-id="73289-110">Описание</span><span class="sxs-lookup"><span data-stu-id="73289-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="73289-111">Список участников чата</span><span class="sxs-lookup"><span data-stu-id="73289-111">List chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="73289-112">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="73289-112">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="73289-113">Получение списка всех пользователей в чате.</span><span class="sxs-lookup"><span data-stu-id="73289-113">Get the list of all users in the chat.</span></span>|
|[<span data-ttu-id="73289-114">Получить участника чата</span><span class="sxs-lookup"><span data-stu-id="73289-114">Get chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="73289-115">conversationMember</span><span class="sxs-lookup"><span data-stu-id="73289-115">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="73289-116">Получение одного пользователя в чате.</span><span class="sxs-lookup"><span data-stu-id="73289-116">Get a single user in the chat.</span></span>|
|[<span data-ttu-id="73289-117">Список участников группы</span><span class="sxs-lookup"><span data-stu-id="73289-117">List team members</span></span>](../api/team-list-members.md)|<span data-ttu-id="73289-118">Коллекция [conversationMember](../resources/conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="73289-118">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="73289-119">Получение списка участников группы.</span><span class="sxs-lookup"><span data-stu-id="73289-119">Get the list of members in the team.</span></span>|
|[<span data-ttu-id="73289-120">Получить участника группы</span><span class="sxs-lookup"><span data-stu-id="73289-120">Get team member</span></span>](../api/team-get-members.md) | <span data-ttu-id="73289-121">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="73289-121">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="73289-122">Получение участника группы.</span><span class="sxs-lookup"><span data-stu-id="73289-122">Get a member in the team.</span></span>|
|[<span data-ttu-id="73289-123">Добавление участника группы</span><span class="sxs-lookup"><span data-stu-id="73289-123">Add team member</span></span>](../api/team-post-members.md)|[<span data-ttu-id="73289-124">conversationMember</span><span class="sxs-lookup"><span data-stu-id="73289-124">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="73289-125">Добавление нового участника в группу.</span><span class="sxs-lookup"><span data-stu-id="73289-125">Add a new member to the team.</span></span>|
|[<span data-ttu-id="73289-126">Массовое добавление участников команды</span><span class="sxs-lookup"><span data-stu-id="73289-126">Add team members in bulk</span></span>](../api/conversationmembers-add.md)|<span data-ttu-id="73289-127">[Коллекция actionResultPart](../resources/actionresultpart.md)</span><span class="sxs-lookup"><span data-stu-id="73289-127">[actionResultPart](../resources/actionresultpart.md) collection</span></span>|<span data-ttu-id="73289-128">Добавьте в команду несколько участников в одном запросе.</span><span class="sxs-lookup"><span data-stu-id="73289-128">Add multiple members to the team in a single request.</span></span>|
|[<span data-ttu-id="73289-129">Обновление роли участника группы</span><span class="sxs-lookup"><span data-stu-id="73289-129">Update team member's role</span></span>](../api/team-update-members.md)|[<span data-ttu-id="73289-130">conversationMember</span><span class="sxs-lookup"><span data-stu-id="73289-130">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="73289-131">Перевод пользователя из категории участников в категорию владельцев или наоборот, из категории владельцев в категорию обычных участников.</span><span class="sxs-lookup"><span data-stu-id="73289-131">Change a member to an owner or back to a regular member.</span></span>|
|[<span data-ttu-id="73289-132">Удаление участника группы</span><span class="sxs-lookup"><span data-stu-id="73289-132">Remove team member</span></span>](../api/team-delete-members.md)|<span data-ttu-id="73289-133">Нет</span><span class="sxs-lookup"><span data-stu-id="73289-133">None</span></span>|<span data-ttu-id="73289-134">Удаление существующего участника из группы.</span><span class="sxs-lookup"><span data-stu-id="73289-134">Remove an existing member from the team.</span></span>|
|[<span data-ttu-id="73289-135">Получение участника канала</span><span class="sxs-lookup"><span data-stu-id="73289-135">Get channel member</span></span>](../api/channel-get-members.md) | <span data-ttu-id="73289-136">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="73289-136">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="73289-137">Получение участника канала.</span><span class="sxs-lookup"><span data-stu-id="73289-137">Get a member in a channel.</span></span>|
|[<span data-ttu-id="73289-138">Создание участника канала</span><span class="sxs-lookup"><span data-stu-id="73289-138">Create channel member</span></span>](../api/channel-post-members.md) | [<span data-ttu-id="73289-139">conversationMember</span><span class="sxs-lookup"><span data-stu-id="73289-139">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="73289-140">Добавление участника в канал.</span><span class="sxs-lookup"><span data-stu-id="73289-140">Add a member to a channel.</span></span> <span data-ttu-id="73289-141">Поддерживается только для `channel` с типом членства `private`.</span><span class="sxs-lookup"><span data-stu-id="73289-141">Only supported for `channel`with membershipType of `private`.</span></span>|
|[<span data-ttu-id="73289-142">Обновление роли участника канала</span><span class="sxs-lookup"><span data-stu-id="73289-142">Update channel member's role</span></span>](../api/channel-update-members.md) | [<span data-ttu-id="73289-143">conversationMember</span><span class="sxs-lookup"><span data-stu-id="73289-143">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="73289-144">Обновление свойства участника канала.</span><span class="sxs-lookup"><span data-stu-id="73289-144">Update the properties of a member of the channel.</span></span> <span data-ttu-id="73289-145">Поддерживается только для канала с типом членства `private`.</span><span class="sxs-lookup"><span data-stu-id="73289-145">Only supported for channel with membershipType of `private`.</span></span>|
|[<span data-ttu-id="73289-146">Удаление участника канала</span><span class="sxs-lookup"><span data-stu-id="73289-146">Remove channel member</span></span>](../api/channel-delete-members.md) | <span data-ttu-id="73289-147">Нет</span><span class="sxs-lookup"><span data-stu-id="73289-147">None</span></span> | <span data-ttu-id="73289-148">Удаление участника канала.</span><span class="sxs-lookup"><span data-stu-id="73289-148">Delete a member from a channel.</span></span> <span data-ttu-id="73289-149">Поддерживается, только если параметру `channelType` присвоено значение `private`.</span><span class="sxs-lookup"><span data-stu-id="73289-149">Only supported for `channelType` of `private`.</span></span>|



## <a name="properties"></a><span data-ttu-id="73289-150">Свойства</span><span class="sxs-lookup"><span data-stu-id="73289-150">Properties</span></span>

| <span data-ttu-id="73289-151">Свойство</span><span class="sxs-lookup"><span data-stu-id="73289-151">Property</span></span>   | <span data-ttu-id="73289-152">Тип</span><span class="sxs-lookup"><span data-stu-id="73289-152">Type</span></span> |<span data-ttu-id="73289-153">Описание</span><span class="sxs-lookup"><span data-stu-id="73289-153">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="73289-154">id</span><span class="sxs-lookup"><span data-stu-id="73289-154">id</span></span>|<span data-ttu-id="73289-155">String</span><span class="sxs-lookup"><span data-stu-id="73289-155">String</span></span>| <span data-ttu-id="73289-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="73289-156">Read-only.</span></span> <span data-ttu-id="73289-157">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="73289-157">Unique ID of the user.</span></span>|
|<span data-ttu-id="73289-158">displayName</span><span class="sxs-lookup"><span data-stu-id="73289-158">displayName</span></span>| <span data-ttu-id="73289-159">string</span><span class="sxs-lookup"><span data-stu-id="73289-159">string</span></span> | <span data-ttu-id="73289-160">Отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="73289-160">The display name of the user.</span></span> |
|<span data-ttu-id="73289-161">roles</span><span class="sxs-lookup"><span data-stu-id="73289-161">roles</span></span>| <span data-ttu-id="73289-162">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="73289-162">string collection</span></span> | <span data-ttu-id="73289-163">Роли этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="73289-163">The roles for that user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="73289-164">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="73289-164">JSON representation</span></span>

<span data-ttu-id="73289-165">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="73289-165">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.conversationMember",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)",
  "roles": ["String"]
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


