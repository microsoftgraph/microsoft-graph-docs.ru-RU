---
title: Тип ресурса aadUserConversationMember
description: Представляет пользователя Azure Active Directory в чате или канале.
localization_priority: Priority
author: laujan
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c7e989adcafd4752dea6d2fca82ecfa7638bf1ec
ms.sourcegitcommit: 0d4377b0153bc339ab7b3b1a6ee4d52848b622d4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2020
ms.locfileid: "49714125"
---
# <a name="aaduserconversationmember-resource-type"></a><span data-ttu-id="13171-103">Тип ресурса aadUserConversationMember</span><span class="sxs-lookup"><span data-stu-id="13171-103">aadUserConversationMember resource type</span></span>

<span data-ttu-id="13171-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13171-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="13171-105">Представляет пользователя Azure Active Directory в [команде](team.md), [канале](channel.md) или [чате](chat.md).</span><span class="sxs-lookup"><span data-stu-id="13171-105">Represents an Azure Active Directory user in a [team](team.md), a [channel](channel.md), or a [chat](chat.md).</span></span>
<span data-ttu-id="13171-106">Этот тип наследуется от [conversationMember](conversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="13171-106">This type inherits from [conversationMember](conversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="13171-107">Методы</span><span class="sxs-lookup"><span data-stu-id="13171-107">Methods</span></span>

| <span data-ttu-id="13171-108">Метод</span><span class="sxs-lookup"><span data-stu-id="13171-108">Method</span></span>       | <span data-ttu-id="13171-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="13171-109">Return Type</span></span>  |<span data-ttu-id="13171-110">Описание</span><span class="sxs-lookup"><span data-stu-id="13171-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="13171-111">Список участников группы</span><span class="sxs-lookup"><span data-stu-id="13171-111">List team members</span></span>](../api/team-list-members.md)|<span data-ttu-id="13171-112">Коллекция [conversationMember](../resources/conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="13171-112">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="13171-113">Получение списка участников группы.</span><span class="sxs-lookup"><span data-stu-id="13171-113">Get the list of members in the team.</span></span>|
|[<span data-ttu-id="13171-114">Добавление участника в команду</span><span class="sxs-lookup"><span data-stu-id="13171-114">Add team member</span></span>](../api/team-post-members.md)|[<span data-ttu-id="13171-115">conversationMember</span><span class="sxs-lookup"><span data-stu-id="13171-115">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="13171-116">Добавление нового участника в группу.</span><span class="sxs-lookup"><span data-stu-id="13171-116">Add a new member to the team.</span></span>|
|[<span data-ttu-id="13171-117">Получение участника группы</span><span class="sxs-lookup"><span data-stu-id="13171-117">Get team member</span></span>](../api/team-get-members.md) | <span data-ttu-id="13171-118">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="13171-118">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="13171-119">Получение участника группы.</span><span class="sxs-lookup"><span data-stu-id="13171-119">Get a member in the team.</span></span>|
|[<span data-ttu-id="13171-120">Обновление роли участника команды</span><span class="sxs-lookup"><span data-stu-id="13171-120">Update team member's role</span></span>](../api/team-update-members.md)|[<span data-ttu-id="13171-121">conversationMember</span><span class="sxs-lookup"><span data-stu-id="13171-121">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="13171-122">Перевод пользователя из категории участников в категорию владельцев или наоборот, из категории владельцев в категорию обычных участников.</span><span class="sxs-lookup"><span data-stu-id="13171-122">Change a member to an owner or back to a regular member.</span></span>|
|[<span data-ttu-id="13171-123">Удаление участника группы</span><span class="sxs-lookup"><span data-stu-id="13171-123">Remove team member</span></span>](../api/team-delete-members.md)|<span data-ttu-id="13171-124">Нет</span><span class="sxs-lookup"><span data-stu-id="13171-124">None</span></span>|<span data-ttu-id="13171-125">Удаление существующего участника из группы.</span><span class="sxs-lookup"><span data-stu-id="13171-125">Remove an existing member from the team.</span></span>|
|[<span data-ttu-id="13171-126">Перечисление участников канала</span><span class="sxs-lookup"><span data-stu-id="13171-126">List channel members</span></span>](../api/channel-list-members.md) | <span data-ttu-id="13171-127">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="13171-127">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="13171-128">Получение списка всех участников канала.</span><span class="sxs-lookup"><span data-stu-id="13171-128">Get the list of all members in a channel.</span></span>|
|[<span data-ttu-id="13171-129">Добавление участника канала</span><span class="sxs-lookup"><span data-stu-id="13171-129">Add channel member</span></span>](../api/channel-post-members.md) | [<span data-ttu-id="13171-130">conversationMember</span><span class="sxs-lookup"><span data-stu-id="13171-130">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="13171-131">Добавление участника в канал.</span><span class="sxs-lookup"><span data-stu-id="13171-131">Add a member to a channel.</span></span> <span data-ttu-id="13171-132">Поддерживается только для `channel` с типом членства `private`.</span><span class="sxs-lookup"><span data-stu-id="13171-132">Only supported for `channel`with membershipType of `private`.</span></span>|
|[<span data-ttu-id="13171-133">Получение участника канала</span><span class="sxs-lookup"><span data-stu-id="13171-133">Get channel member</span></span>](../api/channel-get-members.md) | <span data-ttu-id="13171-134">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="13171-134">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="13171-135">Получение участника канала.</span><span class="sxs-lookup"><span data-stu-id="13171-135">Get a member in a channel.</span></span>|
|[<span data-ttu-id="13171-136">Обновление роли участника канала</span><span class="sxs-lookup"><span data-stu-id="13171-136">Update channel member's role</span></span>](../api/channel-update-members.md) | [<span data-ttu-id="13171-137">conversationMember</span><span class="sxs-lookup"><span data-stu-id="13171-137">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="13171-138">Обновление свойства участника канала.</span><span class="sxs-lookup"><span data-stu-id="13171-138">Update the properties of a member of the channel.</span></span> <span data-ttu-id="13171-139">Поддерживается только для канала с типом членства `private`.</span><span class="sxs-lookup"><span data-stu-id="13171-139">Only supported for channel with membershipType of `private`.</span></span>|
|[<span data-ttu-id="13171-140">Удаление участника канала</span><span class="sxs-lookup"><span data-stu-id="13171-140">Remove channel member</span></span>](../api/channel-delete-members.md) | <span data-ttu-id="13171-141">Нет</span><span class="sxs-lookup"><span data-stu-id="13171-141">None</span></span> | <span data-ttu-id="13171-142">Удаление участника канала.</span><span class="sxs-lookup"><span data-stu-id="13171-142">Delete a member from a channel.</span></span> <span data-ttu-id="13171-143">Поддерживается, только если параметру `channelType` присвоено значение `private`.</span><span class="sxs-lookup"><span data-stu-id="13171-143">Only supported for `channelType` of `private`.</span></span>|

## <a name="properties"></a><span data-ttu-id="13171-144">Свойства</span><span class="sxs-lookup"><span data-stu-id="13171-144">Properties</span></span>

| <span data-ttu-id="13171-145">Свойство</span><span class="sxs-lookup"><span data-stu-id="13171-145">Property</span></span>   | <span data-ttu-id="13171-146">Тип</span><span class="sxs-lookup"><span data-stu-id="13171-146">Type</span></span> |<span data-ttu-id="13171-147">Описание</span><span class="sxs-lookup"><span data-stu-id="13171-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="13171-148">id</span><span class="sxs-lookup"><span data-stu-id="13171-148">id</span></span>|<span data-ttu-id="13171-149">String</span><span class="sxs-lookup"><span data-stu-id="13171-149">String</span></span>| <span data-ttu-id="13171-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="13171-150">Read-only.</span></span> <span data-ttu-id="13171-151">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="13171-151">Unique ID of the user.</span></span>|
|<span data-ttu-id="13171-152">displayName</span><span class="sxs-lookup"><span data-stu-id="13171-152">displayName</span></span>| <span data-ttu-id="13171-153">string</span><span class="sxs-lookup"><span data-stu-id="13171-153">string</span></span> | <span data-ttu-id="13171-154">Отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="13171-154">The display name of the user.</span></span> |
|<span data-ttu-id="13171-155">roles</span><span class="sxs-lookup"><span data-stu-id="13171-155">roles</span></span>| <span data-ttu-id="13171-156">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="13171-156">string collection</span></span> | <span data-ttu-id="13171-157">Роли этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="13171-157">The roles for that user.</span></span> |
|<span data-ttu-id="13171-158">userId</span><span class="sxs-lookup"><span data-stu-id="13171-158">userId</span></span>| <span data-ttu-id="13171-159">строка</span><span class="sxs-lookup"><span data-stu-id="13171-159">string</span></span> | <span data-ttu-id="13171-160">GUID пользователя.</span><span class="sxs-lookup"><span data-stu-id="13171-160">The guid of the user.</span></span> |
|<span data-ttu-id="13171-161">email</span><span class="sxs-lookup"><span data-stu-id="13171-161">email</span></span>| <span data-ttu-id="13171-162">строка</span><span class="sxs-lookup"><span data-stu-id="13171-162">string</span></span>  | <span data-ttu-id="13171-163">Электронный адрес пользователя.</span><span class="sxs-lookup"><span data-stu-id="13171-163">The email address of the user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="13171-164">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="13171-164">JSON representation</span></span>

<span data-ttu-id="13171-165">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="13171-165">The following is a JSON representation of the resource.</span></span>

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

