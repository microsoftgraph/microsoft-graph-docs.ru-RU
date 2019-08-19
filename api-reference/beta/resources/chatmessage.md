---
title: Тип ресурса chatMessage
description: Представляет отдельное сообщение чата в объекте channel или chat. Сообщение может быть корневым или частью беседы, определяемой свойством **replyToId** в сообщении.
doc_type: resourcePageType
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: 17b6912312c66bca8b84ccce9d25ac3c83a2edf9
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2019
ms.locfileid: "36460768"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="c2174-104">Тип ресурса chatMessage</span><span class="sxs-lookup"><span data-stu-id="c2174-104">chatMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2174-105">Представляет отдельное сообщение чата в [канале](channel.md) или [чате](chat.md).</span><span class="sxs-lookup"><span data-stu-id="c2174-105">Represents an individual chat message within a [channel](channel.md) or [chat](chat.md).</span></span>
<span data-ttu-id="c2174-106">Сообщение может быть корневым или частью беседы, определяемой свойством **replyToId** в сообщении.</span><span class="sxs-lookup"><span data-stu-id="c2174-106">The message can be a root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>

## <a name="methods"></a><span data-ttu-id="c2174-107">Методы</span><span class="sxs-lookup"><span data-stu-id="c2174-107">Methods</span></span>

| <span data-ttu-id="c2174-108">Метод</span><span class="sxs-lookup"><span data-stu-id="c2174-108">Method</span></span>       | <span data-ttu-id="c2174-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c2174-109">Return Type</span></span>  |<span data-ttu-id="c2174-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c2174-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c2174-111">Перечисление сообщений в канале</span><span class="sxs-lookup"><span data-stu-id="c2174-111">List Channel messages</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="c2174-112">Коллекция [chatMessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="c2174-112">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="c2174-113">Список всех корневых сообщений в канале.</span><span class="sxs-lookup"><span data-stu-id="c2174-113">List of all root messages in a channel.</span></span>|
|[<span data-ttu-id="c2174-114">Получение сообщения в канале</span><span class="sxs-lookup"><span data-stu-id="c2174-114">Get Channel message</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="c2174-115">chatMessage</span><span class="sxs-lookup"><span data-stu-id="c2174-115">chatMessage</span></span>](chatmessage.md) | <span data-ttu-id="c2174-116">Получение одного корневого сообщения из канала.</span><span class="sxs-lookup"><span data-stu-id="c2174-116">Get a single root message from a channel.</span></span>|
|[<span data-ttu-id="c2174-117">Перечисление ответов на сообщение</span><span class="sxs-lookup"><span data-stu-id="c2174-117">List replies to a message</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="c2174-118">Коллекция [chatMessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="c2174-118">[chatMessage](chatmessage.md) collection</span></span>| <span data-ttu-id="c2174-119">Список всех ответов на сообщение в канале.</span><span class="sxs-lookup"><span data-stu-id="c2174-119">List of all replies to a message in channel.</span></span>|
|[<span data-ttu-id="c2174-120">Получение ответа на сообщение</span><span class="sxs-lookup"><span data-stu-id="c2174-120">Get a reply to a message</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="c2174-121">chatMessage</span><span class="sxs-lookup"><span data-stu-id="c2174-121">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="c2174-122">Получение одного ответа на сообщение в канале.</span><span class="sxs-lookup"><span data-stu-id="c2174-122">Get a single reply to a message in a channel.</span></span>|
|[<span data-ttu-id="c2174-123">Создание chatMessage в канале</span><span class="sxs-lookup"><span data-stu-id="c2174-123">Create chatMessage in a channel</span></span>](../api/channel-post-messages.md) | [<span data-ttu-id="c2174-124">chatMessage</span><span class="sxs-lookup"><span data-stu-id="c2174-124">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="c2174-125">Создание сообщения верхнего уровня в канале.</span><span class="sxs-lookup"><span data-stu-id="c2174-125">Create a new top-level message in a channel.</span></span>|
|[<span data-ttu-id="c2174-126">Ответ на сообщение в канале</span><span class="sxs-lookup"><span data-stu-id="c2174-126">Reply to a message in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="c2174-127">chatMessage</span><span class="sxs-lookup"><span data-stu-id="c2174-127">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="c2174-128">Ответ на существующее сообщение в канале.</span><span class="sxs-lookup"><span data-stu-id="c2174-128">Reply to an existing message in a channel.</span></span>|
|[<span data-ttu-id="c2174-129">Создание chatMessage в чате</span><span class="sxs-lookup"><span data-stu-id="c2174-129">Create chatMessage in a chat</span></span>](../api/chat-post-messages.md) | [<span data-ttu-id="c2174-130">chatMessage</span><span class="sxs-lookup"><span data-stu-id="c2174-130">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="c2174-131">Отправка сообщения в существующей беседе в Интернете 1:1 или группе.</span><span class="sxs-lookup"><span data-stu-id="c2174-131">Send a message in an existing 1:1 or group chat conversation.</span></span>|
|[<span data-ttu-id="c2174-132">Список сообщений в чате</span><span class="sxs-lookup"><span data-stu-id="c2174-132">List messages in a chat</span></span>](../api/chatmessage-list.md)  | [<span data-ttu-id="c2174-133">chatMessage</span><span class="sxs-lookup"><span data-stu-id="c2174-133">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="c2174-134">Перечисление сообщений в сообщениях в формате 1:1 или Group Chat.</span><span class="sxs-lookup"><span data-stu-id="c2174-134">List messages in a 1:1 or group chat.</span></span> |
|[<span data-ttu-id="c2174-135">Получение сообщения в чате</span><span class="sxs-lookup"><span data-stu-id="c2174-135">Get message in chat</span></span>](../api/chatmessage-get.md)  | [<span data-ttu-id="c2174-136">chatMessage</span><span class="sxs-lookup"><span data-stu-id="c2174-136">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="c2174-137">Получение одного сообщения в чате.</span><span class="sxs-lookup"><span data-stu-id="c2174-137">Get a single message in a chat.</span></span> |
|[<span data-ttu-id="c2174-138">Перечисление всех размещенных изображений</span><span class="sxs-lookup"><span data-stu-id="c2174-138">List all hosted images</span></span>](../api/chatmessagehostedimage-list-hostedimages.md) | <span data-ttu-id="c2174-139">Коллекция [хостедимаже](../resources/chatmessagehostedimage.md)</span><span class="sxs-lookup"><span data-stu-id="c2174-139">[hostedImage](../resources/chatmessagehostedimage.md) collection</span></span>| <span data-ttu-id="c2174-140">Получение всех размещенных изображений в сообщении.</span><span class="sxs-lookup"><span data-stu-id="c2174-140">Get all hosted images in a message.</span></span>|
|[<span data-ttu-id="c2174-141">Получение размещенного изображения</span><span class="sxs-lookup"><span data-stu-id="c2174-141">Get hosted image</span></span>](../api/chatmessagehostedimage-get.md) | [<span data-ttu-id="c2174-142">хостедимаже</span><span class="sxs-lookup"><span data-stu-id="c2174-142">hostedImage</span></span>](../resources/chatmessagehostedimage.md) | <span data-ttu-id="c2174-143">Получение размещенного изображения из сообщения.</span><span class="sxs-lookup"><span data-stu-id="c2174-143">Get a hosted image from a message.</span></span>|
|[<span data-ttu-id="c2174-144">Получение байтов размещенного изображения</span><span class="sxs-lookup"><span data-stu-id="c2174-144">Get hosted image bytes</span></span>](../api/chatmessagehostedimage-getbytes.md) | <span data-ttu-id="c2174-145">данные двоичных изображений</span><span class="sxs-lookup"><span data-stu-id="c2174-145">binary image data</span></span> | <span data-ttu-id="c2174-146">Получение двоичных данных изображения на размещенном изображении из сообщения.</span><span class="sxs-lookup"><span data-stu-id="c2174-146">Get binary image data of a hosted image from a message.</span></span>|

## <a name="properties"></a><span data-ttu-id="c2174-147">Свойства</span><span class="sxs-lookup"><span data-stu-id="c2174-147">Properties</span></span>

| <span data-ttu-id="c2174-148">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2174-148">Property</span></span>   | <span data-ttu-id="c2174-149">Тип</span><span class="sxs-lookup"><span data-stu-id="c2174-149">Type</span></span> |<span data-ttu-id="c2174-150">Описание</span><span class="sxs-lookup"><span data-stu-id="c2174-150">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c2174-151">id</span><span class="sxs-lookup"><span data-stu-id="c2174-151">id</span></span>|<span data-ttu-id="c2174-152">String</span><span class="sxs-lookup"><span data-stu-id="c2174-152">String</span></span>| <span data-ttu-id="c2174-153">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c2174-153">Read-only.</span></span> <span data-ttu-id="c2174-154">Уникальный идентификатор сообщения.</span><span class="sxs-lookup"><span data-stu-id="c2174-154">Unique Id of the message.</span></span>|
|<span data-ttu-id="c2174-155">replyToId</span><span class="sxs-lookup"><span data-stu-id="c2174-155">replyToId</span></span>| <span data-ttu-id="c2174-156">string</span><span class="sxs-lookup"><span data-stu-id="c2174-156">string</span></span> | <span data-ttu-id="c2174-157">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c2174-157">Read-only.</span></span> <span data-ttu-id="c2174-158">Идентификатор родительского или корневого сообщения беседы.</span><span class="sxs-lookup"><span data-stu-id="c2174-158">Id of the parent message/root message of the thread.</span></span> <span data-ttu-id="c2174-159">(Применимо только к сообщениям в каналах, но не в чате)</span><span class="sxs-lookup"><span data-stu-id="c2174-159">(Only applies to messages in channels not chats)</span></span> |
|<span data-ttu-id="c2174-160">from</span><span class="sxs-lookup"><span data-stu-id="c2174-160">from</span></span>|[<span data-ttu-id="c2174-161">identitySet</span><span class="sxs-lookup"><span data-stu-id="c2174-161">identitySet</span></span>](identityset.md)| <span data-ttu-id="c2174-162">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c2174-162">Read only.</span></span> <span data-ttu-id="c2174-163">Подробные сведения об отправителе сообщения.</span><span class="sxs-lookup"><span data-stu-id="c2174-163">Details of the sender of the message.</span></span>|
|<span data-ttu-id="c2174-164">etag</span><span class="sxs-lookup"><span data-stu-id="c2174-164">etag</span></span>| <span data-ttu-id="c2174-165">string</span><span class="sxs-lookup"><span data-stu-id="c2174-165">string</span></span> | <span data-ttu-id="c2174-166">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c2174-166">Read-only.</span></span> <span data-ttu-id="c2174-167">Номер версии сообщения.</span><span class="sxs-lookup"><span data-stu-id="c2174-167">Version number of the message.</span></span> |
|<span data-ttu-id="c2174-168">messageType</span><span class="sxs-lookup"><span data-stu-id="c2174-168">messageType</span></span>|<span data-ttu-id="c2174-169">чатмессажетипе</span><span class="sxs-lookup"><span data-stu-id="c2174-169">chatMessageType</span></span>|<span data-ttu-id="c2174-170">Тип сообщения.</span><span class="sxs-lookup"><span data-stu-id="c2174-170">The type of message.</span></span> <span data-ttu-id="c2174-171">Возможные значения: `message`.</span><span class="sxs-lookup"><span data-stu-id="c2174-171">The possible values are: `message`.</span></span>|
|<span data-ttu-id="c2174-172">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c2174-172">createdDateTime</span></span>|<span data-ttu-id="c2174-173">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2174-173">dateTimeOffset</span></span>|<span data-ttu-id="c2174-174">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c2174-174">Read only.</span></span> <span data-ttu-id="c2174-175">Метка времени создания сообщения.</span><span class="sxs-lookup"><span data-stu-id="c2174-175">Timestamp of when the message was created.</span></span>|
|<span data-ttu-id="c2174-176">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c2174-176">lastModifiedDateTime</span></span>|<span data-ttu-id="c2174-177">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2174-177">dateTimeOffset</span></span>|<span data-ttu-id="c2174-178">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c2174-178">Read only.</span></span> <span data-ttu-id="c2174-179">Метка времени создания или изменения сообщения, включая время ответа (если это корневое сообщение в канале), а также добавление или удаление реакции.</span><span class="sxs-lookup"><span data-stu-id="c2174-179">Timestamp of when the message is created or edited, including when a reply is made (if it's a root message in a channel) or a reaction is added or removed.</span></span> |
|<span data-ttu-id="c2174-180">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="c2174-180">deletedDateTime</span></span>|<span data-ttu-id="c2174-181">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2174-181">dateTimeOffset</span></span>|<span data-ttu-id="c2174-182">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c2174-182">Read only.</span></span> <span data-ttu-id="c2174-183">Метка времени, в которое сообщение было удалено, или значение null, если сообщение не было удалено.</span><span class="sxs-lookup"><span data-stu-id="c2174-183">Timestamp at which the message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="c2174-184">subject</span><span class="sxs-lookup"><span data-stu-id="c2174-184">subject</span></span>|<span data-ttu-id="c2174-185">string</span><span class="sxs-lookup"><span data-stu-id="c2174-185">string</span></span>| <span data-ttu-id="c2174-186">Тема сообщения в формате обычного текста.</span><span class="sxs-lookup"><span data-stu-id="c2174-186">The subject of the message, in plaintext.</span></span>|
|<span data-ttu-id="c2174-187">body</span><span class="sxs-lookup"><span data-stu-id="c2174-187">body</span></span>|[<span data-ttu-id="c2174-188">itemBody</span><span class="sxs-lookup"><span data-stu-id="c2174-188">itemBody</span></span>](itembody.md)|<span data-ttu-id="c2174-189">Представление содержимого сообщения в формате Plaintext/HTML.</span><span class="sxs-lookup"><span data-stu-id="c2174-189">Plaintext/HTML representation of the content of the message.</span></span> <span data-ttu-id="c2174-190">Представление определяется параметром contentType в тексте.</span><span class="sxs-lookup"><span data-stu-id="c2174-190">Representation is specified by the contentType inside the body.</span></span> <span data-ttu-id="c2174-191">Содержимое всегда имеет формат HTML, если сообщение содержит [chatMessageMention](chatmessagemention.md).</span><span class="sxs-lookup"><span data-stu-id="c2174-191">The content is always in HTML if the message contains a [chatMessageMention](chatmessagemention.md).</span></span> |
|<span data-ttu-id="c2174-192">summary</span><span class="sxs-lookup"><span data-stu-id="c2174-192">summary</span></span>|<span data-ttu-id="c2174-193">string</span><span class="sxs-lookup"><span data-stu-id="c2174-193">string</span></span>| <span data-ttu-id="c2174-194">Сводный текст сообщения, который можно использовать для push-уведомлений и представлений сводки или резервных представлений.</span><span class="sxs-lookup"><span data-stu-id="c2174-194">Summary text of the message that could be used for push notifications and summary views or fall back views.</span></span> <span data-ttu-id="c2174-195">Относится только к сообщениям каналов, не к сообщениям чата.</span><span class="sxs-lookup"><span data-stu-id="c2174-195">Only applies to channel messages, not chat messages.</span></span> |
|<span data-ttu-id="c2174-196">attachments</span><span class="sxs-lookup"><span data-stu-id="c2174-196">attachments</span></span>|<span data-ttu-id="c2174-197">Коллекция [chatMessageAttachment](chatmessageattachment.md)</span><span class="sxs-lookup"><span data-stu-id="c2174-197">[chatMessageAttachment](chatmessageattachment.md) collection</span></span> |<span data-ttu-id="c2174-198">Вложенные файлы.</span><span class="sxs-lookup"><span data-stu-id="c2174-198">Attached files.</span></span> <span data-ttu-id="c2174-199">В настоящее время вложения доступны только для чтения. Отправка вложений не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2174-199">Attachments are currently read-only – sending attachments is not supported.</span></span> |
|<span data-ttu-id="c2174-200">mentions</span><span class="sxs-lookup"><span data-stu-id="c2174-200">mentions</span></span>|<span data-ttu-id="c2174-201">Коллекция [chatMessageMention](chatmessagemention.md)</span><span class="sxs-lookup"><span data-stu-id="c2174-201">[chatMessageMention](chatmessagemention.md) collection</span></span>| <span data-ttu-id="c2174-202">Список сущностей, упомянутых в сообщении.</span><span class="sxs-lookup"><span data-stu-id="c2174-202">List of entities mentioned in the message.</span></span> <span data-ttu-id="c2174-203">В настоящее время поддерживаются значения user, bot, team и channel.</span><span class="sxs-lookup"><span data-stu-id="c2174-203">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="c2174-204">importance</span><span class="sxs-lookup"><span data-stu-id="c2174-204">importance</span></span>| <span data-ttu-id="c2174-205">чатмессажеимпортанце</span><span class="sxs-lookup"><span data-stu-id="c2174-205">chatMessageImportance</span></span> | <span data-ttu-id="c2174-206">Важность сообщения.</span><span class="sxs-lookup"><span data-stu-id="c2174-206">The importance of the message.</span></span> <span data-ttu-id="c2174-207">Допустимые значения: `normal`, `high`, `urgent`.</span><span class="sxs-lookup"><span data-stu-id="c2174-207">The possible values are: `normal`, `high`, `urgent`.</span></span>|
|<span data-ttu-id="c2174-208">reactions</span><span class="sxs-lookup"><span data-stu-id="c2174-208">reactions</span></span>| <span data-ttu-id="c2174-209">Коллекция [chatMessageReaction](chatmessagereaction.md)</span><span class="sxs-lookup"><span data-stu-id="c2174-209">[chatMessageReaction](chatmessagereaction.md) collection</span></span> | <span data-ttu-id="c2174-210">Реакции на сообщение (например, "Нравится").</span><span class="sxs-lookup"><span data-stu-id="c2174-210">Reactions for this message (for example, Like).</span></span>|
|<span data-ttu-id="c2174-211">языковые стандарты</span><span class="sxs-lookup"><span data-stu-id="c2174-211">locale</span></span>|<span data-ttu-id="c2174-212">string</span><span class="sxs-lookup"><span data-stu-id="c2174-212">string</span></span>|<span data-ttu-id="c2174-213">Язык сообщения, установленный клиентом.</span><span class="sxs-lookup"><span data-stu-id="c2174-213">Locale of the message set by the client.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c2174-214">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c2174-214">JSON representation</span></span>

<span data-ttu-id="c2174-215">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2174-215">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "deleted",
    "deletedDateTime",
    "attachments",
    "importance",
    "reactions",
    "mentions",
    "subject",
    "summary"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessage"
}-->

```json
{
  "id": "string (identifier)",
  "replyToId": "string (identifier)",
  "from": {"@odata.type": "microsoft.graph.identitySet"},
  "etag": "string",
  "messageType": "string",
  "createdDateTime": "string (timestamp)",
  "lastModifiedDateTime": "string (timestamp)",
  "deletedDateTime": "string (timestamp)",
  "subject": "string",
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "summary": "string",
  "attachments": [{"@odata.type": "microsoft.graph.chatMessageAttachment"}],
  "mentions": [{"@odata.type": "microsoft.graph.chatMessageMention"}],
  "importance": "string",
  "policyViolation": "string",
  "reactions": [{"@odata.type": "microsoft.graph.chatMessageReaction"}],
  "locale": "string",
  "deleted": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chat message resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
