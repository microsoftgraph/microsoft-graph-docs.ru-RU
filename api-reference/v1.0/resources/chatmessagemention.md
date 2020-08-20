---
title: Тип ресурса chatMessageMention
description: 'Представляет упоминание в объекте chatMessage. Упоминание может быть: на пользователя, группу, бот или канал. '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3557ad926ebad764d9ad734c372fd4c367d319e6
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819877"
---
# <a name="chatmessagemention-resource-type"></a><span data-ttu-id="c0218-104">Тип ресурса chatMessageMention</span><span class="sxs-lookup"><span data-stu-id="c0218-104">chatMessageMention resource type</span></span>

<span data-ttu-id="c0218-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0218-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c0218-106">Представляет упоминание в [объекте chatMessage.](./chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="c0218-106">Represents a mention in a [chatMessage](./chatmessage.md) entity.</span></span> <span data-ttu-id="c0218-107">Упоминанием может быть [пользователь,](user.md) [команда,](team.md)бот или [канал.](channel.md)</span><span class="sxs-lookup"><span data-stu-id="c0218-107">The mention can be to a [user](user.md), [team](team.md), bot, or [channel](channel.md).</span></span> 

<span data-ttu-id="c0218-108">В **объекте chatMessage,** содержащем одно или несколько упоминаний, свойство содержимого **сообщения** представляет сообщение чата в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="c0218-108">In a **chatMessage** object that contains one or more mentions, the message body **content** property represents the chat message in HTML.</span></span> <span data-ttu-id="c0218-109">Он заключает **упоминание текста** каждого упоминания в `at` HTML-элементе с атрибутом, соответствующим `id` свойству **id** упоминания.</span><span class="sxs-lookup"><span data-stu-id="c0218-109">It encloses the **mentionText** of each mention in an HTML `at` element, with an `id` attribute that corresponds to the **id** property of the mention.</span></span>

<span data-ttu-id="c0218-110">Например, сообщение чата содержит два упоминания со словом "Меган" и "Арк", соответственно.</span><span class="sxs-lookup"><span data-stu-id="c0218-110">As an example, a chat message contains two mentions, with the mention text "Megan" and "Alex" respectively.</span></span> <span data-ttu-id="c0218-111">Свойство **содержимого в** теле определяет `at` элементы для двух упоминаний следующим образом:</span><span class="sxs-lookup"><span data-stu-id="c0218-111">Its body **content** property specifies `at` elements for the two mentions as follows:</span></span>

``` json
"body": {
    "contentType": "html",
    "content": "<div><div>Ah, <at id=\"0\">Megan</at>, <at id=\"1\">Alex</at>, I saw them in a separate folder. Thanks!</div>\n</div>"
}
```

<span data-ttu-id="c0218-112">В **свойстве содержимого** первый упоминание имеет АТРИБУТ HTML `id` 0.</span><span class="sxs-lookup"><span data-stu-id="c0218-112">In the **content** property, the first mention has an HTML `id` attribute of 0.</span></span> <span data-ttu-id="c0218-113">Соответствует свойству **id** первого экземпляра объекта **chatMessageMention,** которое также равно 0.</span><span class="sxs-lookup"><span data-stu-id="c0218-113">This corresponds to the **id** property of that first instance of **chatMessageMention**, which is also 0.</span></span>

<span data-ttu-id="c0218-114">Второе `id` упоминание имеет атрибут 1, соответствующий свойству **id** второго экземпляра, значение 1.</span><span class="sxs-lookup"><span data-stu-id="c0218-114">The second mention has an `id` attribute of 1, matching the **id** property of the second instance, which is 1.</span></span>

<span data-ttu-id="c0218-115">Более полный контекст примера см. в ответах [на сообщения в виде списка.](/graph/api/channel-list-messagereplies?view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="c0218-115">For a fuller context of the example, see [List channel message replies](/graph/api/channel-list-messagereplies?view=graph-rest-beta).</span></span>

## <a name="properties"></a><span data-ttu-id="c0218-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="c0218-116">Properties</span></span>

| <span data-ttu-id="c0218-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="c0218-117">Property</span></span>| <span data-ttu-id="c0218-118">Тип</span><span class="sxs-lookup"><span data-stu-id="c0218-118">Type</span></span>|<span data-ttu-id="c0218-119">Описание</span><span class="sxs-lookup"><span data-stu-id="c0218-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c0218-120">id</span><span class="sxs-lookup"><span data-stu-id="c0218-120">id</span></span>|<span data-ttu-id="c0218-121">Int32</span><span class="sxs-lookup"><span data-stu-id="c0218-121">Int32</span></span>|<span data-ttu-id="c0218-122">Индекс сущности, упомянутого в **указанном объекте chatMessage.**</span><span class="sxs-lookup"><span data-stu-id="c0218-122">Index of an entity being mentioned in the specified **chatMessage**.</span></span> <span data-ttu-id="c0218-123">Соответствует значению {index} с соответствующим `<at id="{index}">` тегом в тексте сообщения.</span><span class="sxs-lookup"><span data-stu-id="c0218-123">Matches the {index} value in the corresponding `<at id="{index}">` tag in the message body.</span></span>|
|<span data-ttu-id="c0218-124">mentionText</span><span class="sxs-lookup"><span data-stu-id="c0218-124">mentionText</span></span>|<span data-ttu-id="c0218-125">строка</span><span class="sxs-lookup"><span data-stu-id="c0218-125">string</span></span>|<span data-ttu-id="c0218-126">Строка, представляющая упоминание.</span><span class="sxs-lookup"><span data-stu-id="c0218-126">String used to represent the mention.</span></span> <span data-ttu-id="c0218-127">Например, отображаемое имя пользователя, имя команды.</span><span class="sxs-lookup"><span data-stu-id="c0218-127">For example, a user's display name, a team name.</span></span>|
|<span data-ttu-id="c0218-128">mentioned</span><span class="sxs-lookup"><span data-stu-id="c0218-128">mentioned</span></span>|[<span data-ttu-id="c0218-129">identitySet</span><span class="sxs-lookup"><span data-stu-id="c0218-129">identitySet</span></span>](identityset.md)|<span data-ttu-id="c0218-130">Указанный объект (пользователь, приложение, команда или канал).</span><span class="sxs-lookup"><span data-stu-id="c0218-130">The entity (user, application, team, or channel) that was mentioned.</span></span>  <span data-ttu-id="c0218-131">Если это был канал или команда @mentioned, identitySet содержит свойство **беседы,** указывающее идентификатор команды или канала, и **свойство conversationIdentityType,** представляющее команду или канал.</span><span class="sxs-lookup"><span data-stu-id="c0218-131">If it was a channel or team that was @mentioned, the identitySet contains a **conversation** property giving the ID of the team/channel, and a **conversationIdentityType** property that represents either the team or channel.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="c0218-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c0218-132">JSON representation</span></span>

<span data-ttu-id="c0218-133">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c0218-133">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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
