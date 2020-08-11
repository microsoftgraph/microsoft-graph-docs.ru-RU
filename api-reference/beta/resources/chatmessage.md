---
title: Тип ресурса chatMessage
description: Представляет отдельное сообщение чата в объекте channel или chat. Сообщение чата может быть корневым сообщением чата или частью потока, определенного свойством **реплитоид** в сообщении чата.
doc_type: resourcePageType
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: 49f80dec9931c73bc42862cb682c1600fd39a4fe
ms.sourcegitcommit: ab36e03d6bcb5327102214eb078d55709579d465
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2020
ms.locfileid: "46630300"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="230cb-104">Тип ресурса chatMessage</span><span class="sxs-lookup"><span data-stu-id="230cb-104">chatMessage resource type</span></span>

<span data-ttu-id="230cb-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="230cb-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="230cb-106">Представляет отдельное сообщение чата в [канале](channel.md) или [чате](chat.md).</span><span class="sxs-lookup"><span data-stu-id="230cb-106">Represents an individual chat message within a [channel](channel.md) or [chat](chat.md).</span></span> <span data-ttu-id="230cb-107">Сообщение чата может быть корневым сообщением чата или частью ответа, которое определяется свойством **реплитоид** в сообщении чата.</span><span class="sxs-lookup"><span data-stu-id="230cb-107">The chat message can be a root chat message or part of a reply thread that is defined by the **replyToId** property in the chat message.</span></span>

## <a name="methods"></a><span data-ttu-id="230cb-108">Методы</span><span class="sxs-lookup"><span data-stu-id="230cb-108">Methods</span></span>

| <span data-ttu-id="230cb-109">Метод</span><span class="sxs-lookup"><span data-stu-id="230cb-109">Method</span></span>       | <span data-ttu-id="230cb-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="230cb-110">Return Type</span></span>  |<span data-ttu-id="230cb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="230cb-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="230cb-112">**Сообщения канала**</span><span class="sxs-lookup"><span data-stu-id="230cb-112">**Channel messages**</span></span>| | |
|[<span data-ttu-id="230cb-113">Список chatMessage Channel</span><span class="sxs-lookup"><span data-stu-id="230cb-113">List channel chatMessage</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="230cb-114">Коллекция [chatMessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="230cb-114">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="230cb-115">Список всех корневых сообщений чата в канале.</span><span class="sxs-lookup"><span data-stu-id="230cb-115">List of all root chat messages in a channel.</span></span>|
|[<span data-ttu-id="230cb-116">Получение chatMessages в разностном канале</span><span class="sxs-lookup"><span data-stu-id="230cb-116">Get chatMessages in a channel delta</span></span>](../api/chatmessage-delta.md)  | [<span data-ttu-id="230cb-117">chatMessage</span><span class="sxs-lookup"><span data-stu-id="230cb-117">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="230cb-118">Получение добавочных сообщений чата в канале.</span><span class="sxs-lookup"><span data-stu-id="230cb-118">Get incremental chat messages in a channel.</span></span> |
|[<span data-ttu-id="230cb-119">Создание подписки для сообщений о новых каналах</span><span class="sxs-lookup"><span data-stu-id="230cb-119">Create subscription for new channel messages</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="230cb-120">subscription</span><span class="sxs-lookup"><span data-stu-id="230cb-120">subscription</span></span>](subscription.md) | <span data-ttu-id="230cb-121">Прослушивать новые и измененные сообщения каналов и реакции на них.</span><span class="sxs-lookup"><span data-stu-id="230cb-121">Listen for new and edited channel messages, and reactions to them.</span></span> |
|[<span data-ttu-id="230cb-122">Получение chatMessage Channel</span><span class="sxs-lookup"><span data-stu-id="230cb-122">Get channel chatMessage</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="230cb-123">chatMessage</span><span class="sxs-lookup"><span data-stu-id="230cb-123">chatMessage</span></span>](chatmessage.md) | <span data-ttu-id="230cb-124">Получение одного из каналов сообщения с одним корневым сеансом.</span><span class="sxs-lookup"><span data-stu-id="230cb-124">Get a single root chat message from a channel.</span></span>|
|[<span data-ttu-id="230cb-125">Создание chatMessage в канале или чате</span><span class="sxs-lookup"><span data-stu-id="230cb-125">Create chatMessage in a channel or chat</span></span>](../api/chatmessage-post.md) | [<span data-ttu-id="230cb-126">chatMessage</span><span class="sxs-lookup"><span data-stu-id="230cb-126">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="230cb-127">Создайте новое сообщение разговора верхнего уровня в канале.</span><span class="sxs-lookup"><span data-stu-id="230cb-127">Create a new top-level chat message in a channel.</span></span>|
|<span data-ttu-id="230cb-128">**Ответы на сообщения канала**</span><span class="sxs-lookup"><span data-stu-id="230cb-128">**Channel message replies**</span></span>| | |
|[<span data-ttu-id="230cb-129">Перечисление ответов на chatMessage</span><span class="sxs-lookup"><span data-stu-id="230cb-129">List replies to a chatMessage</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="230cb-130">Коллекция [chatMessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="230cb-130">[chatMessage](chatmessage.md) collection</span></span>| <span data-ttu-id="230cb-131">Список всех ответов на сообщение чата в канале.</span><span class="sxs-lookup"><span data-stu-id="230cb-131">List of all replies to a chat message in channel.</span></span>|
|[<span data-ttu-id="230cb-132">Получение ответа на chatMessage</span><span class="sxs-lookup"><span data-stu-id="230cb-132">Get a reply to a chatMessage</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="230cb-133">chatMessage</span><span class="sxs-lookup"><span data-stu-id="230cb-133">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="230cb-134">Получение одного ответа на сообщение чата в канале.</span><span class="sxs-lookup"><span data-stu-id="230cb-134">Get a single reply to a chat message in a channel.</span></span>|
|[<span data-ttu-id="230cb-135">Ответ на chatMessage в канале</span><span class="sxs-lookup"><span data-stu-id="230cb-135">Reply to a chatMessage in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="230cb-136">chatMessage</span><span class="sxs-lookup"><span data-stu-id="230cb-136">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="230cb-137">Ответ на существующее сообщение чата в канале.</span><span class="sxs-lookup"><span data-stu-id="230cb-137">Reply to an existing chat message in a channel.</span></span>|
|<span data-ttu-id="230cb-138">**1:1 и сообщения группового чата**</span><span class="sxs-lookup"><span data-stu-id="230cb-138">**1:1 and group chat messages**</span></span>| | |
|[<span data-ttu-id="230cb-139">Создание chatMessage в чате</span><span class="sxs-lookup"><span data-stu-id="230cb-139">Create chatMessage in a chat</span></span>](../api/chat-post-message.md) | [<span data-ttu-id="230cb-140">chatMessage</span><span class="sxs-lookup"><span data-stu-id="230cb-140">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="230cb-141">Отправка сообщения чата в существующей беседе 1:1 или группе чата.</span><span class="sxs-lookup"><span data-stu-id="230cb-141">Send a chat message in an existing 1:1 or group chat conversation.</span></span>|
|[<span data-ttu-id="230cb-142">Перечисление chatMessages в чате</span><span class="sxs-lookup"><span data-stu-id="230cb-142">List chatMessages in a chat</span></span>](../api/chat-list-message.md)  | [<span data-ttu-id="230cb-143">chatMessage</span><span class="sxs-lookup"><span data-stu-id="230cb-143">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="230cb-144">Перечисление сообщений чата в 1:1 или группе чата.</span><span class="sxs-lookup"><span data-stu-id="230cb-144">List chat messages in a 1:1 or group chat.</span></span> |
|[<span data-ttu-id="230cb-145">Создание подписки для новых сообщений чата</span><span class="sxs-lookup"><span data-stu-id="230cb-145">Create subscription for new chat messages</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="230cb-146">subscription</span><span class="sxs-lookup"><span data-stu-id="230cb-146">subscription</span></span>](subscription.md) | <span data-ttu-id="230cb-147">Прослушивание новых и измененных сообщений чата и реакции на них.</span><span class="sxs-lookup"><span data-stu-id="230cb-147">Listen for new and edited chat messages, and reactions to them.</span></span> |
|[<span data-ttu-id="230cb-148">Получение chatMessage в чате</span><span class="sxs-lookup"><span data-stu-id="230cb-148">Get chatMessage in chat</span></span>](../api/chat-get-message.md)  | [<span data-ttu-id="230cb-149">chatMessage</span><span class="sxs-lookup"><span data-stu-id="230cb-149">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="230cb-150">Получение одного сообщения чата в чате.</span><span class="sxs-lookup"><span data-stu-id="230cb-150">Get a single chat message in a chat.</span></span> |
|<span data-ttu-id="230cb-151">**Размещенный контент**</span><span class="sxs-lookup"><span data-stu-id="230cb-151">**Hosted content**</span></span>| | |
|[<span data-ttu-id="230cb-152">Перечисление всех размещенных контента</span><span class="sxs-lookup"><span data-stu-id="230cb-152">List all hosted content</span></span>](../api/chatmessage-list-chatmessagehostedcontents.md) | <span data-ttu-id="230cb-153">Коллекция [чатмессажехостедконтент](../resources/chatmessagehostedcontent.md)</span><span class="sxs-lookup"><span data-stu-id="230cb-153">[chatMessageHostedContent](../resources/chatmessagehostedcontent.md) collection</span></span>| <span data-ttu-id="230cb-154">Получение всего размещенного содержимого в сообщении чата.</span><span class="sxs-lookup"><span data-stu-id="230cb-154">Get all hosted content in a chat message.</span></span>|
|[<span data-ttu-id="230cb-155">Получение размещенного контента</span><span class="sxs-lookup"><span data-stu-id="230cb-155">Get hosted content</span></span>](../api/chatmessagehostedcontent-get.md) | [<span data-ttu-id="230cb-156">чатмессажехостедконтент</span><span class="sxs-lookup"><span data-stu-id="230cb-156">chatMessageHostedContent</span></span>](../resources/chatmessagehostedcontent.md) | <span data-ttu-id="230cb-157">Получение размещенного контента из сообщения чата.</span><span class="sxs-lookup"><span data-stu-id="230cb-157">Get hosted content from a chat message.</span></span>|

## <a name="properties"></a><span data-ttu-id="230cb-158">Свойства</span><span class="sxs-lookup"><span data-stu-id="230cb-158">Properties</span></span>

| <span data-ttu-id="230cb-159">Свойство</span><span class="sxs-lookup"><span data-stu-id="230cb-159">Property</span></span>   | <span data-ttu-id="230cb-160">Тип</span><span class="sxs-lookup"><span data-stu-id="230cb-160">Type</span></span> |<span data-ttu-id="230cb-161">Описание</span><span class="sxs-lookup"><span data-stu-id="230cb-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="230cb-162">id</span><span class="sxs-lookup"><span data-stu-id="230cb-162">id</span></span>|<span data-ttu-id="230cb-163">String</span><span class="sxs-lookup"><span data-stu-id="230cb-163">String</span></span>| <span data-ttu-id="230cb-164">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="230cb-164">Read-only.</span></span> <span data-ttu-id="230cb-165">Уникальный идентификатор сообщения.</span><span class="sxs-lookup"><span data-stu-id="230cb-165">Unique Id of the message.</span></span>|
|<span data-ttu-id="230cb-166">replyToId</span><span class="sxs-lookup"><span data-stu-id="230cb-166">replyToId</span></span>| <span data-ttu-id="230cb-167">string</span><span class="sxs-lookup"><span data-stu-id="230cb-167">string</span></span> | <span data-ttu-id="230cb-168">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="230cb-168">Read-only.</span></span> <span data-ttu-id="230cb-169">Идентификатор родительского сообщения чата или сообщения корневого сеанса беседы в цепочке.</span><span class="sxs-lookup"><span data-stu-id="230cb-169">Id of the parent chat message or root chat message of the thread.</span></span> <span data-ttu-id="230cb-170">(Применяется только к сообщениям чата в каналах без чатов)</span><span class="sxs-lookup"><span data-stu-id="230cb-170">(Only applies to chat messages in channels not chats)</span></span> |
|<span data-ttu-id="230cb-171">from</span><span class="sxs-lookup"><span data-stu-id="230cb-171">from</span></span>|[<span data-ttu-id="230cb-172">identitySet</span><span class="sxs-lookup"><span data-stu-id="230cb-172">identitySet</span></span>](identityset.md)| <span data-ttu-id="230cb-173">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="230cb-173">Read only.</span></span> <span data-ttu-id="230cb-174">Сведения об отправителе сообщения чата.</span><span class="sxs-lookup"><span data-stu-id="230cb-174">Details of the sender of the chat message.</span></span>|
|<span data-ttu-id="230cb-175">etag</span><span class="sxs-lookup"><span data-stu-id="230cb-175">etag</span></span>| <span data-ttu-id="230cb-176">string</span><span class="sxs-lookup"><span data-stu-id="230cb-176">string</span></span> | <span data-ttu-id="230cb-177">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="230cb-177">Read-only.</span></span> <span data-ttu-id="230cb-178">Номер версии сообщения чата.</span><span class="sxs-lookup"><span data-stu-id="230cb-178">Version number of the chat message.</span></span> |
|<span data-ttu-id="230cb-179">messageType</span><span class="sxs-lookup"><span data-stu-id="230cb-179">messageType</span></span>|<span data-ttu-id="230cb-180">string</span><span class="sxs-lookup"><span data-stu-id="230cb-180">string</span></span>|<span data-ttu-id="230cb-181">Тип сообщения чата.</span><span class="sxs-lookup"><span data-stu-id="230cb-181">The type of chat message.</span></span> <span data-ttu-id="230cb-182">Возможные значения: `message` .</span><span class="sxs-lookup"><span data-stu-id="230cb-182">The possible values are: `message`.</span></span>|
|<span data-ttu-id="230cb-183">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="230cb-183">createdDateTime</span></span>|<span data-ttu-id="230cb-184">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="230cb-184">dateTimeOffset</span></span>|<span data-ttu-id="230cb-185">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="230cb-185">Read only.</span></span> <span data-ttu-id="230cb-186">Метка времени создания сообщения чата.</span><span class="sxs-lookup"><span data-stu-id="230cb-186">Timestamp of when the chat message was created.</span></span>|
|<span data-ttu-id="230cb-187">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="230cb-187">lastModifiedDateTime</span></span>|<span data-ttu-id="230cb-188">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="230cb-188">dateTimeOffset</span></span>|<span data-ttu-id="230cb-189">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="230cb-189">Read only.</span></span> <span data-ttu-id="230cb-190">Метка времени создания или изменения сообщения чата, в том числе когда выполняется ответ (если он является корневым сообщением в канале) или добавляется или удаляется реакция.</span><span class="sxs-lookup"><span data-stu-id="230cb-190">Timestamp of when the chat message is created or edited, including when a reply is made (if it's a root chat message in a channel) or a reaction is added or removed.</span></span> |
|<span data-ttu-id="230cb-191">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="230cb-191">deletedDateTime</span></span>|<span data-ttu-id="230cb-192">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="230cb-192">dateTimeOffset</span></span>|<span data-ttu-id="230cb-193">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="230cb-193">Read only.</span></span> <span data-ttu-id="230cb-194">Временная метка, в которой сообщение чата удалено, или значение null, если оно не удалено.</span><span class="sxs-lookup"><span data-stu-id="230cb-194">Timestamp at which the chat message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="230cb-195">subject</span><span class="sxs-lookup"><span data-stu-id="230cb-195">subject</span></span>|<span data-ttu-id="230cb-196">string</span><span class="sxs-lookup"><span data-stu-id="230cb-196">string</span></span>| <span data-ttu-id="230cb-197">Тема сообщения чата в виде открытого текста.</span><span class="sxs-lookup"><span data-stu-id="230cb-197">The subject of the chat message, in plaintext.</span></span>|
|<span data-ttu-id="230cb-198">body</span><span class="sxs-lookup"><span data-stu-id="230cb-198">body</span></span>|[<span data-ttu-id="230cb-199">itemBody</span><span class="sxs-lookup"><span data-stu-id="230cb-199">itemBody</span></span>](itembody.md)|<span data-ttu-id="230cb-200">Представление содержимого сообщения чата в формате обычного текста или в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="230cb-200">Plaintext/HTML representation of the content of the chat message.</span></span> <span data-ttu-id="230cb-201">Представление определяется параметром contentType в тексте.</span><span class="sxs-lookup"><span data-stu-id="230cb-201">Representation is specified by the contentType inside the body.</span></span> <span data-ttu-id="230cb-202">Если сообщение чата содержит [чатмессажементион](chatmessagemention.md), содержимое всегда находится в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="230cb-202">The content is always in HTML if the chat message contains a [chatMessageMention](chatmessagemention.md).</span></span> |
|<span data-ttu-id="230cb-203">summary</span><span class="sxs-lookup"><span data-stu-id="230cb-203">summary</span></span>|<span data-ttu-id="230cb-204">string</span><span class="sxs-lookup"><span data-stu-id="230cb-204">string</span></span>| <span data-ttu-id="230cb-205">Сводный текст сообщения чата, которое можно использовать для push-уведомлений и сводных представлений, а также для обратного просмотра.</span><span class="sxs-lookup"><span data-stu-id="230cb-205">Summary text of the chat message that could be used for push notifications and summary views or fall back views.</span></span> <span data-ttu-id="230cb-206">Применяется только к сообщениям разговора по каналу, а не к сообщениям в чате.</span><span class="sxs-lookup"><span data-stu-id="230cb-206">Only applies to channel chat messages, not chat messages in a chat.</span></span> |
|<span data-ttu-id="230cb-207">attachments</span><span class="sxs-lookup"><span data-stu-id="230cb-207">attachments</span></span>|<span data-ttu-id="230cb-208">Коллекция [chatMessageAttachment](chatmessageattachment.md)</span><span class="sxs-lookup"><span data-stu-id="230cb-208">[chatMessageAttachment](chatmessageattachment.md) collection</span></span> |<span data-ttu-id="230cb-209">Вложенные файлы.</span><span class="sxs-lookup"><span data-stu-id="230cb-209">Attached files.</span></span> <span data-ttu-id="230cb-210">В настоящее время вложения доступны только для чтения. Отправка вложений не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="230cb-210">Attachments are currently read-only – sending attachments is not supported.</span></span> |
|<span data-ttu-id="230cb-211">mentions</span><span class="sxs-lookup"><span data-stu-id="230cb-211">mentions</span></span>|<span data-ttu-id="230cb-212">Коллекция [chatMessageMention](chatmessagemention.md)</span><span class="sxs-lookup"><span data-stu-id="230cb-212">[chatMessageMention](chatmessagemention.md) collection</span></span>| <span data-ttu-id="230cb-213">Список сущностей, упоминаемых в сообщении чата.</span><span class="sxs-lookup"><span data-stu-id="230cb-213">List of entities mentioned in the chat message.</span></span> <span data-ttu-id="230cb-214">В настоящее время поддерживаются значения user, bot, team и channel.</span><span class="sxs-lookup"><span data-stu-id="230cb-214">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="230cb-215">importance</span><span class="sxs-lookup"><span data-stu-id="230cb-215">importance</span></span>|<span data-ttu-id="230cb-216">string</span><span class="sxs-lookup"><span data-stu-id="230cb-216">string</span></span> | <span data-ttu-id="230cb-217">Важность сообщения чата.</span><span class="sxs-lookup"><span data-stu-id="230cb-217">The importance of the chat message.</span></span> <span data-ttu-id="230cb-218">Допустимые значения: `normal`, `high`, `urgent`.</span><span class="sxs-lookup"><span data-stu-id="230cb-218">The possible values are: `normal`, `high`, `urgent`.</span></span>|
|<span data-ttu-id="230cb-219">reactions</span><span class="sxs-lookup"><span data-stu-id="230cb-219">reactions</span></span>| <span data-ttu-id="230cb-220">Коллекция [chatMessageReaction](./chatmessagereaction.md)</span><span class="sxs-lookup"><span data-stu-id="230cb-220">[chatMessageReaction](./chatmessagereaction.md) collection</span></span> | <span data-ttu-id="230cb-221">Реакции на это сообщение чата (например, например).</span><span class="sxs-lookup"><span data-stu-id="230cb-221">Reactions for this chat message (for example, Like).</span></span>|
|<span data-ttu-id="230cb-222">языковые стандарты</span><span class="sxs-lookup"><span data-stu-id="230cb-222">locale</span></span>|<span data-ttu-id="230cb-223">string</span><span class="sxs-lookup"><span data-stu-id="230cb-223">string</span></span>|<span data-ttu-id="230cb-224">Язык сообщения чата, заданное клиентом.</span><span class="sxs-lookup"><span data-stu-id="230cb-224">Locale of the chat message set by the client.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="230cb-225">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="230cb-225">JSON representation</span></span>

<span data-ttu-id="230cb-226">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="230cb-226">The following is a JSON representation of the resource.</span></span>

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
  "reactions":  "string",
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
