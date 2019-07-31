---
title: Тип ресурса Чатмессажереактион
description: 'Представляет реакцию на объект chatMessage. '
localization_priority: Normal
doc_type: resourcePageType
author: RamjotSingh
ms.prod: microsoft-teams
ms.openlocfilehash: e1193e65697187f705f2758c2c195e5519326dc0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973991"
---
# <a name="chatmessagereaction-resource-type"></a><span data-ttu-id="70d81-103">Тип ресурса Чатмессажереактион</span><span class="sxs-lookup"><span data-stu-id="70d81-103">chatMessageReaction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70d81-104">Представляет реакцию на объект [chatMessage](chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="70d81-104">Represents a reaction to a [chatMessage](chatmessage.md) entity.</span></span> 

<span data-ttu-id="70d81-105">Сущность типа `chatMessageReaction` возвращается в составе интерфейса [сообщения канала Get](../api/channel-get-message.md) в виде части объекта [chatMessage](chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="70d81-105">An entity of type `chatMessageReaction` is returned as part of the [Get channel message](../api/channel-get-message.md) API, as a part of the [chatMessage](chatmessage.md) entity.</span></span>

## <a name="properties"></a><span data-ttu-id="70d81-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="70d81-106">Properties</span></span>

| <span data-ttu-id="70d81-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="70d81-107">Property</span></span>     | <span data-ttu-id="70d81-108">Тип</span><span class="sxs-lookup"><span data-stu-id="70d81-108">Type</span></span>        | <span data-ttu-id="70d81-109">Описание</span><span class="sxs-lookup"><span data-stu-id="70d81-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="70d81-110">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="70d81-110">createdDateTime</span></span>|<span data-ttu-id="70d81-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70d81-111">DateTimeOffset</span></span>|<span data-ttu-id="70d81-p101">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="70d81-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="70d81-114">Реактионтипе</span><span class="sxs-lookup"><span data-stu-id="70d81-114">reactionType</span></span>|<span data-ttu-id="70d81-115">String</span><span class="sxs-lookup"><span data-stu-id="70d81-115">String</span></span>|<span data-ttu-id="70d81-116">Поддерживаемые значения: `like`, `angry`, `sad`, `laugh`, `heart`, `surprised`.</span><span class="sxs-lookup"><span data-stu-id="70d81-116">Supported values are `like`, `angry`, `sad`, `laugh`, `heart`, `surprised`.</span></span> |
|<span data-ttu-id="70d81-117">user</span><span class="sxs-lookup"><span data-stu-id="70d81-117">user</span></span>|[<span data-ttu-id="70d81-118">identitySet</span><span class="sxs-lookup"><span data-stu-id="70d81-118">identitySet</span></span>](identityset.md)|<span data-ttu-id="70d81-119">Пользователь, который реагировал на сообщение.</span><span class="sxs-lookup"><span data-stu-id="70d81-119">The user who reacted to the message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="70d81-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="70d81-120">JSON representation</span></span>

<span data-ttu-id="70d81-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="70d81-121">The following is a JSON representation of the resource.</span></span>

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
