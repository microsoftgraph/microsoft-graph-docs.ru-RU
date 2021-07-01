---
title: тип ресурса chatMessageReaction
description: 'Представляет реакцию на объект chatMessage. '
localization_priority: Normal
doc_type: resourcePageType
author: RamjotSingh
ms.prod: microsoft-teams
ms.openlocfilehash: fd94315fef0d11eb5dc54fb592dc7de01f912757
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208927"
---
# <a name="chatmessagereaction-resource-type"></a><span data-ttu-id="031f2-103">тип ресурса chatMessageReaction</span><span class="sxs-lookup"><span data-stu-id="031f2-103">chatMessageReaction resource type</span></span>

<span data-ttu-id="031f2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="031f2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="031f2-105">Представляет реакцию на [объект chatMessage.](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="031f2-105">Represents a reaction to a [chatMessage](chatmessage.md) entity.</span></span> 

<span data-ttu-id="031f2-106">Объект типа возвращается в рамках API сообщения get channel, как часть `chatMessageReaction` [сущности chatMessage.](chatmessage.md) [](../api/chatmessage-get.md)</span><span class="sxs-lookup"><span data-stu-id="031f2-106">An entity of type `chatMessageReaction` is returned as part of the [Get channel message](../api/chatmessage-get.md) API, as a part of the [chatMessage](chatmessage.md) entity.</span></span>

## <a name="properties"></a><span data-ttu-id="031f2-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="031f2-107">Properties</span></span>

| <span data-ttu-id="031f2-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="031f2-108">Property</span></span>     | <span data-ttu-id="031f2-109">Тип</span><span class="sxs-lookup"><span data-stu-id="031f2-109">Type</span></span>        | <span data-ttu-id="031f2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="031f2-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="031f2-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="031f2-111">createdDateTime</span></span>|<span data-ttu-id="031f2-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="031f2-112">DateTimeOffset</span></span>|<span data-ttu-id="031f2-113">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="031f2-113">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="031f2-114">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="031f2-114">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="031f2-115">reactionType</span><span class="sxs-lookup"><span data-stu-id="031f2-115">reactionType</span></span>|<span data-ttu-id="031f2-116">String</span><span class="sxs-lookup"><span data-stu-id="031f2-116">String</span></span>|<span data-ttu-id="031f2-117">Поддерживаемые значения `like` : , , , , `angry` `sad` `laugh` `heart` `surprised` .</span><span class="sxs-lookup"><span data-stu-id="031f2-117">Supported values are `like`, `angry`, `sad`, `laugh`, `heart`, `surprised`.</span></span> |
|<span data-ttu-id="031f2-118">user</span><span class="sxs-lookup"><span data-stu-id="031f2-118">user</span></span>|[<span data-ttu-id="031f2-119">chatMessageReactionIdentitySet</span><span class="sxs-lookup"><span data-stu-id="031f2-119">chatMessageReactionIdentitySet</span></span>](chatmessagereactionidentityset.md)|<span data-ttu-id="031f2-120">Пользователь, реагирувший на сообщение.</span><span class="sxs-lookup"><span data-stu-id="031f2-120">The user who reacted to the message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="031f2-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="031f2-121">JSON representation</span></span>

<span data-ttu-id="031f2-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="031f2-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chatMessageReaction",
  "baseType": null
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "reactionType": "String",
  "user": {"@odata.type": "microsoft.graph.chatMessageReactionIdentitySet"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chatMessageReaction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


