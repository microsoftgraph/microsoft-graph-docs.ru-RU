---
title: Тип ресурса Чатмессажементион
description: 'Представляет упоминание в объекте chatMessage. Упоминание может быть у пользователя, группы, ленты или канала. '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 1aaf4b062bc46241ced0c862972cbfebffb2fbf4
ms.sourcegitcommit: 62c900af626e46439d949462f09061cc5c41d6ff
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/16/2020
ms.locfileid: "44272787"
---
# <a name="chatmessagemention-resource-type"></a><span data-ttu-id="5f1f0-104">Тип ресурса Чатмессажементион</span><span class="sxs-lookup"><span data-stu-id="5f1f0-104">chatMessageMention resource type</span></span>

<span data-ttu-id="5f1f0-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f1f0-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5f1f0-106">Представляет упоминание в объекте [chatMessage](./chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="5f1f0-106">Represents a mention in a [chatMessage](./chatmessage.md) entity.</span></span> <span data-ttu-id="5f1f0-107">Упоминание может быть у [пользователя](user.md), [группы](team.md), ленты или [канала](channel.md).</span><span class="sxs-lookup"><span data-stu-id="5f1f0-107">The mention can be to a [user](user.md), [team](team.md), bot, or [channel](channel.md).</span></span> 

<span data-ttu-id="5f1f0-108">В объекте **chatMessage** , содержащем одно или несколько упоминаний, свойство **Content** текста сообщения представляет сообщение чата в HTML.</span><span class="sxs-lookup"><span data-stu-id="5f1f0-108">In a **chatMessage** object that contains one or more mentions, the message body **content** property represents the chat message in HTML.</span></span> <span data-ttu-id="5f1f0-109">Он заключает **ментионтекст** каждого упоминания в `at` элементе HTML с `id` атрибутом, соответствующим свойству **ID** упомянутого упоминания.</span><span class="sxs-lookup"><span data-stu-id="5f1f0-109">It encloses the **mentionText** of each mention in an HTML `at` element, with an `id` attribute that corresponds to the **id** property of the mention.</span></span>

<span data-ttu-id="5f1f0-110">Например, сообщение чата содержит два упомянутых элемента с текстом "Меган" и "Алекс" соответственно.</span><span class="sxs-lookup"><span data-stu-id="5f1f0-110">As an example, a chat message contains two mentions, with the mention text "Megan" and "Alex" respectively.</span></span> <span data-ttu-id="5f1f0-111">Его свойство Body свойства **Content** определяет `at` элементы для двух упомянутых ниже элементов.</span><span class="sxs-lookup"><span data-stu-id="5f1f0-111">Its body **content** property specifies `at` elements for the two mentions as follows:</span></span>

``` json
"body": {
    "contentType": "html",
    "content": "<div><div>Ah, <at id=\"0\">Megan</at>, <at id=\"1\">Alex</at>, I saw them in a separate folder. Thanks!</div>\n</div>"
}
```

<span data-ttu-id="5f1f0-112">В свойстве **Content** первое упоминание имеет `id` атрибут HTML 0.</span><span class="sxs-lookup"><span data-stu-id="5f1f0-112">In the **content** property, the first mention has an HTML `id` attribute of 0.</span></span> <span data-ttu-id="5f1f0-113">Это соответствует свойству **ID** этого первого экземпляра **чатмессажементион**, которое также равно 0.</span><span class="sxs-lookup"><span data-stu-id="5f1f0-113">This corresponds to the **id** property of that first instance of **chatMessageMention**, which is also 0.</span></span>

<span data-ttu-id="5f1f0-114">Второе упоминание имеет `id` атрибут 1, совпадающий со свойством **ID** второго экземпляра, который равен 1.</span><span class="sxs-lookup"><span data-stu-id="5f1f0-114">The second mention has an `id` attribute of 1, matching the **id** property of the second instance, which is 1.</span></span>

<span data-ttu-id="5f1f0-115">Полный контекст этого примера приведен в разделе [список ответов на сообщения канала](/graph/api/channel-list-messagereplies?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="5f1f0-115">For a fuller context of the example, see [List channel message replies](/graph/api/channel-list-messagereplies?view=graph-rest-beta).</span></span>

## <a name="properties"></a><span data-ttu-id="5f1f0-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="5f1f0-116">Properties</span></span>

| <span data-ttu-id="5f1f0-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="5f1f0-117">Property</span></span>| <span data-ttu-id="5f1f0-118">Тип</span><span class="sxs-lookup"><span data-stu-id="5f1f0-118">Type</span></span>|<span data-ttu-id="5f1f0-119">Описание</span><span class="sxs-lookup"><span data-stu-id="5f1f0-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5f1f0-120">id</span><span class="sxs-lookup"><span data-stu-id="5f1f0-120">id</span></span>|<span data-ttu-id="5f1f0-121">Int32</span><span class="sxs-lookup"><span data-stu-id="5f1f0-121">Int32</span></span>|<span data-ttu-id="5f1f0-122">Индекс объекта, упоминаемого в заданном **chatMessage**.</span><span class="sxs-lookup"><span data-stu-id="5f1f0-122">Index of an entity being mentioned in the specified **chatMessage**.</span></span> <span data-ttu-id="5f1f0-123">Соответствует значению {index} в соответствующем `<at id="{index}">` теге в тексте сообщения.</span><span class="sxs-lookup"><span data-stu-id="5f1f0-123">Matches the {index} value in the corresponding `<at id="{index}">` tag in the message body.</span></span>|
|<span data-ttu-id="5f1f0-124">ментионтекст</span><span class="sxs-lookup"><span data-stu-id="5f1f0-124">mentionText</span></span>|<span data-ttu-id="5f1f0-125">string</span><span class="sxs-lookup"><span data-stu-id="5f1f0-125">string</span></span>|<span data-ttu-id="5f1f0-126">Строка, используемая для представления упоминания.</span><span class="sxs-lookup"><span data-stu-id="5f1f0-126">String used to represent the mention.</span></span> <span data-ttu-id="5f1f0-127">Например, отображаемое имя пользователя, имя группы.</span><span class="sxs-lookup"><span data-stu-id="5f1f0-127">For example, a user's display name, a team name.</span></span>|
|<span data-ttu-id="5f1f0-128">котором</span><span class="sxs-lookup"><span data-stu-id="5f1f0-128">mentioned</span></span>|[<span data-ttu-id="5f1f0-129">identitySet</span><span class="sxs-lookup"><span data-stu-id="5f1f0-129">identitySet</span></span>](identityset.md)|<span data-ttu-id="5f1f0-130">Упоминаемая сущность (пользователь, приложение, группа или канал).</span><span class="sxs-lookup"><span data-stu-id="5f1f0-130">The entity (user, application, team, or channel) that was mentioned.</span></span>  <span data-ttu-id="5f1f0-131">Если это канал или группа, @mentioned, Identity содержит свойство **CONVERSATION** , предоставляющее идентификатор команды или канала, и свойство **конверсатионидентититипе** , которое представляет группу или канал.</span><span class="sxs-lookup"><span data-stu-id="5f1f0-131">If it was a channel or team that was @mentioned, the identitySet contains a **conversation** property giving the ID of the team/channel, and a **conversationIdentityType** property that represents either the team or channel.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="5f1f0-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5f1f0-132">JSON representation</span></span>

<span data-ttu-id="5f1f0-133">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5f1f0-133">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessageMention"
}-->

```json
{
  "id": 1024,
  "mentionText": "string",
  "mentioned": {"@odata.type": "microsoft.graph.identitySet"}
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
