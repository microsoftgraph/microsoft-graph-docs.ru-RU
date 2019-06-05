---
title: Тип ресурса Чатмессажереактион
description: 'Представляет реакцию на объект chatMessage. '
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 33fe5a881d05b2ac2bc86e97e11b00c3465a8c09
ms.sourcegitcommit: 624ac42e74533a9bf0d0d22b3b15adbb258fd594
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2019
ms.locfileid: "34709427"
---
# <a name="chatmessagereaction-resource-type"></a><span data-ttu-id="98c55-103">Тип ресурса Чатмессажереактион</span><span class="sxs-lookup"><span data-stu-id="98c55-103">chatMessageReaction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98c55-104">Представляет реакцию на объект [chatMessage](chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="98c55-104">Represents a reaction to a [chatMessage](chatmessage.md) entity.</span></span> 

<span data-ttu-id="98c55-105">Сущность типа `chatMessageReaction` возвращается в составе интерфейса [сообщения канала Get](../api/channel-get-message.md) в виде части объекта [chatMessage](chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="98c55-105">An entity of type `chatMessageReaction` is returned as part of the [Get channel message](../api/channel-get-message.md) API, as a part of the [chatMessage](chatmessage.md) entity.</span></span>

## <a name="properties"></a><span data-ttu-id="98c55-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="98c55-106">Properties</span></span>

| <span data-ttu-id="98c55-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="98c55-107">Property</span></span>     | <span data-ttu-id="98c55-108">Тип</span><span class="sxs-lookup"><span data-stu-id="98c55-108">Type</span></span>        | <span data-ttu-id="98c55-109">Описание</span><span class="sxs-lookup"><span data-stu-id="98c55-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="98c55-110">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="98c55-110">createdDateTime</span></span>|<span data-ttu-id="98c55-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="98c55-111">DateTimeOffset</span></span>|<span data-ttu-id="98c55-p101">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="98c55-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="98c55-114">Реактионтипе</span><span class="sxs-lookup"><span data-stu-id="98c55-114">reactionType</span></span>|<span data-ttu-id="98c55-115">String</span><span class="sxs-lookup"><span data-stu-id="98c55-115">String</span></span>|<span data-ttu-id="98c55-116">Планируемые значения включают:</span><span class="sxs-lookup"><span data-stu-id="98c55-116">Planned values include:</span></span> <br><ul><li><span data-ttu-id="98c55-117">В данном случае, как и сообщение, в этом случае используется пустое содержимое.</span><span class="sxs-lookup"><span data-stu-id="98c55-117">Like - Like a message, content is blank in this case.</span></span></li><li><span data-ttu-id="98c55-118">Эмодзи, реакция на эмодзи.</span><span class="sxs-lookup"><span data-stu-id="98c55-118">Emoji - Emoji reaction.</span></span> <span data-ttu-id="98c55-119">Для содержимого задано значение Юникод для эмодзи.</span><span class="sxs-lookup"><span data-stu-id="98c55-119">Content is set to unicode value of the emoji.</span></span></li><li><span data-ttu-id="98c55-120">Label — содержимое задается в виде строки в метке.</span><span class="sxs-lookup"><span data-stu-id="98c55-120">Label - Content is set to the string in the label.</span></span></li></ul>|
|<span data-ttu-id="98c55-121">user</span><span class="sxs-lookup"><span data-stu-id="98c55-121">user</span></span>|[<span data-ttu-id="98c55-122">identitySet</span><span class="sxs-lookup"><span data-stu-id="98c55-122">identitySet</span></span>](identityset.md)|<span data-ttu-id="98c55-123">Пользователь, который реагировал на сообщение.</span><span class="sxs-lookup"><span data-stu-id="98c55-123">The user who reacted to the message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="98c55-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="98c55-124">JSON representation</span></span>

<span data-ttu-id="98c55-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="98c55-125">The following is a JSON representation of the resource.</span></span>

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
