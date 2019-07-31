---
title: Тип ресурса aadUserConversationMember
description: Представляет пользователя в беседе.
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c4e937d88a1e504c6774b2dcb657dee443d54843
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013635"
---
# <a name="aaduserconversationmember-resource-type"></a><span data-ttu-id="2a9a7-103">Тип ресурса aadUserConversationMember</span><span class="sxs-lookup"><span data-stu-id="2a9a7-103">aadUserConversationMember resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a9a7-104">Представляет пользователя Azure Active Directory в [чате](chat.md).</span><span class="sxs-lookup"><span data-stu-id="2a9a7-104">Represents an Azure Active Directory user in a [chat](chat.md).</span></span> <span data-ttu-id="2a9a7-105">Этот тип наследуется от [conversationMember](conversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="2a9a7-105">This type inherits from [conversationMember](conversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="2a9a7-106">Методы</span><span class="sxs-lookup"><span data-stu-id="2a9a7-106">Methods</span></span>

| <span data-ttu-id="2a9a7-107">Метод</span><span class="sxs-lookup"><span data-stu-id="2a9a7-107">Method</span></span>       | <span data-ttu-id="2a9a7-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2a9a7-108">Return Type</span></span>  |<span data-ttu-id="2a9a7-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2a9a7-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2a9a7-110">Список участников чата</span><span class="sxs-lookup"><span data-stu-id="2a9a7-110">List Chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="2a9a7-111">Коллекция [conversationmember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="2a9a7-111">[conversationmember](conversationmember.md) collection</span></span> | <span data-ttu-id="2a9a7-112">Получение списка всех пользователей в чате.</span><span class="sxs-lookup"><span data-stu-id="2a9a7-112">Get the list of all users in the chat.</span></span>|
|[<span data-ttu-id="2a9a7-113">Получение участника чата</span><span class="sxs-lookup"><span data-stu-id="2a9a7-113">Get Chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="2a9a7-114">conversationmember</span><span class="sxs-lookup"><span data-stu-id="2a9a7-114">conversationmember</span></span>](conversationmember.md) | <span data-ttu-id="2a9a7-115">Получение одного пользователя в чате.</span><span class="sxs-lookup"><span data-stu-id="2a9a7-115">Get a single user in the chat.</span></span>|

## <a name="properties"></a><span data-ttu-id="2a9a7-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="2a9a7-116">Properties</span></span>
| <span data-ttu-id="2a9a7-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="2a9a7-117">Property</span></span>     | <span data-ttu-id="2a9a7-118">Тип</span><span class="sxs-lookup"><span data-stu-id="2a9a7-118">Type</span></span>   |<span data-ttu-id="2a9a7-119">Описание</span><span class="sxs-lookup"><span data-stu-id="2a9a7-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2a9a7-120">id</span><span class="sxs-lookup"><span data-stu-id="2a9a7-120">id</span></span>|<span data-ttu-id="2a9a7-121">String</span><span class="sxs-lookup"><span data-stu-id="2a9a7-121">String</span></span>| <span data-ttu-id="2a9a7-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2a9a7-122">Read-only.</span></span> <span data-ttu-id="2a9a7-123">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="2a9a7-123">Unique ID of the message.</span></span>|
|<span data-ttu-id="2a9a7-124">displayName</span><span class="sxs-lookup"><span data-stu-id="2a9a7-124">displayName</span></span>| <span data-ttu-id="2a9a7-125">string</span><span class="sxs-lookup"><span data-stu-id="2a9a7-125">string</span></span> | <span data-ttu-id="2a9a7-126">Отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="2a9a7-126">The display name of the user.</span></span> |
|<span data-ttu-id="2a9a7-127">roles</span><span class="sxs-lookup"><span data-stu-id="2a9a7-127">roles</span></span>| <span data-ttu-id="2a9a7-128">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="2a9a7-128">string collection</span></span> | <span data-ttu-id="2a9a7-129">Роли этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="2a9a7-129">The roles for that user.</span></span> |
|<span data-ttu-id="2a9a7-130">userId</span><span class="sxs-lookup"><span data-stu-id="2a9a7-130">userId</span></span>| <span data-ttu-id="2a9a7-131">строка</span><span class="sxs-lookup"><span data-stu-id="2a9a7-131">string</span></span> | <span data-ttu-id="2a9a7-132">GUID пользователя.</span><span class="sxs-lookup"><span data-stu-id="2a9a7-132">The guid of the user.</span></span> |
|<span data-ttu-id="2a9a7-133">email</span><span class="sxs-lookup"><span data-stu-id="2a9a7-133">email</span></span>| <span data-ttu-id="2a9a7-134">строка</span><span class="sxs-lookup"><span data-stu-id="2a9a7-134">string</span></span>  | <span data-ttu-id="2a9a7-135">Электронный адрес пользователя.</span><span class="sxs-lookup"><span data-stu-id="2a9a7-135">The e-mail address of the user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2a9a7-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2a9a7-136">JSON representation</span></span>

<span data-ttu-id="2a9a7-137">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2a9a7-137">The following is a JSON representation of the resource.</span></span>

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
