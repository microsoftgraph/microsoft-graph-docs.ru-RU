---
title: тип ресурса chatMessageMention
description: 'Представляет упоминание в объекте chatMessage. Упоминание может быть для пользователя, команды, бота или канала. '
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: fefa80cf6fa66b61a3db8457f5b7f8809b07e2f3
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207009"
---
# <a name="chatmessagemention-resource-type"></a><span data-ttu-id="9d040-104">тип ресурса chatMessageMention</span><span class="sxs-lookup"><span data-stu-id="9d040-104">chatMessageMention resource type</span></span>

<span data-ttu-id="9d040-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d040-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d040-106">Представляет упоминание в [объекте chatMessage.](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="9d040-106">Represents a mention in a [chatMessage](chatmessage.md) entity.</span></span> <span data-ttu-id="9d040-107">Упоминание может быть для пользователя, [команды,](user.md)бота или [канала](channel.md). [](team.md)</span><span class="sxs-lookup"><span data-stu-id="9d040-107">The mention can be to a [user](user.md), [team](team.md), bot, or [channel](channel.md).</span></span> 

<span data-ttu-id="9d040-108">В **объекте chatMessage,** который содержит одно или  несколько упоминаний, свойство контента тела сообщения представляет сообщение чата в HTML.</span><span class="sxs-lookup"><span data-stu-id="9d040-108">In a **chatMessage** object that contains one or more mentions, the message body **content** property represents the chat message in HTML.</span></span> <span data-ttu-id="9d040-109">В него **заключено упоминание Каждого** упоминания в элементе HTML с атрибутом, соответствующим свойству `at` `id` **id** упоминания.</span><span class="sxs-lookup"><span data-stu-id="9d040-109">It encloses the **mentionText** of each mention in an HTML `at` element, with an `id` attribute that corresponds to the **id** property of the mention.</span></span>

<span data-ttu-id="9d040-110">В качестве примера, сообщение чата содержит два упоминания, с текстом упоминания "Меган" и "Алекс" соответственно.</span><span class="sxs-lookup"><span data-stu-id="9d040-110">As an example, a chat message contains two mentions, with the mention text "Megan" and "Alex" respectively.</span></span> <span data-ttu-id="9d040-111">Свойство **контента** тела указывает элементы для `at` этих двух упоминаний следующим образом:</span><span class="sxs-lookup"><span data-stu-id="9d040-111">Its body **content** property specifies `at` elements for the two mentions as follows:</span></span>

``` json
"body": {
    "contentType": "html",
    "content": "<div><div>Ah, <at id=\"0\">Megan</at>, <at id=\"1\">Alex</at>, I saw them in a separate folder. Thanks!</div>\n</div>"
}
```

<span data-ttu-id="9d040-112">В **свойстве контента** первое упоминание имеет htmL-атрибут `id` 0.</span><span class="sxs-lookup"><span data-stu-id="9d040-112">In the **content** property, the first mention has an HTML `id` attribute of 0.</span></span> <span data-ttu-id="9d040-113">Это соответствует свойству **id** этого первого экземпляра **chatMessageMention,** которое также является 0.</span><span class="sxs-lookup"><span data-stu-id="9d040-113">This corresponds to the **id** property of that first instance of **chatMessageMention**, which is also 0.</span></span>

<span data-ttu-id="9d040-114">Второе упоминание имеет атрибут 1, совпадающий с свойством `id` **id** второго экземпляра, которое является 1.</span><span class="sxs-lookup"><span data-stu-id="9d040-114">The second mention has an `id` attribute of 1, matching the **id** property of the second instance, which is 1.</span></span>

<span data-ttu-id="9d040-115">Более полный контекст примера см. в списке [ответов на сообщения канала.](../api/chatmessage-list-replies.md#example)</span><span class="sxs-lookup"><span data-stu-id="9d040-115">For a fuller context of the example, see [List channel message replies](../api/chatmessage-list-replies.md#example).</span></span>

## <a name="properties"></a><span data-ttu-id="9d040-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="9d040-116">Properties</span></span>
| <span data-ttu-id="9d040-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="9d040-117">Property</span></span>     | <span data-ttu-id="9d040-118">Тип</span><span class="sxs-lookup"><span data-stu-id="9d040-118">Type</span></span>   |<span data-ttu-id="9d040-119">Описание</span><span class="sxs-lookup"><span data-stu-id="9d040-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9d040-120">id</span><span class="sxs-lookup"><span data-stu-id="9d040-120">id</span></span>|<span data-ttu-id="9d040-121">Int32</span><span class="sxs-lookup"><span data-stu-id="9d040-121">Int32</span></span>|<span data-ttu-id="9d040-122">Индекс сущности, упоминаемой в указанном **chatMessage.**</span><span class="sxs-lookup"><span data-stu-id="9d040-122">Index of an entity being mentioned in the specified **chatMessage**.</span></span> <span data-ttu-id="9d040-123">Соответствует значению {index} в соответствующем `<at id="{index}">` теге в теле сообщения.</span><span class="sxs-lookup"><span data-stu-id="9d040-123">Matches the {index} value in the corresponding `<at id="{index}">` tag in the message body.</span></span>|
|<span data-ttu-id="9d040-124">mentionText</span><span class="sxs-lookup"><span data-stu-id="9d040-124">mentionText</span></span>|<span data-ttu-id="9d040-125">строка</span><span class="sxs-lookup"><span data-stu-id="9d040-125">string</span></span>|<span data-ttu-id="9d040-126">Строка, используемая для представления упоминания.</span><span class="sxs-lookup"><span data-stu-id="9d040-126">String used to represent the mention.</span></span> <span data-ttu-id="9d040-127">Например, имя отображения пользователя, имя команды.</span><span class="sxs-lookup"><span data-stu-id="9d040-127">For example, a user's display name, a team name.</span></span>|
|<span data-ttu-id="9d040-128">упомянутый</span><span class="sxs-lookup"><span data-stu-id="9d040-128">mentioned</span></span>|[<span data-ttu-id="9d040-129">chatMessageMentionedIdentitySet</span><span class="sxs-lookup"><span data-stu-id="9d040-129">chatMessageMentionedIdentitySet</span></span>](chatmessagementionedidentityset.md)|<span data-ttu-id="9d040-130">Объект (пользователь, приложение, команда или канал), который @mentioned.</span><span class="sxs-lookup"><span data-stu-id="9d040-130">The entity (user, application, team, or channel) that was @mentioned.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="9d040-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9d040-131">JSON representation</span></span>

<span data-ttu-id="9d040-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9d040-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.chatMessageMention"
}-->

```json
{
  "id": 1024,
  "mentionText": "string",
  "mentioned": {"@odata.type": "microsoft.graph.chatMessageMentionedIdentitySet"}
 }
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chat mention resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


