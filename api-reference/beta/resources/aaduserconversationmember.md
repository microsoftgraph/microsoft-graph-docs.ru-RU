---
title: Тип ресурса aadUserConversationMember
description: Представляет пользователя Azure Active Directory в чате или канале.
localization_priority: Priority
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 058164d44ef6d9d6ba6667cf1cb7249bf57c2a83
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/27/2019
ms.locfileid: "36633512"
---
# <a name="aaduserconversationmember-resource-type"></a><span data-ttu-id="10e26-103">Тип ресурса aadUserConversationMember</span><span class="sxs-lookup"><span data-stu-id="10e26-103">aadUserConversationMember resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10e26-104">Представляет пользователя Azure Active Directory в [чате](chat.md) или [канале](channel.md).</span><span class="sxs-lookup"><span data-stu-id="10e26-104">Represents an Azure Active Directory user in a [chat](chat.md) or [channel](channel.md).</span></span> <span data-ttu-id="10e26-105">Этот тип наследуется от [conversationMember](conversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="10e26-105">This type inherits from [conversationMember](conversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="10e26-106">Методы</span><span class="sxs-lookup"><span data-stu-id="10e26-106">Methods</span></span>

| <span data-ttu-id="10e26-107">Метод</span><span class="sxs-lookup"><span data-stu-id="10e26-107">Method</span></span>       | <span data-ttu-id="10e26-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="10e26-108">Return Type</span></span>  |<span data-ttu-id="10e26-109">Описание</span><span class="sxs-lookup"><span data-stu-id="10e26-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="10e26-110">Перечисление участников</span><span class="sxs-lookup"><span data-stu-id="10e26-110">List members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="10e26-111">Коллекция [conversationmember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="10e26-111">[conversationmember](conversationmember.md) collection</span></span> | <span data-ttu-id="10e26-112">Получение списка всех пользователей в чате или канале.</span><span class="sxs-lookup"><span data-stu-id="10e26-112">Get the list of all users in the chat or channel.</span></span>|
|[<span data-ttu-id="10e26-113">Получение участника</span><span class="sxs-lookup"><span data-stu-id="10e26-113">Get member groups</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="10e26-114">conversationmember</span><span class="sxs-lookup"><span data-stu-id="10e26-114">conversationmember</span></span>](conversationmember.md) | <span data-ttu-id="10e26-115">Получение одного пользователя в чате или канале.</span><span class="sxs-lookup"><span data-stu-id="10e26-115">Get a single user in the chat or channel.</span></span>|
|[<span data-ttu-id="10e26-116">Добавление участника</span><span class="sxs-lookup"><span data-stu-id="10e26-116">Add member</span></span>](../api/conversationmember-add.md) | [<span data-ttu-id="10e26-117">conversationMember</span><span class="sxs-lookup"><span data-stu-id="10e26-117">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="10e26-118">Добавление участника в канал.</span><span class="sxs-lookup"><span data-stu-id="10e26-118">Add a member to a class.</span></span>|
|[<span data-ttu-id="10e26-119">Обновление участника</span><span class="sxs-lookup"><span data-stu-id="10e26-119">Update member</span></span>](../api/conversationmember-update.md) | [<span data-ttu-id="10e26-120">conversationMember</span><span class="sxs-lookup"><span data-stu-id="10e26-120">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="10e26-121">Обновление участника в канале.</span><span class="sxs-lookup"><span data-stu-id="10e26-121">Update a member in the channel.</span></span>|
|[<span data-ttu-id="10e26-122">Удаление участника</span><span class="sxs-lookup"><span data-stu-id="10e26-122">Delete member</span></span>](../api/conversationmember-delete.md) | [<span data-ttu-id="10e26-123">conversationMember</span><span class="sxs-lookup"><span data-stu-id="10e26-123">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="10e26-124">Удаление участника из канала.</span><span class="sxs-lookup"><span data-stu-id="10e26-124">Delete a member from the channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="10e26-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="10e26-125">Properties</span></span>

| <span data-ttu-id="10e26-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="10e26-126">Property</span></span>   | <span data-ttu-id="10e26-127">Тип</span><span class="sxs-lookup"><span data-stu-id="10e26-127">Type</span></span> |<span data-ttu-id="10e26-128">Описание</span><span class="sxs-lookup"><span data-stu-id="10e26-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="10e26-129">id</span><span class="sxs-lookup"><span data-stu-id="10e26-129">id</span></span>|<span data-ttu-id="10e26-130">String</span><span class="sxs-lookup"><span data-stu-id="10e26-130">String</span></span>| <span data-ttu-id="10e26-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="10e26-131">Read-only.</span></span> <span data-ttu-id="10e26-132">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="10e26-132">Unique ID of the message.</span></span>|
|<span data-ttu-id="10e26-133">displayName</span><span class="sxs-lookup"><span data-stu-id="10e26-133">displayName</span></span>| <span data-ttu-id="10e26-134">string</span><span class="sxs-lookup"><span data-stu-id="10e26-134">string</span></span> | <span data-ttu-id="10e26-135">Отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="10e26-135">The display name of the user.</span></span> |
|<span data-ttu-id="10e26-136">roles</span><span class="sxs-lookup"><span data-stu-id="10e26-136">roles</span></span>| <span data-ttu-id="10e26-137">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="10e26-137">string collection</span></span> | <span data-ttu-id="10e26-138">Роли этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="10e26-138">The roles for that user.</span></span> |
|<span data-ttu-id="10e26-139">userId</span><span class="sxs-lookup"><span data-stu-id="10e26-139">userId</span></span>| <span data-ttu-id="10e26-140">строка</span><span class="sxs-lookup"><span data-stu-id="10e26-140">string</span></span> | <span data-ttu-id="10e26-141">GUID пользователя.</span><span class="sxs-lookup"><span data-stu-id="10e26-141">The guid of the user.</span></span> |
|<span data-ttu-id="10e26-142">email</span><span class="sxs-lookup"><span data-stu-id="10e26-142">email</span></span>| <span data-ttu-id="10e26-143">строка</span><span class="sxs-lookup"><span data-stu-id="10e26-143">string</span></span>  | <span data-ttu-id="10e26-144">Электронный адрес пользователя.</span><span class="sxs-lookup"><span data-stu-id="10e26-144">The e-mail address of the user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="10e26-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="10e26-145">JSON representation</span></span>

<span data-ttu-id="10e26-146">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="10e26-146">The following is a JSON representation of the resource.</span></span>

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
