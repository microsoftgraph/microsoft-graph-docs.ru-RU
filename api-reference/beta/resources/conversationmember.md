---
title: Тип ресурса conversationMember
description: Представляет пользователя в беседе.
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: f6908106390e527ab4e33e777dd232b58ead727a
ms.sourcegitcommit: afea19508ad74a3583b11b5f7b544c53eafb3740
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/22/2019
ms.locfileid: "34379306"
---
# <a name="conversationmember-resource-type"></a><span data-ttu-id="d30ba-103">Тип ресурса conversationMember</span><span class="sxs-lookup"><span data-stu-id="d30ba-103">conversationMember resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d30ba-104">Представляет пользователя в [чате](chat.md).</span><span class="sxs-lookup"><span data-stu-id="d30ba-104">Represents a user in a [chat](chat.md).</span></span>

## <a name="methods"></a><span data-ttu-id="d30ba-105">Методы</span><span class="sxs-lookup"><span data-stu-id="d30ba-105">Methods</span></span>

| <span data-ttu-id="d30ba-106">Метод</span><span class="sxs-lookup"><span data-stu-id="d30ba-106">Method</span></span>       | <span data-ttu-id="d30ba-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d30ba-107">Return Type</span></span>  |<span data-ttu-id="d30ba-108">Описание</span><span class="sxs-lookup"><span data-stu-id="d30ba-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d30ba-109">Список участников чата</span><span class="sxs-lookup"><span data-stu-id="d30ba-109">List Chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="d30ba-110">Коллекция [conversationmember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="d30ba-110">[conversationmember](conversationmember.md) collection</span></span> | <span data-ttu-id="d30ba-111">Получение списка всех пользователей в чате.</span><span class="sxs-lookup"><span data-stu-id="d30ba-111">Get the list of all users in the chat.</span></span>|
|[<span data-ttu-id="d30ba-112">Получение участника чата</span><span class="sxs-lookup"><span data-stu-id="d30ba-112">Get Chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="d30ba-113">conversationmember</span><span class="sxs-lookup"><span data-stu-id="d30ba-113">conversationmember</span></span>](conversationmember.md) | <span data-ttu-id="d30ba-114">Получение одного пользователя в чате.</span><span class="sxs-lookup"><span data-stu-id="d30ba-114">Get a single user in the chat.</span></span>|

## <a name="properties"></a><span data-ttu-id="d30ba-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="d30ba-115">Properties</span></span>
| <span data-ttu-id="d30ba-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="d30ba-116">Property</span></span>     | <span data-ttu-id="d30ba-117">Тип</span><span class="sxs-lookup"><span data-stu-id="d30ba-117">Type</span></span>   |<span data-ttu-id="d30ba-118">Описание</span><span class="sxs-lookup"><span data-stu-id="d30ba-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d30ba-119">id</span><span class="sxs-lookup"><span data-stu-id="d30ba-119">id</span></span>|<span data-ttu-id="d30ba-120">String</span><span class="sxs-lookup"><span data-stu-id="d30ba-120">String</span></span>| <span data-ttu-id="d30ba-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d30ba-121">Read-only.</span></span> <span data-ttu-id="d30ba-122">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="d30ba-122">Unique ID of the message.</span></span>|
|<span data-ttu-id="d30ba-123">displayName</span><span class="sxs-lookup"><span data-stu-id="d30ba-123">displayName</span></span>| <span data-ttu-id="d30ba-124">string</span><span class="sxs-lookup"><span data-stu-id="d30ba-124">string</span></span> | <span data-ttu-id="d30ba-125">Отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="d30ba-125">The display name of the user.</span></span> |
|<span data-ttu-id="d30ba-126">roles</span><span class="sxs-lookup"><span data-stu-id="d30ba-126">roles</span></span>| <span data-ttu-id="d30ba-127">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d30ba-127">string collection</span></span> | <span data-ttu-id="d30ba-128">Роли этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="d30ba-128">The roles for that user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d30ba-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d30ba-129">JSON representation</span></span>

<span data-ttu-id="d30ba-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d30ba-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.conversationMember"
}-->

```json
{
  "id": "string (identifier)",
  "displayName" : "string",
  "roles" : ["string"]
}

```

## <a name="see-also"></a><span data-ttu-id="d30ba-131">См. также</span><span class="sxs-lookup"><span data-stu-id="d30ba-131">See Also</span></span>

[<span data-ttu-id="d30ba-132">aadUserConversationMember</span><span class="sxs-lookup"><span data-stu-id="d30ba-132">aadUserConversationMember</span></span>](aaduserconversationmember.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "conversationMember",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
