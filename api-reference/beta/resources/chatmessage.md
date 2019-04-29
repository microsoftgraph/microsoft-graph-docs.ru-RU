---
title: Тип ресурса chatMessage
description: Представляет отдельное сообщение чата в объекте channel или chat. Сообщение может быть корневым или частью беседы, определяемой свойством **replyToId** в сообщении.
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 4c2631d0ba4883160c443000fa2ecb0e1853523d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339849"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="28081-104">Тип ресурса chatMessage</span><span class="sxs-lookup"><span data-stu-id="28081-104">chatMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28081-105">Представляет отдельное сообщение чата в [канале](channel.md) или [чате](chat.md).</span><span class="sxs-lookup"><span data-stu-id="28081-105">Represents an individual chat message within a channel or chat entity.</span></span> <span data-ttu-id="28081-106">Сообщение может быть корневым или частью беседы, определяемой свойством **replyToId** в сообщении.</span><span class="sxs-lookup"><span data-stu-id="28081-106">The message can be an root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>

## <a name="methods"></a><span data-ttu-id="28081-107">Методы</span><span class="sxs-lookup"><span data-stu-id="28081-107">Methods</span></span>

| <span data-ttu-id="28081-108">Метод</span><span class="sxs-lookup"><span data-stu-id="28081-108">Method</span></span>       | <span data-ttu-id="28081-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="28081-109">Return Type</span></span>  |<span data-ttu-id="28081-110">Описание</span><span class="sxs-lookup"><span data-stu-id="28081-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="28081-111">Перечисление сообщений в канале</span><span class="sxs-lookup"><span data-stu-id="28081-111">List Channel messages</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="28081-112">Коллекция [chatmessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="28081-112">[chatmessage](chatmessage.md) collection</span></span> | <span data-ttu-id="28081-113">Получение списка всех корневых сообщений в канале.</span><span class="sxs-lookup"><span data-stu-id="28081-113">Get the list of all root messages in a channel.</span></span>|
|[<span data-ttu-id="28081-114">Получение сообщения в канале</span><span class="sxs-lookup"><span data-stu-id="28081-114">Get Channel message</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="28081-115">chatmessage</span><span class="sxs-lookup"><span data-stu-id="28081-115">chatmessage</span></span>](chatmessage.md) | <span data-ttu-id="28081-116">Получение одного корневого сообщения из канала.</span><span class="sxs-lookup"><span data-stu-id="28081-116">Get a single root message from a channel.</span></span>|
|[<span data-ttu-id="28081-117">Перечисление ответов на сообщение</span><span class="sxs-lookup"><span data-stu-id="28081-117">List replies to a message</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="28081-118">Коллекция [chatmessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="28081-118">[chatmessage](chatmessage.md) collection</span></span>| <span data-ttu-id="28081-119">Получение списка всех ответов на сообщение в канале.</span><span class="sxs-lookup"><span data-stu-id="28081-119">Get the list of all replies to a message in channel.</span></span>|
|[<span data-ttu-id="28081-120">Получение ответа на сообщение</span><span class="sxs-lookup"><span data-stu-id="28081-120">Get a reply to a message</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="28081-121">chatmessage</span><span class="sxs-lookup"><span data-stu-id="28081-121">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="28081-122">Получение одного ответа на сообщение в канале.</span><span class="sxs-lookup"><span data-stu-id="28081-122">Get a single reply to a message in a channel.</span></span>|
|[<span data-ttu-id="28081-123">Отправка сообщения в канал</span><span class="sxs-lookup"><span data-stu-id="28081-123">Send a message in a channel</span></span>](../api/channel-post-chatmessage.md) | [<span data-ttu-id="28081-124">chatmessage</span><span class="sxs-lookup"><span data-stu-id="28081-124">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="28081-125">Создание сообщения верхнего уровня в канале.</span><span class="sxs-lookup"><span data-stu-id="28081-125">Create a new top-level message in a channel.</span></span>|
|[<span data-ttu-id="28081-126">Ответ на сообщение в канале</span><span class="sxs-lookup"><span data-stu-id="28081-126">Reply to a message in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="28081-127">chatmessage</span><span class="sxs-lookup"><span data-stu-id="28081-127">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="28081-128">Ответ на существующее сообщение в канале.</span><span class="sxs-lookup"><span data-stu-id="28081-128">Reply to an existing message in a channel.</span></span>|
|[<span data-ttu-id="28081-129">Список сообщений в чате</span><span class="sxs-lookup"><span data-stu-id="28081-129">List messages in a chat</span></span>](../api/chat-list-messages.md)  | [<span data-ttu-id="28081-130">chatMessage</span><span class="sxs-lookup"><span data-stu-id="28081-130">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="28081-131">Получение сообщений в индивидуальном или групповом чате.</span><span class="sxs-lookup"><span data-stu-id="28081-131">Get messages in a 1:1 or group chat.</span></span> |
|[<span data-ttu-id="28081-132">Получение сообщения в чате</span><span class="sxs-lookup"><span data-stu-id="28081-132">Get message in chat</span></span>](../api/chat-get-message.md)  | [<span data-ttu-id="28081-133">chatMessage</span><span class="sxs-lookup"><span data-stu-id="28081-133">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="28081-134">Получение одного сообщения в чате.</span><span class="sxs-lookup"><span data-stu-id="28081-134">Get a single reply to a message in a channel.</span></span> |


## <a name="properties"></a><span data-ttu-id="28081-135">Свойства</span><span class="sxs-lookup"><span data-stu-id="28081-135">Properties</span></span>
| <span data-ttu-id="28081-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="28081-136">Property</span></span>     | <span data-ttu-id="28081-137">Тип</span><span class="sxs-lookup"><span data-stu-id="28081-137">Type</span></span>   |<span data-ttu-id="28081-138">Описание</span><span class="sxs-lookup"><span data-stu-id="28081-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="28081-139">id</span><span class="sxs-lookup"><span data-stu-id="28081-139">id</span></span>|<span data-ttu-id="28081-140">String</span><span class="sxs-lookup"><span data-stu-id="28081-140">String</span></span>| <span data-ttu-id="28081-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="28081-141">Read-only.</span></span> <span data-ttu-id="28081-142">Уникальный идентификатор сообщения.</span><span class="sxs-lookup"><span data-stu-id="28081-142">Unique ID of the message.</span></span>|
|<span data-ttu-id="28081-143">replyToId</span><span class="sxs-lookup"><span data-stu-id="28081-143">replyToId</span></span>| <span data-ttu-id="28081-144">string</span><span class="sxs-lookup"><span data-stu-id="28081-144">string</span></span> | <span data-ttu-id="28081-145">Идентификатор родительского или корневого сообщения беседы.</span><span class="sxs-lookup"><span data-stu-id="28081-145">Id of the parent message/root message of the thread.</span></span> <span data-ttu-id="28081-146">(Применимо только к сообщениям в каналах, но не в чате)</span><span class="sxs-lookup"><span data-stu-id="28081-146">(Only applies to messages in channels not chats)</span></span> |
|<span data-ttu-id="28081-147">from</span><span class="sxs-lookup"><span data-stu-id="28081-147">from</span></span>|[<span data-ttu-id="28081-148">identitySet</span><span class="sxs-lookup"><span data-stu-id="28081-148">identitySet</span></span>](identityset.md)| <span data-ttu-id="28081-149">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="28081-149">Read only.</span></span> <span data-ttu-id="28081-150">Подробные сведения об отправителе сообщения.</span><span class="sxs-lookup"><span data-stu-id="28081-150">Details of the sender of the message.</span></span>|
|<span data-ttu-id="28081-151">etag</span><span class="sxs-lookup"><span data-stu-id="28081-151">etag</span></span>| <span data-ttu-id="28081-152">строка</span><span class="sxs-lookup"><span data-stu-id="28081-152">string</span></span> | <span data-ttu-id="28081-153">Номер версии сообщения.</span><span class="sxs-lookup"><span data-stu-id="28081-153">Version number of the message.</span></span> |
|<span data-ttu-id="28081-154">messageType</span><span class="sxs-lookup"><span data-stu-id="28081-154">messageType</span></span>|<span data-ttu-id="28081-155">Строка</span><span class="sxs-lookup"><span data-stu-id="28081-155">String</span></span>|<span data-ttu-id="28081-156">Тип сообщения. В настоящее время поддерживаются следующие значения: message, chatEvent, Typing.</span><span class="sxs-lookup"><span data-stu-id="28081-156">The type of message, current supported values are: message, chatEvent, Typing.</span></span>|
|<span data-ttu-id="28081-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="28081-157">createdDateTime</span></span>|<span data-ttu-id="28081-158">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28081-158">dateTimeOffset</span></span>|<span data-ttu-id="28081-159">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="28081-159">Read only.</span></span> <span data-ttu-id="28081-160">Метка времени создания сообщения.</span><span class="sxs-lookup"><span data-stu-id="28081-160">Timestamp of when the message was created.</span></span>|
|<span data-ttu-id="28081-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="28081-161">lastModifiedDateTime</span></span>|<span data-ttu-id="28081-162">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28081-162">dateTimeOffset</span></span>|<span data-ttu-id="28081-163">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="28081-163">Read only.</span></span> <span data-ttu-id="28081-164">Метка времени изменения или обновления сообщения.</span><span class="sxs-lookup"><span data-stu-id="28081-164">Timestamp of when the message was edited/updated.</span></span>|
|<span data-ttu-id="28081-165">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="28081-165">deletedDateTime</span></span>|<span data-ttu-id="28081-166">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28081-166">dateTimeOffset</span></span>|<span data-ttu-id="28081-167">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="28081-167">Read only.</span></span> <span data-ttu-id="28081-168">Метка времени, в которое сообщение было удалено, или значение null, если сообщение не было удалено.</span><span class="sxs-lookup"><span data-stu-id="28081-168">Timestamp at which the message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="28081-169">subject</span><span class="sxs-lookup"><span data-stu-id="28081-169">subject</span></span>|<span data-ttu-id="28081-170">string</span><span class="sxs-lookup"><span data-stu-id="28081-170">string</span></span>| <span data-ttu-id="28081-171">Тема сообщения в формате обычного текста.</span><span class="sxs-lookup"><span data-stu-id="28081-171">The subject of the message.</span></span>|
|<span data-ttu-id="28081-172">body</span><span class="sxs-lookup"><span data-stu-id="28081-172">body</span></span>|[<span data-ttu-id="28081-173">itemBody</span><span class="sxs-lookup"><span data-stu-id="28081-173">itemBody</span></span>](itembody.md)|<span data-ttu-id="28081-174">Представление содержимого сообщения в формате Plaintext/HTML.</span><span class="sxs-lookup"><span data-stu-id="28081-174">Plaintext/HTML representation of the content of the message.</span></span> <span data-ttu-id="28081-175">Представление определяется параметром contentType в тексте.</span><span class="sxs-lookup"><span data-stu-id="28081-175">Representation is specified by the contentType inside the body.</span></span> <span data-ttu-id="28081-176">Содержимое всегда имеет формат HTML, если сообщение содержит [chatMessageMention](chatmessagemention.md).</span><span class="sxs-lookup"><span data-stu-id="28081-176">The content is always in HTML if the message contains a [chatMessageMention](chatmessagemention.md).</span></span> |
|<span data-ttu-id="28081-177">summary</span><span class="sxs-lookup"><span data-stu-id="28081-177">summary</span></span>|<span data-ttu-id="28081-178">string</span><span class="sxs-lookup"><span data-stu-id="28081-178">string</span></span>| <span data-ttu-id="28081-179">Сводный текст сообщения, который можно использовать для push-уведомлений и представлений сводки или резервных представлений.</span><span class="sxs-lookup"><span data-stu-id="28081-179">Summary text of the message that could be used for push notifications and summary views or fall back views</span></span> <span data-ttu-id="28081-180">Относится только к сообщениям каналов, не к сообщениям чата.</span><span class="sxs-lookup"><span data-stu-id="28081-180">Only applies to channel messages, not chat messages.</span></span> |
|<span data-ttu-id="28081-181">attachments</span><span class="sxs-lookup"><span data-stu-id="28081-181">attachments</span></span>|<span data-ttu-id="28081-182">Коллекция [chatMessageAttachment](chatmessageattachment.md)</span><span class="sxs-lookup"><span data-stu-id="28081-182">[chatMessageAttachment](chatmessageattachment.md) collection</span></span> |<span data-ttu-id="28081-183">Вложенные файлы.</span><span class="sxs-lookup"><span data-stu-id="28081-183">Attached files.</span></span> <span data-ttu-id="28081-184">В настоящее время вложения доступны только для чтения. Отправка вложений не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28081-184">Attachments are currently read-only – sending attachments is not supported.</span></span> |
|<span data-ttu-id="28081-185">mentions</span><span class="sxs-lookup"><span data-stu-id="28081-185">mentions</span></span>|<span data-ttu-id="28081-186">Коллекция [chatMessageMention](chatmessagemention.md)</span><span class="sxs-lookup"><span data-stu-id="28081-186">[chatMessageMention](chatmessagemention.md) collection</span></span>| <span data-ttu-id="28081-187">Список сущностей, упомянутых в сообщении.</span><span class="sxs-lookup"><span data-stu-id="28081-187">List of entities mentioned in the message.</span></span> <span data-ttu-id="28081-188">В настоящее время поддерживаются значения user, bot, team и channel.</span><span class="sxs-lookup"><span data-stu-id="28081-188">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="28081-189">importance</span><span class="sxs-lookup"><span data-stu-id="28081-189">importance</span></span>| <span data-ttu-id="28081-190">строка</span><span class="sxs-lookup"><span data-stu-id="28081-190">string</span></span> | <span data-ttu-id="28081-191">Важность сообщения: Normal, High.</span><span class="sxs-lookup"><span data-stu-id="28081-191">The importance of the message: Normal, High.</span></span>|
|<span data-ttu-id="28081-192">reactions</span><span class="sxs-lookup"><span data-stu-id="28081-192">reactions</span></span>| <span data-ttu-id="28081-193">Коллекция [chatMessageReaction](chatmessagereaction.md)</span><span class="sxs-lookup"><span data-stu-id="28081-193">[chatMessageReaction](chatmessagereaction.md) collection</span></span> | <span data-ttu-id="28081-194">Реакции на сообщение (например, "Нравится").</span><span class="sxs-lookup"><span data-stu-id="28081-194">Reactions for this message (for example, Like)</span></span>|
|<span data-ttu-id="28081-195">языковые стандарты</span><span class="sxs-lookup"><span data-stu-id="28081-195">locale</span></span>|<span data-ttu-id="28081-196">string</span><span class="sxs-lookup"><span data-stu-id="28081-196">string</span></span>|<span data-ttu-id="28081-197">Язык сообщения, установленный клиентом.</span><span class="sxs-lookup"><span data-stu-id="28081-197">Locale of the message set by the client</span></span>|


## <a name="json-representation"></a><span data-ttu-id="28081-198">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="28081-198">JSON representation</span></span>

<span data-ttu-id="28081-199">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="28081-199">The following is a JSON representation of the resource.</span></span>

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
