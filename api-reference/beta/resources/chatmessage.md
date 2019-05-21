---
title: Тип ресурса chatMessage
description: Представляет отдельное сообщение чата в объекте channel или chat. Сообщение может быть корневым или частью беседы, определяемой свойством **replyToId** в сообщении.
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 0639fd0b5317abd4814123b500ec0548f78d05ac
ms.sourcegitcommit: abca7fcefeaa74b50f4600b35d816b626ba08468
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/21/2019
ms.locfileid: "34311163"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="ef1e4-104">Тип ресурса chatMessage</span><span class="sxs-lookup"><span data-stu-id="ef1e4-104">chatMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef1e4-105">Представляет отдельное сообщение чата в [канале](channel.md) или [чате](chat.md).</span><span class="sxs-lookup"><span data-stu-id="ef1e4-105">Represents an individual chat message within a [channel](channel.md) or [chat](chat.md).</span></span> <span data-ttu-id="ef1e4-106">Сообщение может быть корневым или частью беседы, определяемой свойством **replyToId** в сообщении.</span><span class="sxs-lookup"><span data-stu-id="ef1e4-106">The message can be a root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>

## <a name="methods"></a><span data-ttu-id="ef1e4-107">Методы</span><span class="sxs-lookup"><span data-stu-id="ef1e4-107">Methods</span></span>

| <span data-ttu-id="ef1e4-108">Метод</span><span class="sxs-lookup"><span data-stu-id="ef1e4-108">Method</span></span>       | <span data-ttu-id="ef1e4-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ef1e4-109">Return Type</span></span>  |<span data-ttu-id="ef1e4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ef1e4-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ef1e4-111">Перечисление сообщений в канале</span><span class="sxs-lookup"><span data-stu-id="ef1e4-111">List Channel messages</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="ef1e4-112">Коллекция [chatmessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="ef1e4-112">[chatmessage](chatmessage.md) collection</span></span> | <span data-ttu-id="ef1e4-113">Получение списка всех корневых сообщений в канале.</span><span class="sxs-lookup"><span data-stu-id="ef1e4-113">Get the list of all root messages in a channel.</span></span>|
|[<span data-ttu-id="ef1e4-114">Получение сообщения в канале</span><span class="sxs-lookup"><span data-stu-id="ef1e4-114">Get Channel message</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="ef1e4-115">chatmessage</span><span class="sxs-lookup"><span data-stu-id="ef1e4-115">chatmessage</span></span>](chatmessage.md) | <span data-ttu-id="ef1e4-116">Получение одного корневого сообщения из канала.</span><span class="sxs-lookup"><span data-stu-id="ef1e4-116">Get a single root message from a channel.</span></span>|
|[<span data-ttu-id="ef1e4-117">Перечисление ответов на сообщение</span><span class="sxs-lookup"><span data-stu-id="ef1e4-117">List replies to a message</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="ef1e4-118">Коллекция [chatmessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="ef1e4-118">[chatmessage](chatmessage.md) collection</span></span>| <span data-ttu-id="ef1e4-119">Получение списка всех ответов на сообщение в канале.</span><span class="sxs-lookup"><span data-stu-id="ef1e4-119">Get the list of all replies to a message in channel.</span></span>|
|[<span data-ttu-id="ef1e4-120">Получение ответа на сообщение</span><span class="sxs-lookup"><span data-stu-id="ef1e4-120">Get a reply to a message</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="ef1e4-121">chatmessage</span><span class="sxs-lookup"><span data-stu-id="ef1e4-121">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="ef1e4-122">Получение одного ответа на сообщение в канале.</span><span class="sxs-lookup"><span data-stu-id="ef1e4-122">Get a single reply to a message in a channel.</span></span>|
|[<span data-ttu-id="ef1e4-123">Отправка сообщения в канал</span><span class="sxs-lookup"><span data-stu-id="ef1e4-123">Send a message in a channel</span></span>](../api/channel-post-chatmessage.md) | [<span data-ttu-id="ef1e4-124">chatmessage</span><span class="sxs-lookup"><span data-stu-id="ef1e4-124">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="ef1e4-125">Создание сообщения верхнего уровня в канале.</span><span class="sxs-lookup"><span data-stu-id="ef1e4-125">Create a new top-level message in a channel.</span></span>|
|[<span data-ttu-id="ef1e4-126">Ответ на сообщение в канале</span><span class="sxs-lookup"><span data-stu-id="ef1e4-126">Reply to a message in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="ef1e4-127">chatmessage</span><span class="sxs-lookup"><span data-stu-id="ef1e4-127">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="ef1e4-128">Ответ на существующее сообщение в канале.</span><span class="sxs-lookup"><span data-stu-id="ef1e4-128">Reply to an existing message in a channel.</span></span>|
|[<span data-ttu-id="ef1e4-129">Список сообщений в чате</span><span class="sxs-lookup"><span data-stu-id="ef1e4-129">List messages in a chat</span></span>](../api/chat-list-messages.md)  | [<span data-ttu-id="ef1e4-130">chatMessage</span><span class="sxs-lookup"><span data-stu-id="ef1e4-130">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="ef1e4-131">Получение сообщений в индивидуальном или групповом чате.</span><span class="sxs-lookup"><span data-stu-id="ef1e4-131">Get messages in a 1:1 or group chat.</span></span> |
|[<span data-ttu-id="ef1e4-132">Получение сообщения в чате</span><span class="sxs-lookup"><span data-stu-id="ef1e4-132">Get message in chat</span></span>](../api/chat-get-message.md)  | [<span data-ttu-id="ef1e4-133">chatMessage</span><span class="sxs-lookup"><span data-stu-id="ef1e4-133">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="ef1e4-134">Получение одного сообщения в чате.</span><span class="sxs-lookup"><span data-stu-id="ef1e4-134">Get a single message in a chat.</span></span> |


## <a name="properties"></a><span data-ttu-id="ef1e4-135">Свойства</span><span class="sxs-lookup"><span data-stu-id="ef1e4-135">Properties</span></span>
| <span data-ttu-id="ef1e4-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="ef1e4-136">Property</span></span>     | <span data-ttu-id="ef1e4-137">Тип</span><span class="sxs-lookup"><span data-stu-id="ef1e4-137">Type</span></span>   |<span data-ttu-id="ef1e4-138">Описание</span><span class="sxs-lookup"><span data-stu-id="ef1e4-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ef1e4-139">id</span><span class="sxs-lookup"><span data-stu-id="ef1e4-139">id</span></span>|<span data-ttu-id="ef1e4-140">String</span><span class="sxs-lookup"><span data-stu-id="ef1e4-140">String</span></span>| <span data-ttu-id="ef1e4-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef1e4-141">Read-only.</span></span> <span data-ttu-id="ef1e4-142">Уникальный идентификатор сообщения.</span><span class="sxs-lookup"><span data-stu-id="ef1e4-142">Unique ID of the message.</span></span>|
|<span data-ttu-id="ef1e4-143">replyToId</span><span class="sxs-lookup"><span data-stu-id="ef1e4-143">replyToId</span></span>| <span data-ttu-id="ef1e4-144">string</span><span class="sxs-lookup"><span data-stu-id="ef1e4-144">string</span></span> | <span data-ttu-id="ef1e4-145">Идентификатор родительского или корневого сообщения беседы.</span><span class="sxs-lookup"><span data-stu-id="ef1e4-145">Id of the parent message/root message of the thread.</span></span> <span data-ttu-id="ef1e4-146">(Применимо только к сообщениям в каналах, но не в чате)</span><span class="sxs-lookup"><span data-stu-id="ef1e4-146">(Only applies to messages in channels not chats)</span></span> |
|<span data-ttu-id="ef1e4-147">from</span><span class="sxs-lookup"><span data-stu-id="ef1e4-147">from</span></span>|[<span data-ttu-id="ef1e4-148">identitySet</span><span class="sxs-lookup"><span data-stu-id="ef1e4-148">identitySet</span></span>](identityset.md)| <span data-ttu-id="ef1e4-149">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef1e4-149">Read only.</span></span> <span data-ttu-id="ef1e4-150">Подробные сведения об отправителе сообщения.</span><span class="sxs-lookup"><span data-stu-id="ef1e4-150">Details of the sender of the message.</span></span>|
|<span data-ttu-id="ef1e4-151">etag</span><span class="sxs-lookup"><span data-stu-id="ef1e4-151">etag</span></span>| <span data-ttu-id="ef1e4-152">string</span><span class="sxs-lookup"><span data-stu-id="ef1e4-152">string</span></span> | <span data-ttu-id="ef1e4-153">Номер версии сообщения.</span><span class="sxs-lookup"><span data-stu-id="ef1e4-153">Version number of the message.</span></span> |
|<span data-ttu-id="ef1e4-154">messageType</span><span class="sxs-lookup"><span data-stu-id="ef1e4-154">messageType</span></span>|<span data-ttu-id="ef1e4-155">String</span><span class="sxs-lookup"><span data-stu-id="ef1e4-155">String</span></span>|<span data-ttu-id="ef1e4-156">Тип сообщения. В настоящее время поддерживаются следующие значения: message, chatEvent, Typing.</span><span class="sxs-lookup"><span data-stu-id="ef1e4-156">The type of message, current supported values are: message, chatEvent, Typing.</span></span>|
|<span data-ttu-id="ef1e4-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ef1e4-157">createdDateTime</span></span>|<span data-ttu-id="ef1e4-158">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef1e4-158">dateTimeOffset</span></span>|<span data-ttu-id="ef1e4-159">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef1e4-159">Read only.</span></span> <span data-ttu-id="ef1e4-160">Метка времени создания сообщения.</span><span class="sxs-lookup"><span data-stu-id="ef1e4-160">Timestamp of when the message was created.</span></span>|
|<span data-ttu-id="ef1e4-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ef1e4-161">lastModifiedDateTime</span></span>|<span data-ttu-id="ef1e4-162">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef1e4-162">dateTimeOffset</span></span>|<span data-ttu-id="ef1e4-163">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef1e4-163">Read only.</span></span> <span data-ttu-id="ef1e4-164">Метка времени изменения или обновления сообщения.</span><span class="sxs-lookup"><span data-stu-id="ef1e4-164">Timestamp of when the message was edited/updated.</span></span>|
|<span data-ttu-id="ef1e4-165">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="ef1e4-165">deletedDateTime</span></span>|<span data-ttu-id="ef1e4-166">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef1e4-166">dateTimeOffset</span></span>|<span data-ttu-id="ef1e4-167">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef1e4-167">Read only.</span></span> <span data-ttu-id="ef1e4-168">Метка времени, в которое сообщение было удалено, или значение null, если сообщение не было удалено.</span><span class="sxs-lookup"><span data-stu-id="ef1e4-168">Timestamp at which the message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="ef1e4-169">subject</span><span class="sxs-lookup"><span data-stu-id="ef1e4-169">subject</span></span>|<span data-ttu-id="ef1e4-170">string</span><span class="sxs-lookup"><span data-stu-id="ef1e4-170">string</span></span>| <span data-ttu-id="ef1e4-171">Тема сообщения в формате обычного текста.</span><span class="sxs-lookup"><span data-stu-id="ef1e4-171">The subject of the message, in plaintext.</span></span>|
|<span data-ttu-id="ef1e4-172">body</span><span class="sxs-lookup"><span data-stu-id="ef1e4-172">body</span></span>|[<span data-ttu-id="ef1e4-173">itemBody</span><span class="sxs-lookup"><span data-stu-id="ef1e4-173">itemBody</span></span>](itembody.md)|<span data-ttu-id="ef1e4-174">Представление содержимого сообщения в формате Plaintext/HTML.</span><span class="sxs-lookup"><span data-stu-id="ef1e4-174">Plaintext/HTML representation of the content of the message.</span></span> <span data-ttu-id="ef1e4-175">Представление определяется параметром contentType в тексте.</span><span class="sxs-lookup"><span data-stu-id="ef1e4-175">Representation is specified by the contentType inside the body.</span></span> <span data-ttu-id="ef1e4-176">Содержимое всегда имеет формат HTML, если сообщение содержит [chatMessageMention](chatmessagemention.md).</span><span class="sxs-lookup"><span data-stu-id="ef1e4-176">The content is always in HTML if the message contains a [chatMessageMention](chatmessagemention.md).</span></span> |
|<span data-ttu-id="ef1e4-177">summary</span><span class="sxs-lookup"><span data-stu-id="ef1e4-177">summary</span></span>|<span data-ttu-id="ef1e4-178">string</span><span class="sxs-lookup"><span data-stu-id="ef1e4-178">string</span></span>| <span data-ttu-id="ef1e4-179">Сводный текст сообщения, который можно использовать для push-уведомлений и представлений сводки или резервных представлений.</span><span class="sxs-lookup"><span data-stu-id="ef1e4-179">Summary text of the message that could be used for push notifications and summary views or fall back views.</span></span> <span data-ttu-id="ef1e4-180">Относится только к сообщениям каналов, не к сообщениям чата.</span><span class="sxs-lookup"><span data-stu-id="ef1e4-180">Only applies to channel messages, not chat messages.</span></span> |
|<span data-ttu-id="ef1e4-181">attachments</span><span class="sxs-lookup"><span data-stu-id="ef1e4-181">attachments</span></span>|<span data-ttu-id="ef1e4-182">Коллекция [chatMessageAttachment](chatmessageattachment.md)</span><span class="sxs-lookup"><span data-stu-id="ef1e4-182">[chatMessageAttachment](chatmessageattachment.md) collection</span></span> |<span data-ttu-id="ef1e4-183">Вложенные файлы.</span><span class="sxs-lookup"><span data-stu-id="ef1e4-183">Attached files.</span></span> <span data-ttu-id="ef1e4-184">В настоящее время вложения доступны только для чтения. Отправка вложений не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef1e4-184">Attachments are currently read-only – sending attachments is not supported.</span></span> |
|<span data-ttu-id="ef1e4-185">mentions</span><span class="sxs-lookup"><span data-stu-id="ef1e4-185">mentions</span></span>|<span data-ttu-id="ef1e4-186">Коллекция [chatMessageMention](chatmessagemention.md)</span><span class="sxs-lookup"><span data-stu-id="ef1e4-186">[chatMessageMention](chatmessagemention.md) collection</span></span>| <span data-ttu-id="ef1e4-187">Список сущностей, упомянутых в сообщении.</span><span class="sxs-lookup"><span data-stu-id="ef1e4-187">List of entities mentioned in the message.</span></span> <span data-ttu-id="ef1e4-188">В настоящее время поддерживаются значения user, bot, team и channel.</span><span class="sxs-lookup"><span data-stu-id="ef1e4-188">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="ef1e4-189">importance</span><span class="sxs-lookup"><span data-stu-id="ef1e4-189">importance</span></span>| <span data-ttu-id="ef1e4-190">string</span><span class="sxs-lookup"><span data-stu-id="ef1e4-190">string</span></span> | <span data-ttu-id="ef1e4-191">Важность сообщения: Normal, High.</span><span class="sxs-lookup"><span data-stu-id="ef1e4-191">The importance of the message: Normal, High.</span></span>|
|<span data-ttu-id="ef1e4-192">reactions</span><span class="sxs-lookup"><span data-stu-id="ef1e4-192">reactions</span></span>| <span data-ttu-id="ef1e4-193">Коллекция [chatMessageReaction](chatmessagereaction.md)</span><span class="sxs-lookup"><span data-stu-id="ef1e4-193">[chatMessageReaction](chatmessagereaction.md) collection</span></span> | <span data-ttu-id="ef1e4-194">Реакции на сообщение (например, "Нравится").</span><span class="sxs-lookup"><span data-stu-id="ef1e4-194">Reactions for this message (for example, Like).</span></span>|
|<span data-ttu-id="ef1e4-195">языковые стандарты</span><span class="sxs-lookup"><span data-stu-id="ef1e4-195">locale</span></span>|<span data-ttu-id="ef1e4-196">string</span><span class="sxs-lookup"><span data-stu-id="ef1e4-196">string</span></span>|<span data-ttu-id="ef1e4-197">Язык сообщения, установленный клиентом.</span><span class="sxs-lookup"><span data-stu-id="ef1e4-197">Locale of the message set by the client.</span></span>|
|<span data-ttu-id="ef1e4-198">webUrl</span><span class="sxs-lookup"><span data-stu-id="ef1e4-198">webUrl</span></span>|<span data-ttu-id="ef1e4-199">string</span><span class="sxs-lookup"><span data-stu-id="ef1e4-199">string</span></span>|<span data-ttu-id="ef1e4-200">Гиперссылка, ведущая к каналу в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="ef1e4-200">A hyperlink that will navigate to the channel in Microsoft Teams.</span></span> <span data-ttu-id="ef1e4-201">Это URL-адрес, получаемый при щелчке правой кнопкой мыши по каналу в Microsoft Teams и выборе пункта "Получить ссылку на канал".</span><span class="sxs-lookup"><span data-stu-id="ef1e4-201">This is the URL that you get when you right-click a channel in Microsoft Teams and select Get link to channel.</span></span> <span data-ttu-id="ef1e4-202">Этот URL-адрес должен обрабатываться как непрозрачный BLOB-объект и не должен анализироваться.</span><span class="sxs-lookup"><span data-stu-id="ef1e4-202">This URL should be treated as an opaque blob, and not parsed.</span></span> <span data-ttu-id="ef1e4-203">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef1e4-203">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ef1e4-204">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ef1e4-204">JSON representation</span></span>

<span data-ttu-id="ef1e4-205">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ef1e4-205">The following is a JSON representation of the resource.</span></span>

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
