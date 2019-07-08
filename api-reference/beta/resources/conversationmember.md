---
title: Тип ресурса conversationMember
description: Представляет пользователя в беседе.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 10a40e53831cc44559a42d1684039c186554e433
ms.sourcegitcommit: 624ac42e74533a9bf0d0d22b3b15adbb258fd594
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2019
ms.locfileid: "34709350"
---
# <a name="conversationmember-resource-type"></a><span data-ttu-id="a2180-103">Тип ресурса conversationMember</span><span class="sxs-lookup"><span data-stu-id="a2180-103">conversationMember resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2180-104">Представляет пользователя в [чате](chat.md).</span><span class="sxs-lookup"><span data-stu-id="a2180-104">Represents a user in a [chat](chat.md).</span></span>

## <a name="methods"></a><span data-ttu-id="a2180-105">Методы</span><span class="sxs-lookup"><span data-stu-id="a2180-105">Methods</span></span>

| <span data-ttu-id="a2180-106">Метод</span><span class="sxs-lookup"><span data-stu-id="a2180-106">Method</span></span>       | <span data-ttu-id="a2180-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a2180-107">Return Type</span></span>  |<span data-ttu-id="a2180-108">Описание</span><span class="sxs-lookup"><span data-stu-id="a2180-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a2180-109">Список участников чата</span><span class="sxs-lookup"><span data-stu-id="a2180-109">List Chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="a2180-110">Коллекция [conversationmember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="a2180-110">[conversationmember](conversationmember.md) collection</span></span> | <span data-ttu-id="a2180-111">Получение списка всех пользователей в чате.</span><span class="sxs-lookup"><span data-stu-id="a2180-111">Get the list of all users in the chat.</span></span>|
|[<span data-ttu-id="a2180-112">Получение участника чата</span><span class="sxs-lookup"><span data-stu-id="a2180-112">Get Chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="a2180-113">conversationmember</span><span class="sxs-lookup"><span data-stu-id="a2180-113">conversationmember</span></span>](conversationmember.md) | <span data-ttu-id="a2180-114">Получение одного пользователя в чате.</span><span class="sxs-lookup"><span data-stu-id="a2180-114">Get a single user in the chat.</span></span>|

## <a name="properties"></a><span data-ttu-id="a2180-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="a2180-115">Properties</span></span>

| <span data-ttu-id="a2180-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="a2180-116">Property</span></span>     | <span data-ttu-id="a2180-117">Тип</span><span class="sxs-lookup"><span data-stu-id="a2180-117">Type</span></span>   |<span data-ttu-id="a2180-118">Описание</span><span class="sxs-lookup"><span data-stu-id="a2180-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a2180-119">id</span><span class="sxs-lookup"><span data-stu-id="a2180-119">id</span></span>|<span data-ttu-id="a2180-120">String</span><span class="sxs-lookup"><span data-stu-id="a2180-120">String</span></span>| <span data-ttu-id="a2180-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a2180-121">Read-only.</span></span> <span data-ttu-id="a2180-122">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="a2180-122">Unique ID of the message.</span></span>|
|<span data-ttu-id="a2180-123">displayName</span><span class="sxs-lookup"><span data-stu-id="a2180-123">displayName</span></span>| <span data-ttu-id="a2180-124">string</span><span class="sxs-lookup"><span data-stu-id="a2180-124">string</span></span> | <span data-ttu-id="a2180-125">Отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="a2180-125">The display name of the user.</span></span> |
|<span data-ttu-id="a2180-126">roles</span><span class="sxs-lookup"><span data-stu-id="a2180-126">roles</span></span>| <span data-ttu-id="a2180-127">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="a2180-127">string collection</span></span> | <span data-ttu-id="a2180-128">Роли этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="a2180-128">The roles for that user.</span></span> |

## <a name="relationships"></a><span data-ttu-id="a2180-129">Связи</span><span class="sxs-lookup"><span data-stu-id="a2180-129">Relationships</span></span>

<span data-ttu-id="a2180-130">Нет</span><span class="sxs-lookup"><span data-stu-id="a2180-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a2180-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a2180-131">JSON representation</span></span>

<span data-ttu-id="a2180-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a2180-132">The following is a JSON representation of the resource.</span></span>

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