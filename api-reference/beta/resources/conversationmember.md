---
title: Тип ресурса conversationMember
description: Представляет пользователя в беседе.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9e20a1aa0ef42f41a3fc300f804bb5477b5fe1cb
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/27/2019
ms.locfileid: "36633701"
---
# <a name="conversationmember-resource-type"></a><span data-ttu-id="3b99f-103">Тип ресурса conversationMember</span><span class="sxs-lookup"><span data-stu-id="3b99f-103">conversationMember resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b99f-104">Представляет пользователя в [чате](chat.md) или [канале](channel.md).</span><span class="sxs-lookup"><span data-stu-id="3b99f-104">Represents a user in a [chat](chat.md) or a [channel](channel.md).</span></span>

## <a name="methods"></a><span data-ttu-id="3b99f-105">Методы</span><span class="sxs-lookup"><span data-stu-id="3b99f-105">Methods</span></span>

| <span data-ttu-id="3b99f-106">Метод</span><span class="sxs-lookup"><span data-stu-id="3b99f-106">Method</span></span>       | <span data-ttu-id="3b99f-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3b99f-107">Return Type</span></span>  |<span data-ttu-id="3b99f-108">Описание</span><span class="sxs-lookup"><span data-stu-id="3b99f-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3b99f-109">Список участников чата</span><span class="sxs-lookup"><span data-stu-id="3b99f-109">List Chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="3b99f-110">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="3b99f-110">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="3b99f-111">Получение списка всех пользователей в чате.</span><span class="sxs-lookup"><span data-stu-id="3b99f-111">Get the list of all users in the chat.</span></span>|
|[<span data-ttu-id="3b99f-112">Получение участника чата</span><span class="sxs-lookup"><span data-stu-id="3b99f-112">Get Chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="3b99f-113">conversationMember</span><span class="sxs-lookup"><span data-stu-id="3b99f-113">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="3b99f-114">Получение одного пользователя в чате.</span><span class="sxs-lookup"><span data-stu-id="3b99f-114">Get a single user in the chat.</span></span>|
|[<span data-ttu-id="3b99f-115">Список участников</span><span class="sxs-lookup"><span data-stu-id="3b99f-115">List members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="3b99f-116">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="3b99f-116">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="3b99f-117">Получение списка всех пользователей в чате или канале.</span><span class="sxs-lookup"><span data-stu-id="3b99f-117">Get the list of all users in the chat or channel.</span></span>|
|[<span data-ttu-id="3b99f-118">Получение участника</span><span class="sxs-lookup"><span data-stu-id="3b99f-118">Get member groups</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="3b99f-119">conversationMember</span><span class="sxs-lookup"><span data-stu-id="3b99f-119">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="3b99f-120">Получение одного пользователя в чате или канале.</span><span class="sxs-lookup"><span data-stu-id="3b99f-120">Get a single user in the chat or channel.</span></span>|
|[<span data-ttu-id="3b99f-121">Добавление участника</span><span class="sxs-lookup"><span data-stu-id="3b99f-121">Add member</span></span>](../api/conversationmember-add.md) | [<span data-ttu-id="3b99f-122">conversationMember</span><span class="sxs-lookup"><span data-stu-id="3b99f-122">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="3b99f-123">Добавление участника в канал.</span><span class="sxs-lookup"><span data-stu-id="3b99f-123">Add a member to a class.</span></span>|
|[<span data-ttu-id="3b99f-124">Обновление участника</span><span class="sxs-lookup"><span data-stu-id="3b99f-124">Update member</span></span>](../api/conversationmember-update.md) | [<span data-ttu-id="3b99f-125">conversationMember</span><span class="sxs-lookup"><span data-stu-id="3b99f-125">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="3b99f-126">Обновление участника в канале.</span><span class="sxs-lookup"><span data-stu-id="3b99f-126">Update a member in the channel.</span></span>|
|[<span data-ttu-id="3b99f-127">Удаление участника</span><span class="sxs-lookup"><span data-stu-id="3b99f-127">Delete member</span></span>](../api/conversationmember-delete.md) | [<span data-ttu-id="3b99f-128">conversationMember</span><span class="sxs-lookup"><span data-stu-id="3b99f-128">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="3b99f-129">Удаление участника из канала.</span><span class="sxs-lookup"><span data-stu-id="3b99f-129">Delete a member from the channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="3b99f-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="3b99f-130">Properties</span></span>

| <span data-ttu-id="3b99f-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="3b99f-131">Property</span></span>   | <span data-ttu-id="3b99f-132">Тип</span><span class="sxs-lookup"><span data-stu-id="3b99f-132">Type</span></span> |<span data-ttu-id="3b99f-133">Описание</span><span class="sxs-lookup"><span data-stu-id="3b99f-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3b99f-134">id</span><span class="sxs-lookup"><span data-stu-id="3b99f-134">id</span></span>|<span data-ttu-id="3b99f-135">String</span><span class="sxs-lookup"><span data-stu-id="3b99f-135">String</span></span>| <span data-ttu-id="3b99f-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3b99f-136">Read-only.</span></span> <span data-ttu-id="3b99f-137">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="3b99f-137">Unique ID of the message.</span></span>|
|<span data-ttu-id="3b99f-138">displayName</span><span class="sxs-lookup"><span data-stu-id="3b99f-138">displayName</span></span>| <span data-ttu-id="3b99f-139">string</span><span class="sxs-lookup"><span data-stu-id="3b99f-139">string</span></span> | <span data-ttu-id="3b99f-140">Отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="3b99f-140">The display name of the user.</span></span> |
|<span data-ttu-id="3b99f-141">roles</span><span class="sxs-lookup"><span data-stu-id="3b99f-141">roles</span></span>| <span data-ttu-id="3b99f-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="3b99f-142">string collection</span></span> | <span data-ttu-id="3b99f-143">Роли этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="3b99f-143">The roles for that user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3b99f-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3b99f-144">JSON representation</span></span>

<span data-ttu-id="3b99f-145">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3b99f-145">The following is a JSON representation of the resource.</span></span>

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
