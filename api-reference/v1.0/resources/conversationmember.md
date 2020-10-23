---
title: Тип ресурса conversationMember
description: Представляет пользователя в беседе.
localization_priority: Normal
author: laujan
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 970e64ff358654aafee5b47a229a8425fdc69c9e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725836"
---
# <a name="conversationmember-resource-type"></a><span data-ttu-id="2f447-103">Тип ресурса conversationMember</span><span class="sxs-lookup"><span data-stu-id="2f447-103">conversationMember resource type</span></span>

<span data-ttu-id="2f447-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f447-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2f447-105">Представляет пользователя в [команде](team.md).</span><span class="sxs-lookup"><span data-stu-id="2f447-105">Represents a user in a [team](team.md).</span></span>
<span data-ttu-id="2f447-106">См. также [аадусерконверсатионмембер](aaduserconversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="2f447-106">See also [aadUserConversationMember](aaduserconversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="2f447-107">Методы</span><span class="sxs-lookup"><span data-stu-id="2f447-107">Methods</span></span>

| <span data-ttu-id="2f447-108">Метод</span><span class="sxs-lookup"><span data-stu-id="2f447-108">Method</span></span>       | <span data-ttu-id="2f447-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2f447-109">Return Type</span></span>  |<span data-ttu-id="2f447-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2f447-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2f447-111">Перечисление участников</span><span class="sxs-lookup"><span data-stu-id="2f447-111">List members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="2f447-112">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="2f447-112">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="2f447-113">Получение списка всех пользователей в чате или канале.</span><span class="sxs-lookup"><span data-stu-id="2f447-113">Get the list of all users in the chat or channel.</span></span>|
|[<span data-ttu-id="2f447-114">Получение участника</span><span class="sxs-lookup"><span data-stu-id="2f447-114">Get member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="2f447-115">conversationMember</span><span class="sxs-lookup"><span data-stu-id="2f447-115">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="2f447-116">Получение одного пользователя в чате или канале.</span><span class="sxs-lookup"><span data-stu-id="2f447-116">Get a single user in the chat or channel.</span></span>|
|[<span data-ttu-id="2f447-117">Добавление участника</span><span class="sxs-lookup"><span data-stu-id="2f447-117">Add member</span></span>](../api/conversationmember-add.md) | [<span data-ttu-id="2f447-118">conversationMember</span><span class="sxs-lookup"><span data-stu-id="2f447-118">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="2f447-119">Добавление участника в канал.</span><span class="sxs-lookup"><span data-stu-id="2f447-119">Add a member to a channel.</span></span>|
|[<span data-ttu-id="2f447-120">Обновление участника</span><span class="sxs-lookup"><span data-stu-id="2f447-120">Update member</span></span>](../api/conversationmember-update.md) | [<span data-ttu-id="2f447-121">conversationMember</span><span class="sxs-lookup"><span data-stu-id="2f447-121">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="2f447-122">Обновление участника в канале.</span><span class="sxs-lookup"><span data-stu-id="2f447-122">Update a member in the channel.</span></span>|
|[<span data-ttu-id="2f447-123">Удаление участника</span><span class="sxs-lookup"><span data-stu-id="2f447-123">Delete member</span></span>](../api/conversationmember-delete.md) | [<span data-ttu-id="2f447-124">conversationMember</span><span class="sxs-lookup"><span data-stu-id="2f447-124">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="2f447-125">Удаление участника из канала.</span><span class="sxs-lookup"><span data-stu-id="2f447-125">Delete a member from the channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="2f447-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="2f447-126">Properties</span></span>

| <span data-ttu-id="2f447-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="2f447-127">Property</span></span>   | <span data-ttu-id="2f447-128">Тип</span><span class="sxs-lookup"><span data-stu-id="2f447-128">Type</span></span> |<span data-ttu-id="2f447-129">Описание</span><span class="sxs-lookup"><span data-stu-id="2f447-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2f447-130">id</span><span class="sxs-lookup"><span data-stu-id="2f447-130">id</span></span>|<span data-ttu-id="2f447-131">String</span><span class="sxs-lookup"><span data-stu-id="2f447-131">String</span></span>| <span data-ttu-id="2f447-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2f447-132">Read-only.</span></span> <span data-ttu-id="2f447-133">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="2f447-133">Unique ID of the user.</span></span>|
|<span data-ttu-id="2f447-134">displayName</span><span class="sxs-lookup"><span data-stu-id="2f447-134">displayName</span></span>| <span data-ttu-id="2f447-135">string</span><span class="sxs-lookup"><span data-stu-id="2f447-135">string</span></span> | <span data-ttu-id="2f447-136">Отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="2f447-136">The display name of the user.</span></span> |
|<span data-ttu-id="2f447-137">roles</span><span class="sxs-lookup"><span data-stu-id="2f447-137">roles</span></span>| <span data-ttu-id="2f447-138">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="2f447-138">string collection</span></span> | <span data-ttu-id="2f447-139">Роли этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="2f447-139">The roles for that user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2f447-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2f447-140">JSON representation</span></span>

<span data-ttu-id="2f447-141">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2f447-141">The following is a JSON representation of the resource.</span></span>

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

