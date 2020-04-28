---
title: Тип ресурса Чатмессажереактион
description: 'Представляет реакцию на объект chatMessage. '
localization_priority: Normal
doc_type: resourcePageType
author: RamjotSingh
ms.prod: microsoft-teams
ms.openlocfilehash: cb26a46a3669b721184399036fa80e4a6b291ec8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507693"
---
# <a name="chatmessagereaction-resource-type"></a><span data-ttu-id="444e4-103">Тип ресурса Чатмессажереактион</span><span class="sxs-lookup"><span data-stu-id="444e4-103">chatMessageReaction resource type</span></span>

<span data-ttu-id="444e4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="444e4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="444e4-105">Представляет реакцию на объект [chatMessage](chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="444e4-105">Represents a reaction to a [chatMessage](chatmessage.md) entity.</span></span> 

<span data-ttu-id="444e4-106">Сущность типа `chatMessageReaction` возвращается в составе интерфейса [сообщения канала Get](../api/channel-get-message.md) в виде части объекта [chatMessage](chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="444e4-106">An entity of type `chatMessageReaction` is returned as part of the [Get channel message](../api/channel-get-message.md) API, as a part of the [chatMessage](chatmessage.md) entity.</span></span>

## <a name="properties"></a><span data-ttu-id="444e4-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="444e4-107">Properties</span></span>

| <span data-ttu-id="444e4-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="444e4-108">Property</span></span>     | <span data-ttu-id="444e4-109">Тип</span><span class="sxs-lookup"><span data-stu-id="444e4-109">Type</span></span>        | <span data-ttu-id="444e4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="444e4-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="444e4-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="444e4-111">createdDateTime</span></span>|<span data-ttu-id="444e4-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="444e4-112">DateTimeOffset</span></span>|<span data-ttu-id="444e4-p101">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="444e4-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="444e4-115">реактионтипе</span><span class="sxs-lookup"><span data-stu-id="444e4-115">reactionType</span></span>|<span data-ttu-id="444e4-116">String</span><span class="sxs-lookup"><span data-stu-id="444e4-116">String</span></span>|<span data-ttu-id="444e4-117">Поддерживаемые значения: `like`, `angry`, `sad`, `laugh`, `heart`, `surprised`.</span><span class="sxs-lookup"><span data-stu-id="444e4-117">Supported values are `like`, `angry`, `sad`, `laugh`, `heart`, `surprised`.</span></span> |
|<span data-ttu-id="444e4-118">user</span><span class="sxs-lookup"><span data-stu-id="444e4-118">user</span></span>|[<span data-ttu-id="444e4-119">identitySet</span><span class="sxs-lookup"><span data-stu-id="444e4-119">identitySet</span></span>](identityset.md)|<span data-ttu-id="444e4-120">Пользователь, который реагировал на сообщение.</span><span class="sxs-lookup"><span data-stu-id="444e4-120">The user who reacted to the message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="444e4-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="444e4-121">JSON representation</span></span>

<span data-ttu-id="444e4-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="444e4-122">The following is a JSON representation of the resource.</span></span>

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
  "user": {"@odata.type": "microsoft.graph.identitySet"}
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
