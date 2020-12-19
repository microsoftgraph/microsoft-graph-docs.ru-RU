---
title: Тип ресурса conversationMember
description: Представляет пользователя в беседе.
localization_priority: Normal
author: laujan
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2d2e44349f7896dfed0d0dff455e9afd0ac65772
ms.sourcegitcommit: 0d4377b0153bc339ab7b3b1a6ee4d52848b622d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2020
ms.locfileid: "49714279"
---
# <a name="conversationmember-resource-type"></a><span data-ttu-id="56144-103">Тип ресурса conversationMember</span><span class="sxs-lookup"><span data-stu-id="56144-103">conversationMember resource type</span></span>

<span data-ttu-id="56144-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56144-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="56144-105">Представляет пользователя в команде, [канале](channel.md)или [чате.](chat.md) [](team.md)</span><span class="sxs-lookup"><span data-stu-id="56144-105">Represents a user in a [team](team.md), a [channel](channel.md), or a [chat](chat.md).</span></span>
<span data-ttu-id="56144-106">См. [также aadUserConversationMember.](aaduserconversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="56144-106">See also [aadUserConversationMember](aaduserconversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="56144-107">Методы</span><span class="sxs-lookup"><span data-stu-id="56144-107">Methods</span></span>

| <span data-ttu-id="56144-108">Метод</span><span class="sxs-lookup"><span data-stu-id="56144-108">Method</span></span>       | <span data-ttu-id="56144-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="56144-109">Return Type</span></span>  |<span data-ttu-id="56144-110">Описание</span><span class="sxs-lookup"><span data-stu-id="56144-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="56144-111">Список участников группы</span><span class="sxs-lookup"><span data-stu-id="56144-111">List team members</span></span>](../api/team-list-members.md)|<span data-ttu-id="56144-112">Коллекция [conversationMember](../resources/conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="56144-112">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="56144-113">Получение списка участников группы.</span><span class="sxs-lookup"><span data-stu-id="56144-113">Get the list of members in the team.</span></span>|
|[<span data-ttu-id="56144-114">Добавление участника в команду</span><span class="sxs-lookup"><span data-stu-id="56144-114">Add team member</span></span>](../api/team-post-members.md)|[<span data-ttu-id="56144-115">conversationMember</span><span class="sxs-lookup"><span data-stu-id="56144-115">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="56144-116">Добавление нового участника в группу.</span><span class="sxs-lookup"><span data-stu-id="56144-116">Add a new member to the team.</span></span>|
|[<span data-ttu-id="56144-117">Получение участника группы</span><span class="sxs-lookup"><span data-stu-id="56144-117">Get team member</span></span>](../api/team-get-members.md) | <span data-ttu-id="56144-118">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="56144-118">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="56144-119">Получение участника группы.</span><span class="sxs-lookup"><span data-stu-id="56144-119">Get a member in the team.</span></span>|
|[<span data-ttu-id="56144-120">Обновление роли участника команды</span><span class="sxs-lookup"><span data-stu-id="56144-120">Update team member's role</span></span>](../api/team-update-members.md)|[<span data-ttu-id="56144-121">conversationMember</span><span class="sxs-lookup"><span data-stu-id="56144-121">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="56144-122">Перевод пользователя из категории участников в категорию владельцев или наоборот, из категории владельцев в категорию обычных участников.</span><span class="sxs-lookup"><span data-stu-id="56144-122">Change a member to an owner or back to a regular member.</span></span>|
|[<span data-ttu-id="56144-123">Удаление участника группы</span><span class="sxs-lookup"><span data-stu-id="56144-123">Remove team member</span></span>](../api/team-delete-members.md)|<span data-ttu-id="56144-124">Нет</span><span class="sxs-lookup"><span data-stu-id="56144-124">None</span></span>|<span data-ttu-id="56144-125">Удаление существующего участника из группы.</span><span class="sxs-lookup"><span data-stu-id="56144-125">Remove an existing member from the team.</span></span>|
|[<span data-ttu-id="56144-126">Перечисление участников канала</span><span class="sxs-lookup"><span data-stu-id="56144-126">List channel members</span></span>](../api/channel-list-members.md) | <span data-ttu-id="56144-127">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="56144-127">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="56144-128">Получение списка всех участников канала.</span><span class="sxs-lookup"><span data-stu-id="56144-128">Get the list of all members in a channel.</span></span>|
|[<span data-ttu-id="56144-129">Добавление участника канала</span><span class="sxs-lookup"><span data-stu-id="56144-129">Add channel member</span></span>](../api/channel-post-members.md) | [<span data-ttu-id="56144-130">conversationMember</span><span class="sxs-lookup"><span data-stu-id="56144-130">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="56144-131">Добавление участника в канал.</span><span class="sxs-lookup"><span data-stu-id="56144-131">Add a member to a channel.</span></span> <span data-ttu-id="56144-132">Поддерживается только для `channel` с типом членства `private`.</span><span class="sxs-lookup"><span data-stu-id="56144-132">Only supported for `channel`with membershipType of `private`.</span></span>|
|[<span data-ttu-id="56144-133">Получение участника канала</span><span class="sxs-lookup"><span data-stu-id="56144-133">Get channel member</span></span>](../api/channel-get-members.md) | <span data-ttu-id="56144-134">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="56144-134">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="56144-135">Получение участника канала.</span><span class="sxs-lookup"><span data-stu-id="56144-135">Get a member in a channel.</span></span>|
|[<span data-ttu-id="56144-136">Обновление роли участника канала</span><span class="sxs-lookup"><span data-stu-id="56144-136">Update channel member's role</span></span>](../api/channel-update-members.md) | [<span data-ttu-id="56144-137">conversationMember</span><span class="sxs-lookup"><span data-stu-id="56144-137">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="56144-138">Обновление свойства участника канала.</span><span class="sxs-lookup"><span data-stu-id="56144-138">Update the properties of a member of the channel.</span></span> <span data-ttu-id="56144-139">Поддерживается только для канала с типом членства `private`.</span><span class="sxs-lookup"><span data-stu-id="56144-139">Only supported for channel with membershipType of `private`.</span></span>|
|[<span data-ttu-id="56144-140">Удаление участника канала</span><span class="sxs-lookup"><span data-stu-id="56144-140">Remove channel member</span></span>](../api/channel-delete-members.md) | <span data-ttu-id="56144-141">Нет</span><span class="sxs-lookup"><span data-stu-id="56144-141">None</span></span> | <span data-ttu-id="56144-142">Удаление участника канала.</span><span class="sxs-lookup"><span data-stu-id="56144-142">Delete a member from a channel.</span></span> <span data-ttu-id="56144-143">Поддерживается, только если параметру `channelType` присвоено значение `private`.</span><span class="sxs-lookup"><span data-stu-id="56144-143">Only supported for `channelType` of `private`.</span></span>|

## <a name="properties"></a><span data-ttu-id="56144-144">Свойства</span><span class="sxs-lookup"><span data-stu-id="56144-144">Properties</span></span>

| <span data-ttu-id="56144-145">Свойство</span><span class="sxs-lookup"><span data-stu-id="56144-145">Property</span></span>   | <span data-ttu-id="56144-146">Тип</span><span class="sxs-lookup"><span data-stu-id="56144-146">Type</span></span> |<span data-ttu-id="56144-147">Описание</span><span class="sxs-lookup"><span data-stu-id="56144-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="56144-148">id</span><span class="sxs-lookup"><span data-stu-id="56144-148">id</span></span>|<span data-ttu-id="56144-149">String</span><span class="sxs-lookup"><span data-stu-id="56144-149">String</span></span>| <span data-ttu-id="56144-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="56144-150">Read-only.</span></span> <span data-ttu-id="56144-151">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="56144-151">Unique ID of the user.</span></span>|
|<span data-ttu-id="56144-152">displayName</span><span class="sxs-lookup"><span data-stu-id="56144-152">displayName</span></span>| <span data-ttu-id="56144-153">string</span><span class="sxs-lookup"><span data-stu-id="56144-153">string</span></span> | <span data-ttu-id="56144-154">Отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="56144-154">The display name of the user.</span></span> |
|<span data-ttu-id="56144-155">roles</span><span class="sxs-lookup"><span data-stu-id="56144-155">roles</span></span>| <span data-ttu-id="56144-156">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="56144-156">string collection</span></span> | <span data-ttu-id="56144-157">Роли этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="56144-157">The roles for that user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="56144-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="56144-158">JSON representation</span></span>

<span data-ttu-id="56144-159">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="56144-159">The following is a JSON representation of the resource.</span></span>

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

