---
title: Тип ресурса aadUserConversationMember
description: Представляет пользователя Azure Active Directory в чате или канале.
localization_priority: Priority
author: laujan
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 6057c8cf71ce0f8d71632267d3790c39b69b1eb1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735766"
---
# <a name="aaduserconversationmember-resource-type"></a><span data-ttu-id="9fba2-103">Тип ресурса aadUserConversationMember</span><span class="sxs-lookup"><span data-stu-id="9fba2-103">aadUserConversationMember resource type</span></span>

<span data-ttu-id="9fba2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9fba2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9fba2-105">Представляет пользователя Azure Active Directory в [команде](team.md).</span><span class="sxs-lookup"><span data-stu-id="9fba2-105">Represents an Azure Active Directory user in a [team](team.md).</span></span>
<span data-ttu-id="9fba2-106">Этот тип наследуется от [conversationMember](conversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="9fba2-106">This type inherits from [conversationMember](conversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="9fba2-107">Методы</span><span class="sxs-lookup"><span data-stu-id="9fba2-107">Methods</span></span>

| <span data-ttu-id="9fba2-108">Метод</span><span class="sxs-lookup"><span data-stu-id="9fba2-108">Method</span></span>       | <span data-ttu-id="9fba2-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9fba2-109">Return Type</span></span>  |<span data-ttu-id="9fba2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9fba2-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9fba2-111">Перечисление участников</span><span class="sxs-lookup"><span data-stu-id="9fba2-111">List members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="9fba2-112">Коллекция [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="9fba2-112">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="9fba2-113">Получение списка всех пользователей в чате или канале.</span><span class="sxs-lookup"><span data-stu-id="9fba2-113">Get the list of all users in the chat or channel.</span></span>|
|[<span data-ttu-id="9fba2-114">Получение участника</span><span class="sxs-lookup"><span data-stu-id="9fba2-114">Get member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="9fba2-115">conversationMember</span><span class="sxs-lookup"><span data-stu-id="9fba2-115">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="9fba2-116">Получение одного пользователя в чате или канале.</span><span class="sxs-lookup"><span data-stu-id="9fba2-116">Get a single user in the chat or channel.</span></span>|
|[<span data-ttu-id="9fba2-117">Добавление участника</span><span class="sxs-lookup"><span data-stu-id="9fba2-117">Add member</span></span>](../api/conversationmember-add.md) | [<span data-ttu-id="9fba2-118">conversationMember</span><span class="sxs-lookup"><span data-stu-id="9fba2-118">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="9fba2-119">Добавление участника в канал.</span><span class="sxs-lookup"><span data-stu-id="9fba2-119">Add a member to a channel.</span></span>|
|[<span data-ttu-id="9fba2-120">Обновление участника</span><span class="sxs-lookup"><span data-stu-id="9fba2-120">Update member</span></span>](../api/conversationmember-update.md) | [<span data-ttu-id="9fba2-121">conversationMember</span><span class="sxs-lookup"><span data-stu-id="9fba2-121">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="9fba2-122">Обновление участника в канале.</span><span class="sxs-lookup"><span data-stu-id="9fba2-122">Update a member in the channel.</span></span>|
|[<span data-ttu-id="9fba2-123">Удаление участника</span><span class="sxs-lookup"><span data-stu-id="9fba2-123">Delete member</span></span>](../api/conversationmember-delete.md) | [<span data-ttu-id="9fba2-124">conversationMember</span><span class="sxs-lookup"><span data-stu-id="9fba2-124">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="9fba2-125">Удаление участника из канала.</span><span class="sxs-lookup"><span data-stu-id="9fba2-125">Delete a member from the channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="9fba2-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="9fba2-126">Properties</span></span>

| <span data-ttu-id="9fba2-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="9fba2-127">Property</span></span>   | <span data-ttu-id="9fba2-128">Тип</span><span class="sxs-lookup"><span data-stu-id="9fba2-128">Type</span></span> |<span data-ttu-id="9fba2-129">Описание</span><span class="sxs-lookup"><span data-stu-id="9fba2-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9fba2-130">id</span><span class="sxs-lookup"><span data-stu-id="9fba2-130">id</span></span>|<span data-ttu-id="9fba2-131">String</span><span class="sxs-lookup"><span data-stu-id="9fba2-131">String</span></span>| <span data-ttu-id="9fba2-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9fba2-132">Read-only.</span></span> <span data-ttu-id="9fba2-133">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="9fba2-133">Unique ID of the user.</span></span>|
|<span data-ttu-id="9fba2-134">displayName</span><span class="sxs-lookup"><span data-stu-id="9fba2-134">displayName</span></span>| <span data-ttu-id="9fba2-135">string</span><span class="sxs-lookup"><span data-stu-id="9fba2-135">string</span></span> | <span data-ttu-id="9fba2-136">Отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="9fba2-136">The display name of the user.</span></span> |
|<span data-ttu-id="9fba2-137">roles</span><span class="sxs-lookup"><span data-stu-id="9fba2-137">roles</span></span>| <span data-ttu-id="9fba2-138">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9fba2-138">string collection</span></span> | <span data-ttu-id="9fba2-139">Роли этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="9fba2-139">The roles for that user.</span></span> |
|<span data-ttu-id="9fba2-140">userId</span><span class="sxs-lookup"><span data-stu-id="9fba2-140">userId</span></span>| <span data-ttu-id="9fba2-141">строка</span><span class="sxs-lookup"><span data-stu-id="9fba2-141">string</span></span> | <span data-ttu-id="9fba2-142">GUID пользователя.</span><span class="sxs-lookup"><span data-stu-id="9fba2-142">The guid of the user.</span></span> |
|<span data-ttu-id="9fba2-143">email</span><span class="sxs-lookup"><span data-stu-id="9fba2-143">email</span></span>| <span data-ttu-id="9fba2-144">строка</span><span class="sxs-lookup"><span data-stu-id="9fba2-144">string</span></span>  | <span data-ttu-id="9fba2-145">Электронный адрес пользователя.</span><span class="sxs-lookup"><span data-stu-id="9fba2-145">The email address of the user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9fba2-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9fba2-146">JSON representation</span></span>

<span data-ttu-id="9fba2-147">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9fba2-147">The following is a JSON representation of the resource.</span></span>

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

