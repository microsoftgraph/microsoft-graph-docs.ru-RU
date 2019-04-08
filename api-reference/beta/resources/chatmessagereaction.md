---
title: Тип ресурса Чатмессажереактион
description: 'Представляет реакцию на объект chatMessage. '
localization_priority: Normal
ms.openlocfilehash: 5020653ef02c1604aece46f3ff2c7ea1c82a75ec
ms.sourcegitcommit: 953895b28b6bae6e17eead938565fde289c49ef7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/05/2019
ms.locfileid: "31481386"
---
# <a name="chatmessagereaction-resource-type"></a><span data-ttu-id="147f9-103">Тип ресурса Чатмессажереактион</span><span class="sxs-lookup"><span data-stu-id="147f9-103">chatMessageReaction resource type</span></span>

<span data-ttu-id="147f9-104">Представляет реакцию на объект [chatMessage](chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="147f9-104">Represents a reaction to a [chatMessage](chatmessage.md) entity.</span></span> 

<span data-ttu-id="147f9-105">Сущность типа `chatMessageReaction` возвращается в составе API [сообщений канала](../api/channel-get-message.md) в составе объекта [chatMessage](chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="147f9-105">An entity of type `chatMessageReaction` is returned as part of the [Get channel messages](../api/channel-get-message.md) API, as a part of [chatMessage](chatmessage.md) entity.</span></span>

## <a name="properties"></a><span data-ttu-id="147f9-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="147f9-106">Properties</span></span>
| <span data-ttu-id="147f9-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="147f9-107">Property</span></span>     | <span data-ttu-id="147f9-108">Тип</span><span class="sxs-lookup"><span data-stu-id="147f9-108">Type</span></span>   |<span data-ttu-id="147f9-109">Описание</span><span class="sxs-lookup"><span data-stu-id="147f9-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="147f9-110">Реактионтипе</span><span class="sxs-lookup"><span data-stu-id="147f9-110">reactionType</span></span>|<span data-ttu-id="147f9-111">string</span><span class="sxs-lookup"><span data-stu-id="147f9-111">string</span></span>| <span data-ttu-id="147f9-112">Тип реакции.</span><span class="sxs-lookup"><span data-stu-id="147f9-112">The type of reaction.</span></span> <span data-ttu-id="147f9-113">Планируемые значения включают:</span><span class="sxs-lookup"><span data-stu-id="147f9-113">Planned values include:</span></span> <br><ul><li><span data-ttu-id="147f9-114">В данном случае, как и сообщение, в этом случае используется пустое содержимое.</span><span class="sxs-lookup"><span data-stu-id="147f9-114">Like - Like a message, content is blank in this case.</span></span></li><li><span data-ttu-id="147f9-115">Эмодзи, реакция на эмодзи.</span><span class="sxs-lookup"><span data-stu-id="147f9-115">Emoji - Emoji reaction.</span></span> <span data-ttu-id="147f9-116">Для содержимого задано значение Юникод для эмодзи.</span><span class="sxs-lookup"><span data-stu-id="147f9-116">Content is set to unicode value of the emoji.</span></span></li><li><span data-ttu-id="147f9-117">Label — содержимое задается в виде строки в метке.</span><span class="sxs-lookup"><span data-stu-id="147f9-117">Label - Content is set to the string in the label.</span></span></li></ul>|
|<span data-ttu-id="147f9-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="147f9-118">createdDateTime</span></span>|<span data-ttu-id="147f9-119">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="147f9-119">dateTimeOffset</span></span>|<span data-ttu-id="147f9-120">Метка времени в формате UTC для корневого сообщения в формате ISO-8601.</span><span class="sxs-lookup"><span data-stu-id="147f9-120">UTC timestamp of the root message in ISO-8601 format.</span></span>|
|<span data-ttu-id="147f9-121">user</span><span class="sxs-lookup"><span data-stu-id="147f9-121">user</span></span>|<span data-ttu-id="147f9-122">identitySet</span><span class="sxs-lookup"><span data-stu-id="147f9-122">identitySet</span></span>|<span data-ttu-id="147f9-123">Пользователь, который реагировал на сообщение.</span><span class="sxs-lookup"><span data-stu-id="147f9-123">The user who reacted to the message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="147f9-124">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="147f9-124">JSON representation</span></span>

<span data-ttu-id="147f9-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="147f9-125">The following is a JSON representation of the resource.</span></span>

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
