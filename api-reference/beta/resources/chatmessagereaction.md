---
title: Тип ресурса Чатмессажереактион
description: 'Представляет реакцию на объект chatMessage. '
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: dd1eac9a4630e097f06cf99f30d371de9e32eb5f
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991494"
---
# <a name="chatmessagereaction-resource-type"></a><span data-ttu-id="0cacd-103">Тип ресурса Чатмессажереактион</span><span class="sxs-lookup"><span data-stu-id="0cacd-103">chatMessageReaction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0cacd-104">Представляет реакцию на объект [chatMessage](chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="0cacd-104">Represents a reaction to a [chatMessage](chatmessage.md) entity.</span></span> 

<span data-ttu-id="0cacd-105">Сущность типа `chatMessageReaction` возвращается в составе интерфейса [сообщения канала Get](../api/channel-get-message.md) в виде части объекта [chatMessage](chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="0cacd-105">An entity of type `chatMessageReaction` is returned as part of the [Get channel message](../api/channel-get-message.md) API, as a part of the [chatMessage](chatmessage.md) entity.</span></span>

## <a name="properties"></a><span data-ttu-id="0cacd-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="0cacd-106">Properties</span></span>

| <span data-ttu-id="0cacd-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="0cacd-107">Property</span></span>     | <span data-ttu-id="0cacd-108">Тип</span><span class="sxs-lookup"><span data-stu-id="0cacd-108">Type</span></span>        | <span data-ttu-id="0cacd-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0cacd-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0cacd-110">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0cacd-110">createdDateTime</span></span>|<span data-ttu-id="0cacd-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0cacd-111">DateTimeOffset</span></span>|<span data-ttu-id="0cacd-p101">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="0cacd-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="0cacd-114">Реактионтипе</span><span class="sxs-lookup"><span data-stu-id="0cacd-114">reactionType</span></span>|<span data-ttu-id="0cacd-115">String</span><span class="sxs-lookup"><span data-stu-id="0cacd-115">String</span></span>|<span data-ttu-id="0cacd-116">Поддерживаемые значения: `like`, `angry`, `sad`, `laugh`, `heart`, `surprised`.</span><span class="sxs-lookup"><span data-stu-id="0cacd-116">Supported values are `like`, `angry`, `sad`, `laugh`, `heart`, `surprised`.</span></span> |
|<span data-ttu-id="0cacd-117">user</span><span class="sxs-lookup"><span data-stu-id="0cacd-117">user</span></span>|[<span data-ttu-id="0cacd-118">identitySet</span><span class="sxs-lookup"><span data-stu-id="0cacd-118">identitySet</span></span>](identityset.md)|<span data-ttu-id="0cacd-119">Пользователь, который реагировал на сообщение.</span><span class="sxs-lookup"><span data-stu-id="0cacd-119">The user who reacted to the message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0cacd-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0cacd-120">JSON representation</span></span>

<span data-ttu-id="0cacd-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0cacd-121">The following is a JSON representation of the resource.</span></span>

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
