---
title: Тип ресурса chatMessage
description: Представляет отдельное сообщение чата в объекте channel или chat. Сообщение может быть корневым или частью беседы, определяемой свойством **replyToId** в сообщении.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: 269041dece2ab626c5f3d0ecccbf70d62c296ede
ms.sourcegitcommit: b523648530fcc8c2a3ded35b419be8047b9fcd10
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/20/2019
ms.locfileid: "35084049"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="67f19-104">Тип ресурса chatMessage</span><span class="sxs-lookup"><span data-stu-id="67f19-104">chatMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67f19-105">Представляет отдельное сообщение чата в [канале](channel.md) или [чате](chat.md).</span><span class="sxs-lookup"><span data-stu-id="67f19-105">Represents an individual chat message within a [channel](channel.md) or [chat](chat.md).</span></span>
<span data-ttu-id="67f19-106">Сообщение может быть корневым или частью беседы, определяемой свойством **replyToId** в сообщении.</span><span class="sxs-lookup"><span data-stu-id="67f19-106">The message can be a root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>

## <a name="methods"></a><span data-ttu-id="67f19-107">Методы</span><span class="sxs-lookup"><span data-stu-id="67f19-107">Methods</span></span>

| <span data-ttu-id="67f19-108">Метод</span><span class="sxs-lookup"><span data-stu-id="67f19-108">Method</span></span>       | <span data-ttu-id="67f19-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="67f19-109">Return Type</span></span>  |<span data-ttu-id="67f19-110">Описание</span><span class="sxs-lookup"><span data-stu-id="67f19-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="67f19-111">Перечисление сообщений в канале</span><span class="sxs-lookup"><span data-stu-id="67f19-111">List Channel messages</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="67f19-112">Коллекция [chatMessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="67f19-112">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="67f19-113">Список всех корневых сообщений в канале.</span><span class="sxs-lookup"><span data-stu-id="67f19-113">Get the list of all root messages in a channel.</span></span>|
|[<span data-ttu-id="67f19-114">Получение сообщения в канале</span><span class="sxs-lookup"><span data-stu-id="67f19-114">Get Channel message</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="67f19-115">chatMessage</span><span class="sxs-lookup"><span data-stu-id="67f19-115">chatMessage</span></span>](chatmessage.md) | <span data-ttu-id="67f19-116">Получение одного корневого сообщения из канала.</span><span class="sxs-lookup"><span data-stu-id="67f19-116">Get a single root message from a channel.</span></span>|
|[<span data-ttu-id="67f19-117">Перечисление ответов на сообщение</span><span class="sxs-lookup"><span data-stu-id="67f19-117">List replies to a message</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="67f19-118">Коллекция [chatMessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="67f19-118">[chatMessage](chatmessage.md) collection</span></span>| <span data-ttu-id="67f19-119">Список всех ответов на сообщение в канале.</span><span class="sxs-lookup"><span data-stu-id="67f19-119">Get the list of all replies to a message in channel.</span></span>|
|[<span data-ttu-id="67f19-120">Получение ответа на сообщение</span><span class="sxs-lookup"><span data-stu-id="67f19-120">Get a reply to a message</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="67f19-121">chatMessage</span><span class="sxs-lookup"><span data-stu-id="67f19-121">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="67f19-122">Получение одного ответа на сообщение в канале.</span><span class="sxs-lookup"><span data-stu-id="67f19-122">Get a single reply to a message in a channel.</span></span>|
|[<span data-ttu-id="67f19-123">Создание объекта chatMessage в канале</span><span class="sxs-lookup"><span data-stu-id="67f19-123">Create chatMessage in a channel</span></span>](../api/channel-post-messages.md) | [<span data-ttu-id="67f19-124">chatMessage</span><span class="sxs-lookup"><span data-stu-id="67f19-124">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="67f19-125">Создание сообщения верхнего уровня в канале.</span><span class="sxs-lookup"><span data-stu-id="67f19-125">Create a new top-level message in a channel.</span></span>|
|[<span data-ttu-id="67f19-126">Ответ на сообщение в канале</span><span class="sxs-lookup"><span data-stu-id="67f19-126">Reply to a message in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="67f19-127">chatMessage</span><span class="sxs-lookup"><span data-stu-id="67f19-127">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="67f19-128">Ответ на существующее сообщение в канале.</span><span class="sxs-lookup"><span data-stu-id="67f19-128">Reply to an existing message in a channel.</span></span>|
|[<span data-ttu-id="67f19-129">Список сообщений в чате</span><span class="sxs-lookup"><span data-stu-id="67f19-129">List messages in a chat</span></span>](../api/chat-list-messages.md)  | [<span data-ttu-id="67f19-130">chatMessage</span><span class="sxs-lookup"><span data-stu-id="67f19-130">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="67f19-131">Список сообщений в индивидуальном или групповом чате.</span><span class="sxs-lookup"><span data-stu-id="67f19-131">Get messages in a 1:1 or group chat.</span></span> |
|[<span data-ttu-id="67f19-132">Получение сообщения в чате</span><span class="sxs-lookup"><span data-stu-id="67f19-132">Get message in chat</span></span>](../api/chat-get-message.md)  | [<span data-ttu-id="67f19-133">chatMessage</span><span class="sxs-lookup"><span data-stu-id="67f19-133">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="67f19-134">Получение одного сообщения в чате.</span><span class="sxs-lookup"><span data-stu-id="67f19-134">Get a single message in a chat.</span></span> |
|[<span data-ttu-id="67f19-135">Перечисление всех размещенных изображений</span><span class="sxs-lookup"><span data-stu-id="67f19-135">List all hosted images</span></span>](../api/chatmessagehostedimage-list-hostedimages.md) | <span data-ttu-id="67f19-136">Коллекция [hostedImage](../resources/chatmessagehostedimage.md)</span><span class="sxs-lookup"><span data-stu-id="67f19-136">[hostedImage](../resources/chatmessagehostedimage.md) collection</span></span>| <span data-ttu-id="67f19-137">Получение всех изображений, размещенных в сообщении.</span><span class="sxs-lookup"><span data-stu-id="67f19-137">Get all hosted images in a message.</span></span>|
|[<span data-ttu-id="67f19-138">Получение размещенных изображений</span><span class="sxs-lookup"><span data-stu-id="67f19-138">Get hosted image</span></span>](../api/chatmessagehostedimage-get.md) | [<span data-ttu-id="67f19-139">hostedImage</span><span class="sxs-lookup"><span data-stu-id="67f19-139">hostedImage</span></span>](../resources/chatmessagehostedimage.md) | <span data-ttu-id="67f19-140">Получение размещенного изображения из сообщения.</span><span class="sxs-lookup"><span data-stu-id="67f19-140">Get a hosted image from a message.</span></span>|
|[<span data-ttu-id="67f19-141">Получение байтов размещенных изображений</span><span class="sxs-lookup"><span data-stu-id="67f19-141">Get hosted image bytes</span></span>](../api/chatmessagehostedimage-getbytes.md) | <span data-ttu-id="67f19-142">двоичные данные изображения</span><span class="sxs-lookup"><span data-stu-id="67f19-142">binary image data</span></span> | <span data-ttu-id="67f19-143">Получение двоичных данных размещенного изображения из сообщения.</span><span class="sxs-lookup"><span data-stu-id="67f19-143">Get binary image data of a hosted image from a message.</span></span>|

## <a name="properties"></a><span data-ttu-id="67f19-144">Свойства</span><span class="sxs-lookup"><span data-stu-id="67f19-144">Properties</span></span>

| <span data-ttu-id="67f19-145">Свойство</span><span class="sxs-lookup"><span data-stu-id="67f19-145">Property</span></span>   | <span data-ttu-id="67f19-146">Тип</span><span class="sxs-lookup"><span data-stu-id="67f19-146">Type</span></span> |<span data-ttu-id="67f19-147">Описание</span><span class="sxs-lookup"><span data-stu-id="67f19-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="67f19-148">id</span><span class="sxs-lookup"><span data-stu-id="67f19-148">id</span></span>|<span data-ttu-id="67f19-149">String</span><span class="sxs-lookup"><span data-stu-id="67f19-149">String</span></span>| <span data-ttu-id="67f19-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="67f19-150">Read-only.</span></span> <span data-ttu-id="67f19-151">Уникальный идентификатор сообщения.</span><span class="sxs-lookup"><span data-stu-id="67f19-151">Unique ID of the message.</span></span>|
|<span data-ttu-id="67f19-152">replyToId</span><span class="sxs-lookup"><span data-stu-id="67f19-152">replyToId</span></span>| <span data-ttu-id="67f19-153">строка</span><span class="sxs-lookup"><span data-stu-id="67f19-153">string</span></span> | <span data-ttu-id="67f19-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="67f19-154">Read-only.</span></span> <span data-ttu-id="67f19-155">Идентификатор родительского или корневого сообщения беседы.</span><span class="sxs-lookup"><span data-stu-id="67f19-155">Id of the parent message/root message of the thread.</span></span> <span data-ttu-id="67f19-156">(Применимо только к сообщениям в каналах, но не в чате)</span><span class="sxs-lookup"><span data-stu-id="67f19-156">(Only applies to messages in channels not chats)</span></span> |
|<span data-ttu-id="67f19-157">from</span><span class="sxs-lookup"><span data-stu-id="67f19-157">from</span></span>|[<span data-ttu-id="67f19-158">identitySet</span><span class="sxs-lookup"><span data-stu-id="67f19-158">identitySet</span></span>](identityset.md)| <span data-ttu-id="67f19-159">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="67f19-159">Read only.</span></span> <span data-ttu-id="67f19-160">Подробные сведения об отправителе сообщения.</span><span class="sxs-lookup"><span data-stu-id="67f19-160">Details of the sender of the message.</span></span>|
|<span data-ttu-id="67f19-161">etag</span><span class="sxs-lookup"><span data-stu-id="67f19-161">etag</span></span>| <span data-ttu-id="67f19-162">строка</span><span class="sxs-lookup"><span data-stu-id="67f19-162">string</span></span> | <span data-ttu-id="67f19-163">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="67f19-163">Read-only.</span></span> <span data-ttu-id="67f19-164">Номер версии сообщения.</span><span class="sxs-lookup"><span data-stu-id="67f19-164">Version number of the message.</span></span> |
|<span data-ttu-id="67f19-165">messageType</span><span class="sxs-lookup"><span data-stu-id="67f19-165">messageType</span></span>|<span data-ttu-id="67f19-166">chatMessageType</span><span class="sxs-lookup"><span data-stu-id="67f19-166">chatMessageType</span></span>|<span data-ttu-id="67f19-167">Тип сообщения.</span><span class="sxs-lookup"><span data-stu-id="67f19-167">The type of message.</span></span> <span data-ttu-id="67f19-168">Возможные значения: `message`.</span><span class="sxs-lookup"><span data-stu-id="67f19-168">The possible values are: `message`, , .</span></span>|
|<span data-ttu-id="67f19-169">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="67f19-169">createdDateTime</span></span>|<span data-ttu-id="67f19-170">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67f19-170">dateTimeOffset</span></span>|<span data-ttu-id="67f19-171">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="67f19-171">Read only.</span></span> <span data-ttu-id="67f19-172">Метка времени создания сообщения.</span><span class="sxs-lookup"><span data-stu-id="67f19-172">Timestamp of when the message was created.</span></span>|
|<span data-ttu-id="67f19-173">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="67f19-173">lastModifiedDateTime</span></span>|<span data-ttu-id="67f19-174">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67f19-174">dateTimeOffset</span></span>|<span data-ttu-id="67f19-175">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="67f19-175">Read only.</span></span> <span data-ttu-id="67f19-176">Метка времени изменения или обновления сообщения.</span><span class="sxs-lookup"><span data-stu-id="67f19-176">Timestamp of when the message was edited/updated.</span></span>|
|<span data-ttu-id="67f19-177">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="67f19-177">deletedDateTime</span></span>|<span data-ttu-id="67f19-178">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67f19-178">dateTimeOffset</span></span>|<span data-ttu-id="67f19-179">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="67f19-179">Read only.</span></span> <span data-ttu-id="67f19-180">Метка времени, в которое сообщение было удалено, или значение null, если сообщение не было удалено.</span><span class="sxs-lookup"><span data-stu-id="67f19-180">Timestamp at which the message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="67f19-181">subject</span><span class="sxs-lookup"><span data-stu-id="67f19-181">subject</span></span>|<span data-ttu-id="67f19-182">string</span><span class="sxs-lookup"><span data-stu-id="67f19-182">string</span></span>| <span data-ttu-id="67f19-183">Тема сообщения в формате обычного текста.</span><span class="sxs-lookup"><span data-stu-id="67f19-183">The subject of the message, in plaintext.</span></span>|
|<span data-ttu-id="67f19-184">body</span><span class="sxs-lookup"><span data-stu-id="67f19-184">body</span></span>|[<span data-ttu-id="67f19-185">itemBody</span><span class="sxs-lookup"><span data-stu-id="67f19-185">itemBody</span></span>](itembody.md)|<span data-ttu-id="67f19-186">Представление содержимого сообщения в формате Plaintext/HTML.</span><span class="sxs-lookup"><span data-stu-id="67f19-186">Plaintext/HTML representation of the content of the message.</span></span> <span data-ttu-id="67f19-187">Представление определяется параметром contentType в тексте.</span><span class="sxs-lookup"><span data-stu-id="67f19-187">Representation is specified by the contentType inside the body.</span></span> <span data-ttu-id="67f19-188">Содержимое всегда имеет формат HTML, если сообщение содержит [chatMessageMention](chatmessagemention.md).</span><span class="sxs-lookup"><span data-stu-id="67f19-188">The content is always in HTML if the message contains a [chatMessageMention](chatmessagemention.md).</span></span> |
|<span data-ttu-id="67f19-189">summary</span><span class="sxs-lookup"><span data-stu-id="67f19-189">summary</span></span>|<span data-ttu-id="67f19-190">string</span><span class="sxs-lookup"><span data-stu-id="67f19-190">string</span></span>| <span data-ttu-id="67f19-191">Сводный текст сообщения, который можно использовать для push-уведомлений и представлений сводки или резервных представлений.</span><span class="sxs-lookup"><span data-stu-id="67f19-191">Summary text of the message that could be used for push notifications and summary views or fall back views.</span></span> <span data-ttu-id="67f19-192">Относится только к сообщениям каналов, не к сообщениям чата.</span><span class="sxs-lookup"><span data-stu-id="67f19-192">Only applies to channel messages, not chat messages.</span></span> |
|<span data-ttu-id="67f19-193">attachments</span><span class="sxs-lookup"><span data-stu-id="67f19-193">attachments</span></span>|<span data-ttu-id="67f19-194">Коллекция [chatMessageAttachment](chatmessageattachment.md)</span><span class="sxs-lookup"><span data-stu-id="67f19-194">[chatMessageAttachment](chatmessageattachment.md) collection</span></span> |<span data-ttu-id="67f19-195">Вложенные файлы.</span><span class="sxs-lookup"><span data-stu-id="67f19-195">Attached files.</span></span> <span data-ttu-id="67f19-196">В настоящее время вложения доступны только для чтения. Отправка вложений не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67f19-196">Attachments are currently read-only – sending attachments is not supported.</span></span> |
|<span data-ttu-id="67f19-197">mentions</span><span class="sxs-lookup"><span data-stu-id="67f19-197">mentions</span></span>|<span data-ttu-id="67f19-198">Коллекция [chatMessageMention](chatmessagemention.md)</span><span class="sxs-lookup"><span data-stu-id="67f19-198">[chatMessageMention](chatmessagemention.md) collection</span></span>| <span data-ttu-id="67f19-199">Список сущностей, упомянутых в сообщении.</span><span class="sxs-lookup"><span data-stu-id="67f19-199">List of entities mentioned in the message.</span></span> <span data-ttu-id="67f19-200">В настоящее время поддерживаются значения user, bot, team и channel.</span><span class="sxs-lookup"><span data-stu-id="67f19-200">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="67f19-201">importance</span><span class="sxs-lookup"><span data-stu-id="67f19-201">importance</span></span>| <span data-ttu-id="67f19-202">chatMessageImportance</span><span class="sxs-lookup"><span data-stu-id="67f19-202">chatMessageImportance</span></span> | <span data-ttu-id="67f19-203">Важность сообщения.</span><span class="sxs-lookup"><span data-stu-id="67f19-203">The importance of the message.</span></span> <span data-ttu-id="67f19-204">Допустимые значения: `normal`, `high`, `urgent`.</span><span class="sxs-lookup"><span data-stu-id="67f19-204">The possible values are: `normal`, `high`, `urgent`.</span></span>|
|<span data-ttu-id="67f19-205">reactions</span><span class="sxs-lookup"><span data-stu-id="67f19-205">reactions</span></span>| <span data-ttu-id="67f19-206">Коллекция [chatMessageReaction](chatmessagereaction.md)</span><span class="sxs-lookup"><span data-stu-id="67f19-206">[chatMessageReaction](chatmessagereaction.md) collection</span></span> | <span data-ttu-id="67f19-207">Реакции на сообщение (например, "Нравится").</span><span class="sxs-lookup"><span data-stu-id="67f19-207">Reactions for this message (for example, Like).</span></span>|
|<span data-ttu-id="67f19-208">языковые стандарты</span><span class="sxs-lookup"><span data-stu-id="67f19-208">locale</span></span>|<span data-ttu-id="67f19-209">string</span><span class="sxs-lookup"><span data-stu-id="67f19-209">string</span></span>|<span data-ttu-id="67f19-210">Язык сообщения, установленный клиентом.</span><span class="sxs-lookup"><span data-stu-id="67f19-210">Locale of the message set by the client.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="67f19-211">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="67f19-211">JSON representation</span></span>

<span data-ttu-id="67f19-212">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="67f19-212">The following is a JSON representation of the resource.</span></span>

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
