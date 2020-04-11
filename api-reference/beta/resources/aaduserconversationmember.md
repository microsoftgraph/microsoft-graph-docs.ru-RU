---
title: Тип ресурса aadUserConversationMember
description: Представляет пользователя Azure Active Directory в чате или канале.
localization_priority: Priority
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: caf8336d58ee40fcc1bf51b569cf334ba99294fc
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43228354"
---
# <a name="aaduserconversationmember-resource-type"></a><span data-ttu-id="d59f9-103">Тип ресурса aadUserConversationMember</span><span class="sxs-lookup"><span data-stu-id="d59f9-103">aadUserConversationMember resource type</span></span>

<span data-ttu-id="d59f9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d59f9-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="d59f9-105">Представляет пользователя Azure Active Directory в [чате](chat.md) или [канале](channel.md).</span><span class="sxs-lookup"><span data-stu-id="d59f9-105">Represents an Azure Active Directory user in a [chat](chat.md) or [channel](channel.md).</span></span> <span data-ttu-id="d59f9-106">Этот тип наследуется от [conversationMember](conversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="d59f9-106">This type inherits from [conversationMember](conversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="d59f9-107">Методы</span><span class="sxs-lookup"><span data-stu-id="d59f9-107">Methods</span></span>

| <span data-ttu-id="d59f9-108">Метод</span><span class="sxs-lookup"><span data-stu-id="d59f9-108">Method</span></span>       | <span data-ttu-id="d59f9-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d59f9-109">Return Type</span></span>  |<span data-ttu-id="d59f9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d59f9-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d59f9-111">Перечисление участников</span><span class="sxs-lookup"><span data-stu-id="d59f9-111">List members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="d59f9-112">Коллекция [conversationmember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="d59f9-112">[conversationmember](conversationmember.md) collection</span></span> | <span data-ttu-id="d59f9-113">Получение списка всех пользователей в чате или канале.</span><span class="sxs-lookup"><span data-stu-id="d59f9-113">Get the list of all users in the chat or channel.</span></span>|
|[<span data-ttu-id="d59f9-114">Получение участника</span><span class="sxs-lookup"><span data-stu-id="d59f9-114">Get member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="d59f9-115">conversationmember</span><span class="sxs-lookup"><span data-stu-id="d59f9-115">conversationmember</span></span>](conversationmember.md) | <span data-ttu-id="d59f9-116">Получение одного пользователя в чате или канале.</span><span class="sxs-lookup"><span data-stu-id="d59f9-116">Get a single user in the chat or channel.</span></span>|
|[<span data-ttu-id="d59f9-117">Добавление участника</span><span class="sxs-lookup"><span data-stu-id="d59f9-117">Add member</span></span>](../api/conversationmember-add.md) | [<span data-ttu-id="d59f9-118">conversationMember</span><span class="sxs-lookup"><span data-stu-id="d59f9-118">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="d59f9-119">Добавление участника в канал.</span><span class="sxs-lookup"><span data-stu-id="d59f9-119">Add a member to a channel.</span></span>|
|[<span data-ttu-id="d59f9-120">Обновление участника</span><span class="sxs-lookup"><span data-stu-id="d59f9-120">Update member</span></span>](../api/conversationmember-update.md) | [<span data-ttu-id="d59f9-121">conversationMember</span><span class="sxs-lookup"><span data-stu-id="d59f9-121">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="d59f9-122">Обновление участника в канале.</span><span class="sxs-lookup"><span data-stu-id="d59f9-122">Update a member in the channel.</span></span>|
|[<span data-ttu-id="d59f9-123">Удаление участника</span><span class="sxs-lookup"><span data-stu-id="d59f9-123">Delete member</span></span>](../api/conversationmember-delete.md) | [<span data-ttu-id="d59f9-124">conversationMember</span><span class="sxs-lookup"><span data-stu-id="d59f9-124">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="d59f9-125">Удаление участника из канала.</span><span class="sxs-lookup"><span data-stu-id="d59f9-125">Delete a member from the channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="d59f9-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="d59f9-126">Properties</span></span>

| <span data-ttu-id="d59f9-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="d59f9-127">Property</span></span>   | <span data-ttu-id="d59f9-128">Тип</span><span class="sxs-lookup"><span data-stu-id="d59f9-128">Type</span></span> |<span data-ttu-id="d59f9-129">Описание</span><span class="sxs-lookup"><span data-stu-id="d59f9-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d59f9-130">id</span><span class="sxs-lookup"><span data-stu-id="d59f9-130">id</span></span>|<span data-ttu-id="d59f9-131">String</span><span class="sxs-lookup"><span data-stu-id="d59f9-131">String</span></span>| <span data-ttu-id="d59f9-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d59f9-132">Read-only.</span></span> <span data-ttu-id="d59f9-133">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="d59f9-133">Unique ID of the user.</span></span>|
|<span data-ttu-id="d59f9-134">displayName</span><span class="sxs-lookup"><span data-stu-id="d59f9-134">displayName</span></span>| <span data-ttu-id="d59f9-135">string</span><span class="sxs-lookup"><span data-stu-id="d59f9-135">string</span></span> | <span data-ttu-id="d59f9-136">Отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="d59f9-136">The display name of the user.</span></span> |
|<span data-ttu-id="d59f9-137">roles</span><span class="sxs-lookup"><span data-stu-id="d59f9-137">roles</span></span>| <span data-ttu-id="d59f9-138">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d59f9-138">string collection</span></span> | <span data-ttu-id="d59f9-139">Роли этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="d59f9-139">The roles for that user.</span></span> |
|<span data-ttu-id="d59f9-140">userId</span><span class="sxs-lookup"><span data-stu-id="d59f9-140">userId</span></span>| <span data-ttu-id="d59f9-141">строка</span><span class="sxs-lookup"><span data-stu-id="d59f9-141">string</span></span> | <span data-ttu-id="d59f9-142">GUID пользователя.</span><span class="sxs-lookup"><span data-stu-id="d59f9-142">The guid of the user.</span></span> |
|<span data-ttu-id="d59f9-143">email</span><span class="sxs-lookup"><span data-stu-id="d59f9-143">email</span></span>| <span data-ttu-id="d59f9-144">строка</span><span class="sxs-lookup"><span data-stu-id="d59f9-144">string</span></span>  | <span data-ttu-id="d59f9-145">Электронный адрес пользователя.</span><span class="sxs-lookup"><span data-stu-id="d59f9-145">The email address of the user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d59f9-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d59f9-146">JSON representation</span></span>

<span data-ttu-id="d59f9-147">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d59f9-147">The following is a JSON representation of the resource.</span></span>

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
