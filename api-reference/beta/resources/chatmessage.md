---
title: Тип ресурса chatMessage
description: Представляет отдельное сообщение чата в объекте channel или chat. Сообщение может быть корневым или частью беседы, определяемой свойством **replyToId** в сообщении.
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: ea21d57134643c83406f449ee7cdad192afc0326
ms.sourcegitcommit: 624ac42e74533a9bf0d0d22b3b15adbb258fd594
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2019
ms.locfileid: "34709413"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="1b159-104">Тип ресурса chatMessage</span><span class="sxs-lookup"><span data-stu-id="1b159-104">chatMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b159-105">Представляет отдельное сообщение чата в [канале](channel.md) или [чате](chat.md).</span><span class="sxs-lookup"><span data-stu-id="1b159-105">Represents an individual chat message within a [channel](channel.md) or [chat](chat.md).</span></span>
<span data-ttu-id="1b159-106">Сообщение может быть корневым или частью беседы, определяемой свойством **replyToId** в сообщении.</span><span class="sxs-lookup"><span data-stu-id="1b159-106">The message can be a root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>

## <a name="methods"></a><span data-ttu-id="1b159-107">Методы</span><span class="sxs-lookup"><span data-stu-id="1b159-107">Methods</span></span>

| <span data-ttu-id="1b159-108">Метод</span><span class="sxs-lookup"><span data-stu-id="1b159-108">Method</span></span>       | <span data-ttu-id="1b159-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1b159-109">Return Type</span></span>  |<span data-ttu-id="1b159-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1b159-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1b159-111">Перечисление сообщений в канале</span><span class="sxs-lookup"><span data-stu-id="1b159-111">List Channel messages</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="1b159-112">Коллекция [chatmessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="1b159-112">[chatmessage](chatmessage.md) collection</span></span> | <span data-ttu-id="1b159-113">Получение списка всех корневых сообщений в канале.</span><span class="sxs-lookup"><span data-stu-id="1b159-113">Get the list of all root messages in a channel.</span></span>|
|[<span data-ttu-id="1b159-114">Получение сообщения в канале</span><span class="sxs-lookup"><span data-stu-id="1b159-114">Get Channel message</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="1b159-115">chatmessage</span><span class="sxs-lookup"><span data-stu-id="1b159-115">chatmessage</span></span>](chatmessage.md) | <span data-ttu-id="1b159-116">Получение одного корневого сообщения из канала.</span><span class="sxs-lookup"><span data-stu-id="1b159-116">Get a single root message from a channel.</span></span>|
|[<span data-ttu-id="1b159-117">Перечисление ответов на сообщение</span><span class="sxs-lookup"><span data-stu-id="1b159-117">List replies to a message</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="1b159-118">Коллекция [chatmessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="1b159-118">[chatmessage](chatmessage.md) collection</span></span>| <span data-ttu-id="1b159-119">Получение списка всех ответов на сообщение в канале.</span><span class="sxs-lookup"><span data-stu-id="1b159-119">Get the list of all replies to a message in channel.</span></span>|
|[<span data-ttu-id="1b159-120">Получение ответа на сообщение</span><span class="sxs-lookup"><span data-stu-id="1b159-120">Get a reply to a message</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="1b159-121">chatmessage</span><span class="sxs-lookup"><span data-stu-id="1b159-121">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="1b159-122">Получение одного ответа на сообщение в канале.</span><span class="sxs-lookup"><span data-stu-id="1b159-122">Get a single reply to a message in a channel.</span></span>|
|[<span data-ttu-id="1b159-123">Создание объекта chatMessage в канале</span><span class="sxs-lookup"><span data-stu-id="1b159-123">Create chatMessage in a channel</span></span>](../api/channel-post-messages.md) | [<span data-ttu-id="1b159-124">chatmessage</span><span class="sxs-lookup"><span data-stu-id="1b159-124">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="1b159-125">Создание сообщения верхнего уровня в канале.</span><span class="sxs-lookup"><span data-stu-id="1b159-125">Create a new top-level message in a channel.</span></span>|
|[<span data-ttu-id="1b159-126">Создание ответа на chatMessage в канале</span><span class="sxs-lookup"><span data-stu-id="1b159-126">Create chatMessage reply in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="1b159-127">chatmessage</span><span class="sxs-lookup"><span data-stu-id="1b159-127">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="1b159-128">Ответ на существующее сообщение в канале.</span><span class="sxs-lookup"><span data-stu-id="1b159-128">Reply to an existing message in a channel.</span></span>|
|[<span data-ttu-id="1b159-129">Список сообщений в чате</span><span class="sxs-lookup"><span data-stu-id="1b159-129">List messages in a chat</span></span>](../api/chat-list-messages.md)  | [<span data-ttu-id="1b159-130">chatMessage</span><span class="sxs-lookup"><span data-stu-id="1b159-130">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="1b159-131">Получение сообщений в индивидуальном или групповом чате.</span><span class="sxs-lookup"><span data-stu-id="1b159-131">Get messages in a 1:1 or group chat.</span></span> |
|[<span data-ttu-id="1b159-132">Получение сообщения в чате</span><span class="sxs-lookup"><span data-stu-id="1b159-132">Get message in chat</span></span>](../api/chat-get-message.md)  | [<span data-ttu-id="1b159-133">chatMessage</span><span class="sxs-lookup"><span data-stu-id="1b159-133">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="1b159-134">Получение одного сообщения в чате.</span><span class="sxs-lookup"><span data-stu-id="1b159-134">Get a single message in a chat.</span></span> |

## <a name="properties"></a><span data-ttu-id="1b159-135">Свойства</span><span class="sxs-lookup"><span data-stu-id="1b159-135">Properties</span></span>

| <span data-ttu-id="1b159-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="1b159-136">Property</span></span>   | <span data-ttu-id="1b159-137">Тип</span><span class="sxs-lookup"><span data-stu-id="1b159-137">Type</span></span> |<span data-ttu-id="1b159-138">Описание</span><span class="sxs-lookup"><span data-stu-id="1b159-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1b159-139">id</span><span class="sxs-lookup"><span data-stu-id="1b159-139">id</span></span>|<span data-ttu-id="1b159-140">String</span><span class="sxs-lookup"><span data-stu-id="1b159-140">String</span></span>| <span data-ttu-id="1b159-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1b159-141">Read-only.</span></span> <span data-ttu-id="1b159-142">Уникальный идентификатор сообщения.</span><span class="sxs-lookup"><span data-stu-id="1b159-142">Unique ID of the message.</span></span>|
|<span data-ttu-id="1b159-143">replyToId</span><span class="sxs-lookup"><span data-stu-id="1b159-143">replyToId</span></span>| <span data-ttu-id="1b159-144">строка</span><span class="sxs-lookup"><span data-stu-id="1b159-144">string</span></span> | <span data-ttu-id="1b159-145">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1b159-145">Read-only.</span></span> <span data-ttu-id="1b159-146">Идентификатор родительского или корневого сообщения беседы.</span><span class="sxs-lookup"><span data-stu-id="1b159-146">Id of the parent message/root message of the thread.</span></span> <span data-ttu-id="1b159-147">(Применимо только к сообщениям в каналах, но не в чате)</span><span class="sxs-lookup"><span data-stu-id="1b159-147">(Only applies to messages in channels not chats)</span></span> |
|<span data-ttu-id="1b159-148">from</span><span class="sxs-lookup"><span data-stu-id="1b159-148">from</span></span>|[<span data-ttu-id="1b159-149">identitySet</span><span class="sxs-lookup"><span data-stu-id="1b159-149">identitySet</span></span>](identityset.md)| <span data-ttu-id="1b159-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1b159-150">Read only.</span></span> <span data-ttu-id="1b159-151">Подробные сведения об отправителе сообщения.</span><span class="sxs-lookup"><span data-stu-id="1b159-151">Details of the sender of the message.</span></span>|
|<span data-ttu-id="1b159-152">etag</span><span class="sxs-lookup"><span data-stu-id="1b159-152">etag</span></span>| <span data-ttu-id="1b159-153">строка</span><span class="sxs-lookup"><span data-stu-id="1b159-153">string</span></span> | <span data-ttu-id="1b159-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1b159-154">Read-only.</span></span> <span data-ttu-id="1b159-155">Номер версии сообщения.</span><span class="sxs-lookup"><span data-stu-id="1b159-155">Version number of the message.</span></span> |
|<span data-ttu-id="1b159-156">messageType</span><span class="sxs-lookup"><span data-stu-id="1b159-156">messageType</span></span>|<span data-ttu-id="1b159-157">chatMessageType</span><span class="sxs-lookup"><span data-stu-id="1b159-157">chatMessageType</span></span>|<span data-ttu-id="1b159-158">Тип сообщения.</span><span class="sxs-lookup"><span data-stu-id="1b159-158">The type of message.</span></span> <span data-ttu-id="1b159-159">Возможные значения: `message`.</span><span class="sxs-lookup"><span data-stu-id="1b159-159">The possible values are: `message`, , .</span></span>|
|<span data-ttu-id="1b159-160">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1b159-160">createdDateTime</span></span>|<span data-ttu-id="1b159-161">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b159-161">dateTimeOffset</span></span>|<span data-ttu-id="1b159-162">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1b159-162">Read only.</span></span> <span data-ttu-id="1b159-163">Метка времени создания сообщения.</span><span class="sxs-lookup"><span data-stu-id="1b159-163">Timestamp of when the message was created.</span></span>|
|<span data-ttu-id="1b159-164">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1b159-164">lastModifiedDateTime</span></span>|<span data-ttu-id="1b159-165">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b159-165">dateTimeOffset</span></span>|<span data-ttu-id="1b159-166">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1b159-166">Read only.</span></span> <span data-ttu-id="1b159-167">Метка времени изменения или обновления сообщения.</span><span class="sxs-lookup"><span data-stu-id="1b159-167">Timestamp of when the message was edited/updated.</span></span>|
|<span data-ttu-id="1b159-168">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="1b159-168">deletedDateTime</span></span>|<span data-ttu-id="1b159-169">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b159-169">dateTimeOffset</span></span>|<span data-ttu-id="1b159-170">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1b159-170">Read only.</span></span> <span data-ttu-id="1b159-171">Метка времени, в которое сообщение было удалено, или значение null, если сообщение не было удалено.</span><span class="sxs-lookup"><span data-stu-id="1b159-171">Timestamp at which the message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="1b159-172">subject</span><span class="sxs-lookup"><span data-stu-id="1b159-172">subject</span></span>|<span data-ttu-id="1b159-173">string</span><span class="sxs-lookup"><span data-stu-id="1b159-173">string</span></span>| <span data-ttu-id="1b159-174">Тема сообщения в формате обычного текста.</span><span class="sxs-lookup"><span data-stu-id="1b159-174">The subject of the message, in plaintext.</span></span>|
|<span data-ttu-id="1b159-175">body</span><span class="sxs-lookup"><span data-stu-id="1b159-175">body</span></span>|[<span data-ttu-id="1b159-176">itemBody</span><span class="sxs-lookup"><span data-stu-id="1b159-176">itemBody</span></span>](itembody.md)|<span data-ttu-id="1b159-177">Представление содержимого сообщения в формате Plaintext/HTML.</span><span class="sxs-lookup"><span data-stu-id="1b159-177">Plaintext/HTML representation of the content of the message.</span></span> <span data-ttu-id="1b159-178">Представление определяется параметром contentType в тексте.</span><span class="sxs-lookup"><span data-stu-id="1b159-178">Representation is specified by the contentType inside the body.</span></span> <span data-ttu-id="1b159-179">Содержимое всегда имеет формат HTML, если сообщение содержит [chatMessageMention](chatmessagemention.md).</span><span class="sxs-lookup"><span data-stu-id="1b159-179">The content is always in HTML if the message contains a [chatMessageMention](chatmessagemention.md).</span></span> |
|<span data-ttu-id="1b159-180">summary</span><span class="sxs-lookup"><span data-stu-id="1b159-180">summary</span></span>|<span data-ttu-id="1b159-181">string</span><span class="sxs-lookup"><span data-stu-id="1b159-181">string</span></span>| <span data-ttu-id="1b159-182">Сводный текст сообщения, который можно использовать для push-уведомлений и представлений сводки или резервных представлений.</span><span class="sxs-lookup"><span data-stu-id="1b159-182">Summary text of the message that could be used for push notifications and summary views or fall back views.</span></span> <span data-ttu-id="1b159-183">Относится только к сообщениям каналов, не к сообщениям чата.</span><span class="sxs-lookup"><span data-stu-id="1b159-183">Only applies to channel messages, not chat messages.</span></span> |
|<span data-ttu-id="1b159-184">attachments</span><span class="sxs-lookup"><span data-stu-id="1b159-184">attachments</span></span>|<span data-ttu-id="1b159-185">Коллекция [chatMessageAttachment](chatmessageattachment.md)</span><span class="sxs-lookup"><span data-stu-id="1b159-185">[chatMessageAttachment](chatmessageattachment.md) collection</span></span> |<span data-ttu-id="1b159-186">Вложенные файлы.</span><span class="sxs-lookup"><span data-stu-id="1b159-186">Attached files.</span></span> <span data-ttu-id="1b159-187">В настоящее время вложения доступны только для чтения. Отправка вложений не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b159-187">Attachments are currently read-only – sending attachments is not supported.</span></span> |
|<span data-ttu-id="1b159-188">mentions</span><span class="sxs-lookup"><span data-stu-id="1b159-188">mentions</span></span>|<span data-ttu-id="1b159-189">Коллекция [chatMessageMention](chatmessagemention.md)</span><span class="sxs-lookup"><span data-stu-id="1b159-189">[chatMessageMention](chatmessagemention.md) collection</span></span>| <span data-ttu-id="1b159-190">Список сущностей, упомянутых в сообщении.</span><span class="sxs-lookup"><span data-stu-id="1b159-190">List of entities mentioned in the message.</span></span> <span data-ttu-id="1b159-191">В настоящее время поддерживаются значения user, bot, team и channel.</span><span class="sxs-lookup"><span data-stu-id="1b159-191">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="1b159-192">importance</span><span class="sxs-lookup"><span data-stu-id="1b159-192">importance</span></span>| <span data-ttu-id="1b159-193">chatMessageImportance</span><span class="sxs-lookup"><span data-stu-id="1b159-193">chatMessageImportance</span></span> | <span data-ttu-id="1b159-194">Важность сообщения.</span><span class="sxs-lookup"><span data-stu-id="1b159-194">The importance of the message.</span></span> <span data-ttu-id="1b159-195">Допустимые значения: `normal`, `high`, `urgent`.</span><span class="sxs-lookup"><span data-stu-id="1b159-195">The possible values are: `normal`, `high`, `urgent`.</span></span>|
|<span data-ttu-id="1b159-196">reactions</span><span class="sxs-lookup"><span data-stu-id="1b159-196">reactions</span></span>| <span data-ttu-id="1b159-197">Коллекция [chatMessageReaction](chatmessagereaction.md)</span><span class="sxs-lookup"><span data-stu-id="1b159-197">[chatMessageReaction](chatmessagereaction.md) collection</span></span> | <span data-ttu-id="1b159-198">Реакции на сообщение (например, "Нравится").</span><span class="sxs-lookup"><span data-stu-id="1b159-198">Reactions for this message (for example, Like).</span></span>|
|<span data-ttu-id="1b159-199">языковые стандарты</span><span class="sxs-lookup"><span data-stu-id="1b159-199">locale</span></span>|<span data-ttu-id="1b159-200">string</span><span class="sxs-lookup"><span data-stu-id="1b159-200">string</span></span>|<span data-ttu-id="1b159-201">Язык сообщения, установленный клиентом.</span><span class="sxs-lookup"><span data-stu-id="1b159-201">Locale of the message set by the client.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="1b159-202">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="1b159-202">JSON representation</span></span>

<span data-ttu-id="1b159-203">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1b159-203">The following is a JSON representation of the resource.</span></span>

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
