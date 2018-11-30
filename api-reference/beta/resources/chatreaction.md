---
title: Тип ресурса chatMessageReaction
description: 'Представляет реакцию на chatMessage сущности. '
ms.openlocfilehash: 1ad1f7948405a8891ec9aa13065b71108e9c47c5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082519"
---
# <a name="chatmessagereaction-resource-type"></a><span data-ttu-id="e4f48-103">Тип ресурса chatMessageReaction</span><span class="sxs-lookup"><span data-stu-id="e4f48-103">chatMessageReaction resource type</span></span>

<span data-ttu-id="e4f48-104">Представляет реакцию на [chatMessage](chatmessage.md) сущности.</span><span class="sxs-lookup"><span data-stu-id="e4f48-104">Represents a reaction to a [chatMessage](chatmessage.md) entity.</span></span> 

<span data-ttu-id="e4f48-105">Сущность типа `chatMessageReaction` возвращается как часть [получить сообщения](../api/channel-get-message.md) API, как часть [chatMessage](chatmessage.md) сущности.</span><span class="sxs-lookup"><span data-stu-id="e4f48-105">An entity of type `chatMessageReaction` is returned as part of the [Get channel messages](../api/channel-get-message.md) API, as a part of [chatMessage](chatmessage.md) entity.</span></span>

## <a name="properties"></a><span data-ttu-id="e4f48-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e4f48-106">Properties</span></span>
| <span data-ttu-id="e4f48-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e4f48-107">Property</span></span>     | <span data-ttu-id="e4f48-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e4f48-108">Type</span></span>   |<span data-ttu-id="e4f48-109">Description</span><span class="sxs-lookup"><span data-stu-id="e4f48-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e4f48-110">reactionType</span><span class="sxs-lookup"><span data-stu-id="e4f48-110">reactionType</span></span>|<span data-ttu-id="e4f48-111">string</span><span class="sxs-lookup"><span data-stu-id="e4f48-111">string</span></span>| <span data-ttu-id="e4f48-112">Тип реакции.</span><span class="sxs-lookup"><span data-stu-id="e4f48-112">The type of reaction.</span></span> <span data-ttu-id="e4f48-113">Запланированные значения:</span><span class="sxs-lookup"><span data-stu-id="e4f48-113">Planned values include:</span></span> <br><ul><li><span data-ttu-id="e4f48-114">Как - как сообщение, контент не задан в этом случае.</span><span class="sxs-lookup"><span data-stu-id="e4f48-114">Like - Like a message, content is blank in this case.</span></span></li><li><span data-ttu-id="e4f48-115">Emoji - Emoji реакции.</span><span class="sxs-lookup"><span data-stu-id="e4f48-115">Emoji - Emoji reaction.</span></span> <span data-ttu-id="e4f48-116">Содержимое задано значение Юникод из emoji.</span><span class="sxs-lookup"><span data-stu-id="e4f48-116">Content is set to unicode value of the emoji.</span></span></li><li><span data-ttu-id="e4f48-117">Подпись — содержимое задано значение строки в метку.</span><span class="sxs-lookup"><span data-stu-id="e4f48-117">Label - Content is set to the string in the label.</span></span></li></ul>|
|<span data-ttu-id="e4f48-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e4f48-118">createdDateTime</span></span>|<span data-ttu-id="e4f48-119">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4f48-119">dateTimeOffset</span></span>|<span data-ttu-id="e4f48-120">Метка времени UTC корневой сообщения в формате ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="e4f48-120">UTC timestamp of the root message in ISO-8601 format.</span></span>|
|<span data-ttu-id="e4f48-121">user</span><span class="sxs-lookup"><span data-stu-id="e4f48-121">user</span></span>|<span data-ttu-id="e4f48-122">identitySet</span><span class="sxs-lookup"><span data-stu-id="e4f48-122">identitySet</span></span>|<span data-ttu-id="e4f48-123">Пользователь, отреагировало на сообщение.</span><span class="sxs-lookup"><span data-stu-id="e4f48-123">The user who reacted to the message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e4f48-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e4f48-124">JSON representation</span></span>

<span data-ttu-id="e4f48-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e4f48-125">The following is a JSON representation of the resource.</span></span>

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
