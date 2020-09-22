---
title: Тип ресурса conversationMember
description: Представляет пользователя в беседе.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d9e50c0ca27843461b41b4d86f29ce3604788866
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016769"
---
# <a name="conversationmember-resource-type"></a><span data-ttu-id="c200a-103">Тип ресурса conversationMember</span><span class="sxs-lookup"><span data-stu-id="c200a-103">conversationMember resource type</span></span>

<span data-ttu-id="c200a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c200a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c200a-105">Представляет пользователя в [чате](chat.md) или [канале](channel.md).</span><span class="sxs-lookup"><span data-stu-id="c200a-105">Represents a user in a [chat](chat.md) or a [channel](channel.md).</span></span>
<span data-ttu-id="c200a-106">См. также [аадусерконверсатионмембер](aaduserconversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="c200a-106">See also [aadUserConversationMember](aaduserconversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="c200a-107">Методы</span><span class="sxs-lookup"><span data-stu-id="c200a-107">Methods</span></span>

| <span data-ttu-id="c200a-108">Метод</span><span class="sxs-lookup"><span data-stu-id="c200a-108">Method</span></span>       | <span data-ttu-id="c200a-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c200a-109">Return Type</span></span>  |<span data-ttu-id="c200a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c200a-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c200a-111">Список участников чата</span><span class="sxs-lookup"><span data-stu-id="c200a-111">List Chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="c200a-112">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="c200a-112">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="c200a-113">Получение списка всех пользователей в чате.</span><span class="sxs-lookup"><span data-stu-id="c200a-113">Get the list of all users in the chat.</span></span>|
|[<span data-ttu-id="c200a-114">Получение участника чата</span><span class="sxs-lookup"><span data-stu-id="c200a-114">Get Chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="c200a-115">conversationMember</span><span class="sxs-lookup"><span data-stu-id="c200a-115">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="c200a-116">Получение одного пользователя в чате.</span><span class="sxs-lookup"><span data-stu-id="c200a-116">Get a single user in the chat.</span></span>|
|[<span data-ttu-id="c200a-117">Список участников</span><span class="sxs-lookup"><span data-stu-id="c200a-117">List members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="c200a-118">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="c200a-118">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="c200a-119">Получение списка всех пользователей в чате или канале.</span><span class="sxs-lookup"><span data-stu-id="c200a-119">Get the list of all users in the chat or channel.</span></span>|
|[<span data-ttu-id="c200a-120">Получение участника</span><span class="sxs-lookup"><span data-stu-id="c200a-120">Get member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="c200a-121">conversationMember</span><span class="sxs-lookup"><span data-stu-id="c200a-121">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="c200a-122">Получение одного пользователя в чате или канале.</span><span class="sxs-lookup"><span data-stu-id="c200a-122">Get a single user in the chat or channel.</span></span>|
|[<span data-ttu-id="c200a-123">Добавление участника</span><span class="sxs-lookup"><span data-stu-id="c200a-123">Add member</span></span>](../api/conversationmember-add.md) | [<span data-ttu-id="c200a-124">conversationMember</span><span class="sxs-lookup"><span data-stu-id="c200a-124">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="c200a-125">Добавление участника в канал.</span><span class="sxs-lookup"><span data-stu-id="c200a-125">Add a member to a channel.</span></span>|
|[<span data-ttu-id="c200a-126">Обновление участника</span><span class="sxs-lookup"><span data-stu-id="c200a-126">Update member</span></span>](../api/conversationmember-update.md) | [<span data-ttu-id="c200a-127">conversationMember</span><span class="sxs-lookup"><span data-stu-id="c200a-127">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="c200a-128">Обновление участника в канале.</span><span class="sxs-lookup"><span data-stu-id="c200a-128">Update a member in the channel.</span></span>|
|[<span data-ttu-id="c200a-129">Удаление участника</span><span class="sxs-lookup"><span data-stu-id="c200a-129">Delete member</span></span>](../api/conversationmember-delete.md) | [<span data-ttu-id="c200a-130">conversationMember</span><span class="sxs-lookup"><span data-stu-id="c200a-130">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="c200a-131">Удаление участника из канала.</span><span class="sxs-lookup"><span data-stu-id="c200a-131">Delete a member from the channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="c200a-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="c200a-132">Properties</span></span>

| <span data-ttu-id="c200a-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="c200a-133">Property</span></span>   | <span data-ttu-id="c200a-134">Тип</span><span class="sxs-lookup"><span data-stu-id="c200a-134">Type</span></span> |<span data-ttu-id="c200a-135">Описание</span><span class="sxs-lookup"><span data-stu-id="c200a-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c200a-136">id</span><span class="sxs-lookup"><span data-stu-id="c200a-136">id</span></span>|<span data-ttu-id="c200a-137">String</span><span class="sxs-lookup"><span data-stu-id="c200a-137">String</span></span>| <span data-ttu-id="c200a-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c200a-138">Read-only.</span></span> <span data-ttu-id="c200a-139">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="c200a-139">Unique ID of the user.</span></span>|
|<span data-ttu-id="c200a-140">displayName</span><span class="sxs-lookup"><span data-stu-id="c200a-140">displayName</span></span>| <span data-ttu-id="c200a-141">string</span><span class="sxs-lookup"><span data-stu-id="c200a-141">string</span></span> | <span data-ttu-id="c200a-142">Отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="c200a-142">The display name of the user.</span></span> |
|<span data-ttu-id="c200a-143">roles</span><span class="sxs-lookup"><span data-stu-id="c200a-143">roles</span></span>| <span data-ttu-id="c200a-144">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c200a-144">string collection</span></span> | <span data-ttu-id="c200a-145">Роли этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="c200a-145">The roles for that user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c200a-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c200a-146">JSON representation</span></span>

<span data-ttu-id="c200a-147">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c200a-147">The following is a JSON representation of the resource.</span></span>

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


