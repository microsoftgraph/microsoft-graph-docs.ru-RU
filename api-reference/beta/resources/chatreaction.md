---
title: Тип ресурса chatMessageReaction
description: 'Представляет реакцию на chatMessage сущности. '
localization_priority: Normal
ms.openlocfilehash: 5020653ef02c1604aece46f3ff2c7ea1c82a75ec
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810068"
---
# <a name="chatmessagereaction-resource-type"></a><span data-ttu-id="e7c76-103">Тип ресурса chatMessageReaction</span><span class="sxs-lookup"><span data-stu-id="e7c76-103">chatMessageReaction resource type</span></span>

<span data-ttu-id="e7c76-104">Представляет реакцию на [chatMessage](chatmessage.md) сущности.</span><span class="sxs-lookup"><span data-stu-id="e7c76-104">Represents a reaction to a [chatMessage](chatmessage.md) entity.</span></span> 

<span data-ttu-id="e7c76-105">Сущность типа `chatMessageReaction` возвращается как часть [получить сообщения](../api/channel-get-message.md) API, как часть [chatMessage](chatmessage.md) сущности.</span><span class="sxs-lookup"><span data-stu-id="e7c76-105">An entity of type `chatMessageReaction` is returned as part of the [Get channel messages](../api/channel-get-message.md) API, as a part of [chatMessage](chatmessage.md) entity.</span></span>

## <a name="properties"></a><span data-ttu-id="e7c76-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e7c76-106">Properties</span></span>
| <span data-ttu-id="e7c76-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e7c76-107">Property</span></span>     | <span data-ttu-id="e7c76-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e7c76-108">Type</span></span>   |<span data-ttu-id="e7c76-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e7c76-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e7c76-110">reactionType</span><span class="sxs-lookup"><span data-stu-id="e7c76-110">reactionType</span></span>|<span data-ttu-id="e7c76-111">string</span><span class="sxs-lookup"><span data-stu-id="e7c76-111">string</span></span>| <span data-ttu-id="e7c76-112">Тип реакции.</span><span class="sxs-lookup"><span data-stu-id="e7c76-112">The type of reaction.</span></span> <span data-ttu-id="e7c76-113">Запланированные значения:</span><span class="sxs-lookup"><span data-stu-id="e7c76-113">Planned values include:</span></span> <br><ul><li><span data-ttu-id="e7c76-114">Как - как сообщение, контент не задан в этом случае.</span><span class="sxs-lookup"><span data-stu-id="e7c76-114">Like - Like a message, content is blank in this case.</span></span></li><li><span data-ttu-id="e7c76-115">Emoji - Emoji реакции.</span><span class="sxs-lookup"><span data-stu-id="e7c76-115">Emoji - Emoji reaction.</span></span> <span data-ttu-id="e7c76-116">Содержимое задано значение Юникод из emoji.</span><span class="sxs-lookup"><span data-stu-id="e7c76-116">Content is set to unicode value of the emoji.</span></span></li><li><span data-ttu-id="e7c76-117">Подпись — содержимое задано значение строки в метку.</span><span class="sxs-lookup"><span data-stu-id="e7c76-117">Label - Content is set to the string in the label.</span></span></li></ul>|
|<span data-ttu-id="e7c76-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e7c76-118">createdDateTime</span></span>|<span data-ttu-id="e7c76-119">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7c76-119">dateTimeOffset</span></span>|<span data-ttu-id="e7c76-120">Метка времени UTC корневой сообщения в формате ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="e7c76-120">UTC timestamp of the root message in ISO-8601 format.</span></span>|
|<span data-ttu-id="e7c76-121">user</span><span class="sxs-lookup"><span data-stu-id="e7c76-121">user</span></span>|<span data-ttu-id="e7c76-122">identitySet</span><span class="sxs-lookup"><span data-stu-id="e7c76-122">identitySet</span></span>|<span data-ttu-id="e7c76-123">Пользователь, отреагировало на сообщение.</span><span class="sxs-lookup"><span data-stu-id="e7c76-123">The user who reacted to the message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e7c76-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e7c76-124">JSON representation</span></span>

<span data-ttu-id="e7c76-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e7c76-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "content"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessageReaction"
}-->

```json
{
  "reactionType": "string ",
  "createdDateTime": "string (timestamp)",
  "user": {"@odata.type": "microsoft.graph.identitySet"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chat message reaction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
