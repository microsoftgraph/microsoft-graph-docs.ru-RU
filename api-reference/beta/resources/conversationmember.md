---
title: Тип ресурса conversationMember
description: Представляет пользователя в беседе.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 796bbe9f64342f97a9ae18363fdc01dc1712d015
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507403"
---
# <a name="conversationmember-resource-type"></a><span data-ttu-id="72e5d-103">Тип ресурса conversationMember</span><span class="sxs-lookup"><span data-stu-id="72e5d-103">conversationMember resource type</span></span>

<span data-ttu-id="72e5d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72e5d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72e5d-105">Представляет пользователя в [чате](chat.md) или [канале](channel.md).</span><span class="sxs-lookup"><span data-stu-id="72e5d-105">Represents a user in a [chat](chat.md) or a [channel](channel.md).</span></span>

## <a name="methods"></a><span data-ttu-id="72e5d-106">Методы</span><span class="sxs-lookup"><span data-stu-id="72e5d-106">Methods</span></span>

| <span data-ttu-id="72e5d-107">Метод</span><span class="sxs-lookup"><span data-stu-id="72e5d-107">Method</span></span>       | <span data-ttu-id="72e5d-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="72e5d-108">Return Type</span></span>  |<span data-ttu-id="72e5d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="72e5d-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="72e5d-110">Список участников чата</span><span class="sxs-lookup"><span data-stu-id="72e5d-110">List Chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="72e5d-111">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="72e5d-111">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="72e5d-112">Получение списка всех пользователей в чате.</span><span class="sxs-lookup"><span data-stu-id="72e5d-112">Get the list of all users in the chat.</span></span>|
|[<span data-ttu-id="72e5d-113">Получение участника чата</span><span class="sxs-lookup"><span data-stu-id="72e5d-113">Get Chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="72e5d-114">conversationMember</span><span class="sxs-lookup"><span data-stu-id="72e5d-114">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="72e5d-115">Получение одного пользователя в чате.</span><span class="sxs-lookup"><span data-stu-id="72e5d-115">Get a single user in the chat.</span></span>|
|[<span data-ttu-id="72e5d-116">Список участников</span><span class="sxs-lookup"><span data-stu-id="72e5d-116">List members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="72e5d-117">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="72e5d-117">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="72e5d-118">Получение списка всех пользователей в чате или канале.</span><span class="sxs-lookup"><span data-stu-id="72e5d-118">Get the list of all users in the chat or channel.</span></span>|
|[<span data-ttu-id="72e5d-119">Получение участника</span><span class="sxs-lookup"><span data-stu-id="72e5d-119">Get member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="72e5d-120">conversationMember</span><span class="sxs-lookup"><span data-stu-id="72e5d-120">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="72e5d-121">Получение одного пользователя в чате или канале.</span><span class="sxs-lookup"><span data-stu-id="72e5d-121">Get a single user in the chat or channel.</span></span>|
|[<span data-ttu-id="72e5d-122">Добавление участника</span><span class="sxs-lookup"><span data-stu-id="72e5d-122">Add member</span></span>](../api/conversationmember-add.md) | [<span data-ttu-id="72e5d-123">conversationMember</span><span class="sxs-lookup"><span data-stu-id="72e5d-123">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="72e5d-124">Добавление участника в канал.</span><span class="sxs-lookup"><span data-stu-id="72e5d-124">Add a member to a channel.</span></span>|
|[<span data-ttu-id="72e5d-125">Обновление участника</span><span class="sxs-lookup"><span data-stu-id="72e5d-125">Update member</span></span>](../api/conversationmember-update.md) | [<span data-ttu-id="72e5d-126">conversationMember</span><span class="sxs-lookup"><span data-stu-id="72e5d-126">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="72e5d-127">Обновление участника в канале.</span><span class="sxs-lookup"><span data-stu-id="72e5d-127">Update a member in the channel.</span></span>|
|[<span data-ttu-id="72e5d-128">Удаление участника</span><span class="sxs-lookup"><span data-stu-id="72e5d-128">Delete member</span></span>](../api/conversationmember-delete.md) | [<span data-ttu-id="72e5d-129">conversationMember</span><span class="sxs-lookup"><span data-stu-id="72e5d-129">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="72e5d-130">Удаление участника из канала.</span><span class="sxs-lookup"><span data-stu-id="72e5d-130">Delete a member from the channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="72e5d-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="72e5d-131">Properties</span></span>

| <span data-ttu-id="72e5d-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="72e5d-132">Property</span></span>   | <span data-ttu-id="72e5d-133">Тип</span><span class="sxs-lookup"><span data-stu-id="72e5d-133">Type</span></span> |<span data-ttu-id="72e5d-134">Описание</span><span class="sxs-lookup"><span data-stu-id="72e5d-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="72e5d-135">id</span><span class="sxs-lookup"><span data-stu-id="72e5d-135">id</span></span>|<span data-ttu-id="72e5d-136">String</span><span class="sxs-lookup"><span data-stu-id="72e5d-136">String</span></span>| <span data-ttu-id="72e5d-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="72e5d-137">Read-only.</span></span> <span data-ttu-id="72e5d-138">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="72e5d-138">Unique ID of the user.</span></span>|
|<span data-ttu-id="72e5d-139">displayName</span><span class="sxs-lookup"><span data-stu-id="72e5d-139">displayName</span></span>| <span data-ttu-id="72e5d-140">string</span><span class="sxs-lookup"><span data-stu-id="72e5d-140">string</span></span> | <span data-ttu-id="72e5d-141">Отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="72e5d-141">The display name of the user.</span></span> |
|<span data-ttu-id="72e5d-142">roles</span><span class="sxs-lookup"><span data-stu-id="72e5d-142">roles</span></span>| <span data-ttu-id="72e5d-143">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="72e5d-143">string collection</span></span> | <span data-ttu-id="72e5d-144">Роли этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="72e5d-144">The roles for that user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="72e5d-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="72e5d-145">JSON representation</span></span>

<span data-ttu-id="72e5d-146">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="72e5d-146">The following is a JSON representation of the resource.</span></span>

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
