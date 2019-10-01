---
title: Тип ресурса chatMessage
description: Представляет отдельное сообщение чата в объекте channel или chat. Сообщение чата может быть корневым сообщением чата или частью потока, определенного свойством **реплитоид** в сообщении чата.
doc_type: resourcePageType
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: 0d11230402d95009e414c16962a2eb9b5dce1f58
ms.sourcegitcommit: 2fb178ae78b5ecc47207d2b19d0c5a46e07e0960
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2019
ms.locfileid: "37333372"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="8aea9-104">Тип ресурса chatMessage</span><span class="sxs-lookup"><span data-stu-id="8aea9-104">chatMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8aea9-105">Представляет отдельное сообщение чата в [канале](channel.md) или [чате](chat.md).</span><span class="sxs-lookup"><span data-stu-id="8aea9-105">Represents an individual chat message within a [channel](channel.md) or [chat](chat.md).</span></span> <span data-ttu-id="8aea9-106">Сообщение чата может быть корневым сообщением чата или частью ответа, которое определяется свойством **реплитоид** в сообщении чата.</span><span class="sxs-lookup"><span data-stu-id="8aea9-106">The chat message can be a root chat message or part of a reply thread that is defined by the **replyToId** property in the chat message.</span></span>

## <a name="methods"></a><span data-ttu-id="8aea9-107">Методы</span><span class="sxs-lookup"><span data-stu-id="8aea9-107">Methods</span></span>

| <span data-ttu-id="8aea9-108">Метод</span><span class="sxs-lookup"><span data-stu-id="8aea9-108">Method</span></span>       | <span data-ttu-id="8aea9-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8aea9-109">Return Type</span></span>  |<span data-ttu-id="8aea9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8aea9-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8aea9-111">Список chatMessage Channel</span><span class="sxs-lookup"><span data-stu-id="8aea9-111">List channel chatMessage</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="8aea9-112">Коллекция [chatMessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="8aea9-112">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="8aea9-113">Список всех корневых сообщений чата в канале.</span><span class="sxs-lookup"><span data-stu-id="8aea9-113">List of all root chat messages in a channel.</span></span>|
|[<span data-ttu-id="8aea9-114">Получение chatMessages в разностном канале</span><span class="sxs-lookup"><span data-stu-id="8aea9-114">Get chatMessages in a channel delta</span></span>](../api/chatmessage-delta.md)  | [<span data-ttu-id="8aea9-115">chatMessage</span><span class="sxs-lookup"><span data-stu-id="8aea9-115">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="8aea9-116">Получение добавочных сообщений чата в канале.</span><span class="sxs-lookup"><span data-stu-id="8aea9-116">Get incremental chat messages in a channel.</span></span> |
|[<span data-ttu-id="8aea9-117">Получение chatMessage Channel</span><span class="sxs-lookup"><span data-stu-id="8aea9-117">Get channel chatMessage</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="8aea9-118">chatMessage</span><span class="sxs-lookup"><span data-stu-id="8aea9-118">chatMessage</span></span>](chatmessage.md) | <span data-ttu-id="8aea9-119">Получение одного из каналов сообщения с одним корневым сеансом.</span><span class="sxs-lookup"><span data-stu-id="8aea9-119">Get a single root chat message from a channel.</span></span>|
|[<span data-ttu-id="8aea9-120">Перечисление ответов на chatMessage</span><span class="sxs-lookup"><span data-stu-id="8aea9-120">List replies to a chatMessage</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="8aea9-121">Коллекция [chatMessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="8aea9-121">[chatMessage](chatmessage.md) collection</span></span>| <span data-ttu-id="8aea9-122">Список всех ответов на сообщение чата в канале.</span><span class="sxs-lookup"><span data-stu-id="8aea9-122">List of all replies to a chat message in channel.</span></span>|
|[<span data-ttu-id="8aea9-123">Получение ответа на chatMessage</span><span class="sxs-lookup"><span data-stu-id="8aea9-123">Get a reply to a chatMessage</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="8aea9-124">chatMessage</span><span class="sxs-lookup"><span data-stu-id="8aea9-124">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="8aea9-125">Получение одного ответа на сообщение чата в канале.</span><span class="sxs-lookup"><span data-stu-id="8aea9-125">Get a single reply to a chat message in a channel.</span></span>|
|[<span data-ttu-id="8aea9-126">Создание chatMessage в канале</span><span class="sxs-lookup"><span data-stu-id="8aea9-126">Create chatMessage in a channel</span></span>](../api/channel-post-messages.md) | [<span data-ttu-id="8aea9-127">chatMessage</span><span class="sxs-lookup"><span data-stu-id="8aea9-127">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="8aea9-128">Создайте новое сообщение разговора верхнего уровня в канале.</span><span class="sxs-lookup"><span data-stu-id="8aea9-128">Create a new top-level chat message in a channel.</span></span>|
|[<span data-ttu-id="8aea9-129">Ответ на chatMessage в канале</span><span class="sxs-lookup"><span data-stu-id="8aea9-129">Reply to a chatMessage in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="8aea9-130">chatMessage</span><span class="sxs-lookup"><span data-stu-id="8aea9-130">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="8aea9-131">Ответ на существующее сообщение чата в канале.</span><span class="sxs-lookup"><span data-stu-id="8aea9-131">Reply to an existing chat message in a channel.</span></span>|
|[<span data-ttu-id="8aea9-132">Создание chatMessage в чате</span><span class="sxs-lookup"><span data-stu-id="8aea9-132">Create chatMessage in a chat</span></span>](../api/chat-post-messages.md) | [<span data-ttu-id="8aea9-133">chatMessage</span><span class="sxs-lookup"><span data-stu-id="8aea9-133">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="8aea9-134">Отправка сообщения чата в существующей беседе 1:1 или группе чата.</span><span class="sxs-lookup"><span data-stu-id="8aea9-134">Send a chat message in an existing 1:1 or group chat conversation.</span></span>|
|[<span data-ttu-id="8aea9-135">Перечисление chatMessages в чате</span><span class="sxs-lookup"><span data-stu-id="8aea9-135">List chatMessages in a chat</span></span>](../api/chatmessage-list.md)  | [<span data-ttu-id="8aea9-136">chatMessage</span><span class="sxs-lookup"><span data-stu-id="8aea9-136">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="8aea9-137">Перечисление сообщений чата в 1:1 или группе чата.</span><span class="sxs-lookup"><span data-stu-id="8aea9-137">List chat messages in a 1:1 or group chat.</span></span> |
|[<span data-ttu-id="8aea9-138">Получение chatMessage в чате</span><span class="sxs-lookup"><span data-stu-id="8aea9-138">Get chatMessage in chat</span></span>](../api/chatmessage-get.md)  | [<span data-ttu-id="8aea9-139">chatMessage</span><span class="sxs-lookup"><span data-stu-id="8aea9-139">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="8aea9-140">Получение одного сообщения чата в чате.</span><span class="sxs-lookup"><span data-stu-id="8aea9-140">Get a single chat message in a chat.</span></span> |
|[<span data-ttu-id="8aea9-141">Перечисление всех размещенных контента</span><span class="sxs-lookup"><span data-stu-id="8aea9-141">List all hosted content</span></span>](../api/chatmessage-list-chatmessagehostedcontents.md) | <span data-ttu-id="8aea9-142">Коллекция [чатмессажехостедконтент](../resources/chatmessagehostedcontent.md)</span><span class="sxs-lookup"><span data-stu-id="8aea9-142">[chatMessageHostedContent](../resources/chatmessagehostedcontent.md) collection</span></span>| <span data-ttu-id="8aea9-143">Получение всего размещенного содержимого в сообщении чата.</span><span class="sxs-lookup"><span data-stu-id="8aea9-143">Get all hosted content in a chat message.</span></span>|
|[<span data-ttu-id="8aea9-144">Получение размещенного контента</span><span class="sxs-lookup"><span data-stu-id="8aea9-144">Get hosted content</span></span>](../api/chatmessagehostedcontent-get.md) | [<span data-ttu-id="8aea9-145">чатмессажехостедконтент</span><span class="sxs-lookup"><span data-stu-id="8aea9-145">chatMessageHostedContent</span></span>](../resources/chatmessagehostedcontent.md) | <span data-ttu-id="8aea9-146">Получение размещенного контента из сообщения чата.</span><span class="sxs-lookup"><span data-stu-id="8aea9-146">Get hosted content from a chat message.</span></span>|

## <a name="properties"></a><span data-ttu-id="8aea9-147">Свойства</span><span class="sxs-lookup"><span data-stu-id="8aea9-147">Properties</span></span>

| <span data-ttu-id="8aea9-148">Свойство</span><span class="sxs-lookup"><span data-stu-id="8aea9-148">Property</span></span>   | <span data-ttu-id="8aea9-149">Тип</span><span class="sxs-lookup"><span data-stu-id="8aea9-149">Type</span></span> |<span data-ttu-id="8aea9-150">Описание</span><span class="sxs-lookup"><span data-stu-id="8aea9-150">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8aea9-151">id</span><span class="sxs-lookup"><span data-stu-id="8aea9-151">id</span></span>|<span data-ttu-id="8aea9-152">String</span><span class="sxs-lookup"><span data-stu-id="8aea9-152">String</span></span>| <span data-ttu-id="8aea9-153">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8aea9-153">Read-only.</span></span> <span data-ttu-id="8aea9-154">Уникальный идентификатор сообщения.</span><span class="sxs-lookup"><span data-stu-id="8aea9-154">Unique Id of the message.</span></span>|
|<span data-ttu-id="8aea9-155">replyToId</span><span class="sxs-lookup"><span data-stu-id="8aea9-155">replyToId</span></span>| <span data-ttu-id="8aea9-156">string</span><span class="sxs-lookup"><span data-stu-id="8aea9-156">string</span></span> | <span data-ttu-id="8aea9-157">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8aea9-157">Read-only.</span></span> <span data-ttu-id="8aea9-158">Идентификатор родительского сообщения чата или сообщения корневого сеанса беседы в цепочке.</span><span class="sxs-lookup"><span data-stu-id="8aea9-158">Id of the parent chat message or root chat message of the thread.</span></span> <span data-ttu-id="8aea9-159">(Применяется только к сообщениям чата в каналах без чатов)</span><span class="sxs-lookup"><span data-stu-id="8aea9-159">(Only applies to chat messages in channels not chats)</span></span> |
|<span data-ttu-id="8aea9-160">from</span><span class="sxs-lookup"><span data-stu-id="8aea9-160">from</span></span>|[<span data-ttu-id="8aea9-161">identitySet</span><span class="sxs-lookup"><span data-stu-id="8aea9-161">identitySet</span></span>](identityset.md)| <span data-ttu-id="8aea9-162">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8aea9-162">Read only.</span></span> <span data-ttu-id="8aea9-163">Сведения об отправителе сообщения чата.</span><span class="sxs-lookup"><span data-stu-id="8aea9-163">Details of the sender of the chat message.</span></span>|
|<span data-ttu-id="8aea9-164">etag</span><span class="sxs-lookup"><span data-stu-id="8aea9-164">etag</span></span>| <span data-ttu-id="8aea9-165">string</span><span class="sxs-lookup"><span data-stu-id="8aea9-165">string</span></span> | <span data-ttu-id="8aea9-166">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8aea9-166">Read-only.</span></span> <span data-ttu-id="8aea9-167">Номер версии сообщения чата.</span><span class="sxs-lookup"><span data-stu-id="8aea9-167">Version number of the chat message.</span></span> |
|<span data-ttu-id="8aea9-168">messageType</span><span class="sxs-lookup"><span data-stu-id="8aea9-168">messageType</span></span>|<span data-ttu-id="8aea9-169">чатмессажетипе</span><span class="sxs-lookup"><span data-stu-id="8aea9-169">chatMessageType</span></span>|<span data-ttu-id="8aea9-170">Тип сообщения чата.</span><span class="sxs-lookup"><span data-stu-id="8aea9-170">The type of chat message.</span></span> <span data-ttu-id="8aea9-171">Возможные значения: `message`.</span><span class="sxs-lookup"><span data-stu-id="8aea9-171">The possible values are: `message`.</span></span>|
|<span data-ttu-id="8aea9-172">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8aea9-172">createdDateTime</span></span>|<span data-ttu-id="8aea9-173">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8aea9-173">dateTimeOffset</span></span>|<span data-ttu-id="8aea9-174">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8aea9-174">Read only.</span></span> <span data-ttu-id="8aea9-175">Метка времени создания сообщения чата.</span><span class="sxs-lookup"><span data-stu-id="8aea9-175">Timestamp of when the chat message was created.</span></span>|
|<span data-ttu-id="8aea9-176">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8aea9-176">lastModifiedDateTime</span></span>|<span data-ttu-id="8aea9-177">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8aea9-177">dateTimeOffset</span></span>|<span data-ttu-id="8aea9-178">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8aea9-178">Read only.</span></span> <span data-ttu-id="8aea9-179">Метка времени создания или изменения сообщения чата, в том числе когда выполняется ответ (если он является корневым сообщением в канале) или добавляется или удаляется реакция.</span><span class="sxs-lookup"><span data-stu-id="8aea9-179">Timestamp of when the chat message is created or edited, including when a reply is made (if it's a root chat message in a channel) or a reaction is added or removed.</span></span> |
|<span data-ttu-id="8aea9-180">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="8aea9-180">deletedDateTime</span></span>|<span data-ttu-id="8aea9-181">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8aea9-181">dateTimeOffset</span></span>|<span data-ttu-id="8aea9-182">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8aea9-182">Read only.</span></span> <span data-ttu-id="8aea9-183">Временная метка, в которой сообщение чата удалено, или значение null, если оно не удалено.</span><span class="sxs-lookup"><span data-stu-id="8aea9-183">Timestamp at which the chat message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="8aea9-184">subject</span><span class="sxs-lookup"><span data-stu-id="8aea9-184">subject</span></span>|<span data-ttu-id="8aea9-185">string</span><span class="sxs-lookup"><span data-stu-id="8aea9-185">string</span></span>| <span data-ttu-id="8aea9-186">Тема сообщения чата в виде открытого текста.</span><span class="sxs-lookup"><span data-stu-id="8aea9-186">The subject of the chat message, in plaintext.</span></span>|
|<span data-ttu-id="8aea9-187">body</span><span class="sxs-lookup"><span data-stu-id="8aea9-187">body</span></span>|[<span data-ttu-id="8aea9-188">itemBody</span><span class="sxs-lookup"><span data-stu-id="8aea9-188">itemBody</span></span>](itembody.md)|<span data-ttu-id="8aea9-189">Представление содержимого сообщения чата в формате обычного текста или в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="8aea9-189">Plaintext/HTML representation of the content of the chat message.</span></span> <span data-ttu-id="8aea9-190">Представление определяется параметром contentType в тексте.</span><span class="sxs-lookup"><span data-stu-id="8aea9-190">Representation is specified by the contentType inside the body.</span></span> <span data-ttu-id="8aea9-191">Если сообщение чата содержит [чатмессажементион](chatmessagemention.md), содержимое всегда находится в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="8aea9-191">The content is always in HTML if the chat message contains a [chatMessageMention](chatmessagemention.md).</span></span> |
|<span data-ttu-id="8aea9-192">summary</span><span class="sxs-lookup"><span data-stu-id="8aea9-192">summary</span></span>|<span data-ttu-id="8aea9-193">string</span><span class="sxs-lookup"><span data-stu-id="8aea9-193">string</span></span>| <span data-ttu-id="8aea9-194">Сводный текст сообщения чата, которое можно использовать для push-уведомлений и сводных представлений, а также для обратного просмотра.</span><span class="sxs-lookup"><span data-stu-id="8aea9-194">Summary text of the chat message that could be used for push notifications and summary views or fall back views.</span></span> <span data-ttu-id="8aea9-195">Применяется только к сообщениям разговора по каналу, а не к сообщениям в чате.</span><span class="sxs-lookup"><span data-stu-id="8aea9-195">Only applies to channel chat messages, not chat messages in a chat.</span></span> |
|<span data-ttu-id="8aea9-196">attachments</span><span class="sxs-lookup"><span data-stu-id="8aea9-196">attachments</span></span>|<span data-ttu-id="8aea9-197">Коллекция [chatMessageAttachment](chatmessageattachment.md)</span><span class="sxs-lookup"><span data-stu-id="8aea9-197">[chatMessageAttachment](chatmessageattachment.md) collection</span></span> |<span data-ttu-id="8aea9-198">Вложенные файлы.</span><span class="sxs-lookup"><span data-stu-id="8aea9-198">Attached files.</span></span> <span data-ttu-id="8aea9-199">В настоящее время вложения доступны только для чтения. Отправка вложений не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8aea9-199">Attachments are currently read-only – sending attachments is not supported.</span></span> |
|<span data-ttu-id="8aea9-200">mentions</span><span class="sxs-lookup"><span data-stu-id="8aea9-200">mentions</span></span>|<span data-ttu-id="8aea9-201">Коллекция [chatMessageMention](chatmessagemention.md)</span><span class="sxs-lookup"><span data-stu-id="8aea9-201">[chatMessageMention](chatmessagemention.md) collection</span></span>| <span data-ttu-id="8aea9-202">Список сущностей, упоминаемых в сообщении чата.</span><span class="sxs-lookup"><span data-stu-id="8aea9-202">List of entities mentioned in the chat message.</span></span> <span data-ttu-id="8aea9-203">В настоящее время поддерживаются значения user, bot, team и channel.</span><span class="sxs-lookup"><span data-stu-id="8aea9-203">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="8aea9-204">importance</span><span class="sxs-lookup"><span data-stu-id="8aea9-204">importance</span></span>| <span data-ttu-id="8aea9-205">чатмессажеимпортанце</span><span class="sxs-lookup"><span data-stu-id="8aea9-205">chatMessageImportance</span></span> | <span data-ttu-id="8aea9-206">Важность сообщения чата.</span><span class="sxs-lookup"><span data-stu-id="8aea9-206">The importance of the chat message.</span></span> <span data-ttu-id="8aea9-207">Допустимые значения: `normal`, `high`, `urgent`.</span><span class="sxs-lookup"><span data-stu-id="8aea9-207">The possible values are: `normal`, `high`, `urgent`.</span></span>|
|<span data-ttu-id="8aea9-208">reactions</span><span class="sxs-lookup"><span data-stu-id="8aea9-208">reactions</span></span>| <span data-ttu-id="8aea9-209">Коллекция [chatMessageReaction](chatmessagereaction.md)</span><span class="sxs-lookup"><span data-stu-id="8aea9-209">[chatMessageReaction](chatmessagereaction.md) collection</span></span> | <span data-ttu-id="8aea9-210">Реакции на это сообщение чата (например, например).</span><span class="sxs-lookup"><span data-stu-id="8aea9-210">Reactions for this chat message (for example, Like).</span></span>|
|<span data-ttu-id="8aea9-211">языковые стандарты</span><span class="sxs-lookup"><span data-stu-id="8aea9-211">locale</span></span>|<span data-ttu-id="8aea9-212">string</span><span class="sxs-lookup"><span data-stu-id="8aea9-212">string</span></span>|<span data-ttu-id="8aea9-213">Язык сообщения чата, заданное клиентом.</span><span class="sxs-lookup"><span data-stu-id="8aea9-213">Locale of the chat message set by the client.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8aea9-214">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8aea9-214">JSON representation</span></span>

<span data-ttu-id="8aea9-215">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8aea9-215">The following is a JSON representation of the resource.</span></span>

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
