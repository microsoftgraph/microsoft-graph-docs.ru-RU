---
title: Тип ресурса aadUserConversationMember
description: Представляет пользователя Azure Active Directory в чате или канале.
localization_priority: Priority
author: laujan
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: cf678e090f4af26aca1222ba464771111b0b6a60
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/05/2021
ms.locfileid: "49754301"
---
# <a name="aaduserconversationmember-resource-type"></a><span data-ttu-id="6ec7b-103">Тип ресурса aadUserConversationMember</span><span class="sxs-lookup"><span data-stu-id="6ec7b-103">aadUserConversationMember resource type</span></span>

<span data-ttu-id="6ec7b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ec7b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6ec7b-105">Представляет пользователя Azure Active Directory в [команде](team.md), [канале](channel.md) или [чате](chat.md).</span><span class="sxs-lookup"><span data-stu-id="6ec7b-105">Represents an Azure Active Directory user in a [team](team.md), a [channel](channel.md), or a [chat](chat.md).</span></span>
<span data-ttu-id="6ec7b-106">Этот тип наследуется от [conversationMember](conversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="6ec7b-106">This type inherits from [conversationMember](conversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="6ec7b-107">Методы</span><span class="sxs-lookup"><span data-stu-id="6ec7b-107">Methods</span></span>

| <span data-ttu-id="6ec7b-108">Метод</span><span class="sxs-lookup"><span data-stu-id="6ec7b-108">Method</span></span>       | <span data-ttu-id="6ec7b-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6ec7b-109">Return Type</span></span>  |<span data-ttu-id="6ec7b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6ec7b-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6ec7b-111">Список участников группы</span><span class="sxs-lookup"><span data-stu-id="6ec7b-111">List team members</span></span>](../api/team-list-members.md)|<span data-ttu-id="6ec7b-112">Коллекция [conversationMember](../resources/conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="6ec7b-112">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="6ec7b-113">Получение списка участников группы.</span><span class="sxs-lookup"><span data-stu-id="6ec7b-113">Get the list of members in the team.</span></span>|
|[<span data-ttu-id="6ec7b-114">Добавление участника в команду</span><span class="sxs-lookup"><span data-stu-id="6ec7b-114">Add team member</span></span>](../api/team-post-members.md)|[<span data-ttu-id="6ec7b-115">conversationMember</span><span class="sxs-lookup"><span data-stu-id="6ec7b-115">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="6ec7b-116">Добавление нового участника в группу.</span><span class="sxs-lookup"><span data-stu-id="6ec7b-116">Add a new member to the team.</span></span>|
|[<span data-ttu-id="6ec7b-117">Получение участника группы</span><span class="sxs-lookup"><span data-stu-id="6ec7b-117">Get team member</span></span>](../api/team-get-members.md) | <span data-ttu-id="6ec7b-118">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="6ec7b-118">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="6ec7b-119">Получение участника группы.</span><span class="sxs-lookup"><span data-stu-id="6ec7b-119">Get a member in the team.</span></span>|
|[<span data-ttu-id="6ec7b-120">Обновление роли участника команды</span><span class="sxs-lookup"><span data-stu-id="6ec7b-120">Update team member's role</span></span>](../api/team-update-members.md)|[<span data-ttu-id="6ec7b-121">conversationMember</span><span class="sxs-lookup"><span data-stu-id="6ec7b-121">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="6ec7b-122">Перевод пользователя из категории участников в категорию владельцев или наоборот, из категории владельцев в категорию обычных участников.</span><span class="sxs-lookup"><span data-stu-id="6ec7b-122">Change a member to an owner or back to a regular member.</span></span>|
|[<span data-ttu-id="6ec7b-123">Удаление участника группы</span><span class="sxs-lookup"><span data-stu-id="6ec7b-123">Remove team member</span></span>](../api/team-delete-members.md)|<span data-ttu-id="6ec7b-124">Нет</span><span class="sxs-lookup"><span data-stu-id="6ec7b-124">None</span></span>|<span data-ttu-id="6ec7b-125">Удаление существующего участника из группы.</span><span class="sxs-lookup"><span data-stu-id="6ec7b-125">Remove an existing member from the team.</span></span>|
|[<span data-ttu-id="6ec7b-126">Перечисление участников канала</span><span class="sxs-lookup"><span data-stu-id="6ec7b-126">List channel members</span></span>](../api/channel-list-members.md) | <span data-ttu-id="6ec7b-127">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="6ec7b-127">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="6ec7b-128">Получение списка всех участников канала.</span><span class="sxs-lookup"><span data-stu-id="6ec7b-128">Get the list of all members in a channel.</span></span>|
|[<span data-ttu-id="6ec7b-129">Добавление участника канала</span><span class="sxs-lookup"><span data-stu-id="6ec7b-129">Add channel member</span></span>](../api/channel-post-members.md) | [<span data-ttu-id="6ec7b-130">conversationMember</span><span class="sxs-lookup"><span data-stu-id="6ec7b-130">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="6ec7b-131">Добавление участника в канал.</span><span class="sxs-lookup"><span data-stu-id="6ec7b-131">Add a member to a channel.</span></span> <span data-ttu-id="6ec7b-132">Поддерживается только для `channel` с типом членства `private`.</span><span class="sxs-lookup"><span data-stu-id="6ec7b-132">Only supported for `channel` with membershipType of `private`.</span></span>|
|[<span data-ttu-id="6ec7b-133">Получение участника канала</span><span class="sxs-lookup"><span data-stu-id="6ec7b-133">Get channel member</span></span>](../api/channel-get-members.md) | <span data-ttu-id="6ec7b-134">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="6ec7b-134">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="6ec7b-135">Получение участника канала.</span><span class="sxs-lookup"><span data-stu-id="6ec7b-135">Get a member in a channel.</span></span>|
|[<span data-ttu-id="6ec7b-136">Обновление роли участника канала</span><span class="sxs-lookup"><span data-stu-id="6ec7b-136">Update channel member's role</span></span>](../api/channel-update-members.md) | [<span data-ttu-id="6ec7b-137">conversationMember</span><span class="sxs-lookup"><span data-stu-id="6ec7b-137">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="6ec7b-138">Обновление свойства участника канала.</span><span class="sxs-lookup"><span data-stu-id="6ec7b-138">Update the properties of a member of the channel.</span></span> <span data-ttu-id="6ec7b-139">Поддерживается только для канала с типом членства `private`.</span><span class="sxs-lookup"><span data-stu-id="6ec7b-139">Only supported for channel with membershipType of `private`.</span></span>|
|[<span data-ttu-id="6ec7b-140">Удаление участника канала</span><span class="sxs-lookup"><span data-stu-id="6ec7b-140">Remove channel member</span></span>](../api/channel-delete-members.md) | <span data-ttu-id="6ec7b-141">Нет</span><span class="sxs-lookup"><span data-stu-id="6ec7b-141">None</span></span> | <span data-ttu-id="6ec7b-142">Удаление участника канала.</span><span class="sxs-lookup"><span data-stu-id="6ec7b-142">Delete a member from a channel.</span></span> <span data-ttu-id="6ec7b-143">Поддерживается, только если параметру `channelType` присвоено значение `private`.</span><span class="sxs-lookup"><span data-stu-id="6ec7b-143">Only supported for `channelType` of `private`.</span></span>|

## <a name="properties"></a><span data-ttu-id="6ec7b-144">Свойства</span><span class="sxs-lookup"><span data-stu-id="6ec7b-144">Properties</span></span>

| <span data-ttu-id="6ec7b-145">Свойство</span><span class="sxs-lookup"><span data-stu-id="6ec7b-145">Property</span></span>   | <span data-ttu-id="6ec7b-146">Тип</span><span class="sxs-lookup"><span data-stu-id="6ec7b-146">Type</span></span> |<span data-ttu-id="6ec7b-147">Описание</span><span class="sxs-lookup"><span data-stu-id="6ec7b-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6ec7b-148">id</span><span class="sxs-lookup"><span data-stu-id="6ec7b-148">id</span></span>|<span data-ttu-id="6ec7b-149">String</span><span class="sxs-lookup"><span data-stu-id="6ec7b-149">String</span></span>| <span data-ttu-id="6ec7b-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6ec7b-150">Read-only.</span></span> <span data-ttu-id="6ec7b-151">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="6ec7b-151">Unique ID of the user.</span></span>|
|<span data-ttu-id="6ec7b-152">displayName</span><span class="sxs-lookup"><span data-stu-id="6ec7b-152">displayName</span></span>| <span data-ttu-id="6ec7b-153">string</span><span class="sxs-lookup"><span data-stu-id="6ec7b-153">string</span></span> | <span data-ttu-id="6ec7b-154">Отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="6ec7b-154">The display name of the user.</span></span> |
|<span data-ttu-id="6ec7b-155">roles</span><span class="sxs-lookup"><span data-stu-id="6ec7b-155">roles</span></span>| <span data-ttu-id="6ec7b-156">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="6ec7b-156">string collection</span></span> | <span data-ttu-id="6ec7b-157">Роли этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="6ec7b-157">The roles for that user.</span></span> |
|<span data-ttu-id="6ec7b-158">userId</span><span class="sxs-lookup"><span data-stu-id="6ec7b-158">userId</span></span>| <span data-ttu-id="6ec7b-159">строка</span><span class="sxs-lookup"><span data-stu-id="6ec7b-159">string</span></span> | <span data-ttu-id="6ec7b-160">GUID пользователя.</span><span class="sxs-lookup"><span data-stu-id="6ec7b-160">The guid of the user.</span></span> |
|<span data-ttu-id="6ec7b-161">email</span><span class="sxs-lookup"><span data-stu-id="6ec7b-161">email</span></span>| <span data-ttu-id="6ec7b-162">строка</span><span class="sxs-lookup"><span data-stu-id="6ec7b-162">string</span></span>  | <span data-ttu-id="6ec7b-163">Электронный адрес пользователя.</span><span class="sxs-lookup"><span data-stu-id="6ec7b-163">The email address of the user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6ec7b-164">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6ec7b-164">JSON representation</span></span>

<span data-ttu-id="6ec7b-165">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6ec7b-165">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.aadUserConversationMember"
}-->

```json
{
  "id": "string (identifier)",
  "displayName" : "string",
  "roles" : ["string"],
  "userId" : "string",
  "email" : "string"
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

