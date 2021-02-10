---
title: Тип ресурса conversationMember
description: Представляет пользователя в беседе.
localization_priority: Normal
author: laujan
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 1629b46b12d91fd96dca72577027f0031ab0102a
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161791"
---
# <a name="conversationmember-resource-type"></a><span data-ttu-id="128e4-103">Тип ресурса conversationMember</span><span class="sxs-lookup"><span data-stu-id="128e4-103">conversationMember resource type</span></span>

<span data-ttu-id="128e4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="128e4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="128e4-105">Представляет пользователя в команде, [канале](channel.md)или [чате.](chat.md) [](team.md)</span><span class="sxs-lookup"><span data-stu-id="128e4-105">Represents a user in a [team](team.md), a [channel](channel.md), or a [chat](chat.md).</span></span>
<span data-ttu-id="128e4-106">См. [также aadUserConversationMember.](aaduserconversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="128e4-106">See also [aadUserConversationMember](aaduserconversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="128e4-107">Методы</span><span class="sxs-lookup"><span data-stu-id="128e4-107">Methods</span></span>

| <span data-ttu-id="128e4-108">Метод</span><span class="sxs-lookup"><span data-stu-id="128e4-108">Method</span></span>       | <span data-ttu-id="128e4-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="128e4-109">Return Type</span></span>  |<span data-ttu-id="128e4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="128e4-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="128e4-111">Список участников группы</span><span class="sxs-lookup"><span data-stu-id="128e4-111">List team members</span></span>](../api/team-list-members.md)|<span data-ttu-id="128e4-112">Коллекция [conversationMember](../resources/conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="128e4-112">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="128e4-113">Получение списка участников группы.</span><span class="sxs-lookup"><span data-stu-id="128e4-113">Get the list of members in the team.</span></span>|
|[<span data-ttu-id="128e4-114">Добавление участника в команду</span><span class="sxs-lookup"><span data-stu-id="128e4-114">Add team member</span></span>](../api/team-post-members.md)|[<span data-ttu-id="128e4-115">conversationMember</span><span class="sxs-lookup"><span data-stu-id="128e4-115">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="128e4-116">Добавление нового участника в группу.</span><span class="sxs-lookup"><span data-stu-id="128e4-116">Add a new member to the team.</span></span>|
|[<span data-ttu-id="128e4-117">Получение участника группы</span><span class="sxs-lookup"><span data-stu-id="128e4-117">Get team member</span></span>](../api/team-get-members.md) | <span data-ttu-id="128e4-118">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="128e4-118">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="128e4-119">Получение участника группы.</span><span class="sxs-lookup"><span data-stu-id="128e4-119">Get a member in the team.</span></span>|
|[<span data-ttu-id="128e4-120">Обновление роли участника команды</span><span class="sxs-lookup"><span data-stu-id="128e4-120">Update team member's role</span></span>](../api/team-update-members.md)|[<span data-ttu-id="128e4-121">conversationMember</span><span class="sxs-lookup"><span data-stu-id="128e4-121">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="128e4-122">Перевод пользователя из категории участников в категорию владельцев или наоборот, из категории владельцев в категорию обычных участников.</span><span class="sxs-lookup"><span data-stu-id="128e4-122">Change a member to an owner or back to a regular member.</span></span>|
|[<span data-ttu-id="128e4-123">Удаление участника группы</span><span class="sxs-lookup"><span data-stu-id="128e4-123">Remove team member</span></span>](../api/team-delete-members.md)|<span data-ttu-id="128e4-124">Нет</span><span class="sxs-lookup"><span data-stu-id="128e4-124">None</span></span>|<span data-ttu-id="128e4-125">Удаление существующего участника из группы.</span><span class="sxs-lookup"><span data-stu-id="128e4-125">Remove an existing member from the team.</span></span>|
|[<span data-ttu-id="128e4-126">Перечисление участников канала</span><span class="sxs-lookup"><span data-stu-id="128e4-126">List channel members</span></span>](../api/channel-list-members.md) | <span data-ttu-id="128e4-127">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="128e4-127">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="128e4-128">Получение списка всех участников канала.</span><span class="sxs-lookup"><span data-stu-id="128e4-128">Get the list of all members in a channel.</span></span>|
|[<span data-ttu-id="128e4-129">Добавление участника канала</span><span class="sxs-lookup"><span data-stu-id="128e4-129">Add channel member</span></span>](../api/channel-post-members.md) | [<span data-ttu-id="128e4-130">conversationMember</span><span class="sxs-lookup"><span data-stu-id="128e4-130">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="128e4-131">Добавление участника в канал.</span><span class="sxs-lookup"><span data-stu-id="128e4-131">Add a member to a channel.</span></span> <span data-ttu-id="128e4-132">Поддерживается только для `channel` с типом членства `private`.</span><span class="sxs-lookup"><span data-stu-id="128e4-132">Only supported for `channel`with membershipType of `private`.</span></span>|
|[<span data-ttu-id="128e4-133">Получение участника канала</span><span class="sxs-lookup"><span data-stu-id="128e4-133">Get channel member</span></span>](../api/channel-get-members.md) | <span data-ttu-id="128e4-134">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="128e4-134">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="128e4-135">Получение участника канала.</span><span class="sxs-lookup"><span data-stu-id="128e4-135">Get a member in a channel.</span></span>|
|[<span data-ttu-id="128e4-136">Обновление роли участника канала</span><span class="sxs-lookup"><span data-stu-id="128e4-136">Update channel member's role</span></span>](../api/channel-update-members.md) | [<span data-ttu-id="128e4-137">conversationMember</span><span class="sxs-lookup"><span data-stu-id="128e4-137">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="128e4-138">Обновление свойства участника канала.</span><span class="sxs-lookup"><span data-stu-id="128e4-138">Update the properties of a member of the channel.</span></span> <span data-ttu-id="128e4-139">Поддерживается только для канала с типом членства `private`.</span><span class="sxs-lookup"><span data-stu-id="128e4-139">Only supported for channel with membershipType of `private`.</span></span>|
|[<span data-ttu-id="128e4-140">Удаление участника канала</span><span class="sxs-lookup"><span data-stu-id="128e4-140">Remove channel member</span></span>](../api/channel-delete-members.md) | <span data-ttu-id="128e4-141">Нет</span><span class="sxs-lookup"><span data-stu-id="128e4-141">None</span></span> | <span data-ttu-id="128e4-142">Удаление участника канала.</span><span class="sxs-lookup"><span data-stu-id="128e4-142">Delete a member from a channel.</span></span> <span data-ttu-id="128e4-143">Поддерживается, только если параметру `channelType` присвоено значение `private`.</span><span class="sxs-lookup"><span data-stu-id="128e4-143">Only supported for `channelType` of `private`.</span></span>|

## <a name="properties"></a><span data-ttu-id="128e4-144">Свойства</span><span class="sxs-lookup"><span data-stu-id="128e4-144">Properties</span></span>

| <span data-ttu-id="128e4-145">Свойство</span><span class="sxs-lookup"><span data-stu-id="128e4-145">Property</span></span>   | <span data-ttu-id="128e4-146">Тип</span><span class="sxs-lookup"><span data-stu-id="128e4-146">Type</span></span> |<span data-ttu-id="128e4-147">Описание</span><span class="sxs-lookup"><span data-stu-id="128e4-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="128e4-148">id</span><span class="sxs-lookup"><span data-stu-id="128e4-148">id</span></span>|<span data-ttu-id="128e4-149">String</span><span class="sxs-lookup"><span data-stu-id="128e4-149">String</span></span>| <span data-ttu-id="128e4-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="128e4-150">Read-only.</span></span> <span data-ttu-id="128e4-151">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="128e4-151">Unique ID of the user.</span></span>|
|<span data-ttu-id="128e4-152">displayName</span><span class="sxs-lookup"><span data-stu-id="128e4-152">displayName</span></span>| <span data-ttu-id="128e4-153">string</span><span class="sxs-lookup"><span data-stu-id="128e4-153">string</span></span> | <span data-ttu-id="128e4-154">Отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="128e4-154">The display name of the user.</span></span> |
|<span data-ttu-id="128e4-155">roles</span><span class="sxs-lookup"><span data-stu-id="128e4-155">roles</span></span>| <span data-ttu-id="128e4-156">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="128e4-156">string collection</span></span> | <span data-ttu-id="128e4-157">Роли этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="128e4-157">The roles for that user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="128e4-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="128e4-158">JSON representation</span></span>

<span data-ttu-id="128e4-159">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="128e4-159">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.conversationMember",
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

