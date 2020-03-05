---
title: Тип ресурса chatMessage
description: Представляет отдельное сообщение чата в объекте channel или chat. Сообщение чата может быть корневым сообщением чата или частью потока, определенного свойством **реплитоид** в сообщении чата.
doc_type: resourcePageType
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: 5443f88005f46a07353d6d24ed07bea11df7b30b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507721"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="311a0-104">Тип ресурса chatMessage</span><span class="sxs-lookup"><span data-stu-id="311a0-104">chatMessage resource type</span></span>

<span data-ttu-id="311a0-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="311a0-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="311a0-106">Представляет отдельное сообщение чата в [канале](channel.md) или [чате](chat.md).</span><span class="sxs-lookup"><span data-stu-id="311a0-106">Represents an individual chat message within a [channel](channel.md) or [chat](chat.md).</span></span> <span data-ttu-id="311a0-107">Сообщение чата может быть корневым сообщением чата или частью ответа, которое определяется свойством **реплитоид** в сообщении чата.</span><span class="sxs-lookup"><span data-stu-id="311a0-107">The chat message can be a root chat message or part of a reply thread that is defined by the **replyToId** property in the chat message.</span></span>

## <a name="methods"></a><span data-ttu-id="311a0-108">Методы</span><span class="sxs-lookup"><span data-stu-id="311a0-108">Methods</span></span>

| <span data-ttu-id="311a0-109">Метод</span><span class="sxs-lookup"><span data-stu-id="311a0-109">Method</span></span>       | <span data-ttu-id="311a0-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="311a0-110">Return Type</span></span>  |<span data-ttu-id="311a0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="311a0-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="311a0-112">**Сообщения канала**</span><span class="sxs-lookup"><span data-stu-id="311a0-112">**Channel messages**</span></span>| | |
|[<span data-ttu-id="311a0-113">Список chatMessage Channel</span><span class="sxs-lookup"><span data-stu-id="311a0-113">List channel chatMessage</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="311a0-114">Коллекция [chatMessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="311a0-114">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="311a0-115">Список всех корневых сообщений чата в канале.</span><span class="sxs-lookup"><span data-stu-id="311a0-115">List of all root chat messages in a channel.</span></span>|
|[<span data-ttu-id="311a0-116">Получение chatMessages в разностном канале</span><span class="sxs-lookup"><span data-stu-id="311a0-116">Get chatMessages in a channel delta</span></span>](../api/chatmessage-delta.md)  | [<span data-ttu-id="311a0-117">chatMessage</span><span class="sxs-lookup"><span data-stu-id="311a0-117">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="311a0-118">Получение добавочных сообщений чата в канале.</span><span class="sxs-lookup"><span data-stu-id="311a0-118">Get incremental chat messages in a channel.</span></span> |
|[<span data-ttu-id="311a0-119">Создание подписки для сообщений о новых каналах</span><span class="sxs-lookup"><span data-stu-id="311a0-119">Create subscription for new channel messages</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="311a0-120">subscription</span><span class="sxs-lookup"><span data-stu-id="311a0-120">subscription</span></span>](subscription.md) | <span data-ttu-id="311a0-121">Прослушивать новые и измененные сообщения каналов и реакции на них.</span><span class="sxs-lookup"><span data-stu-id="311a0-121">Listen for new and edited channel messages, and reactions to them.</span></span> |
|[<span data-ttu-id="311a0-122">Получение chatMessage Channel</span><span class="sxs-lookup"><span data-stu-id="311a0-122">Get channel chatMessage</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="311a0-123">chatMessage</span><span class="sxs-lookup"><span data-stu-id="311a0-123">chatMessage</span></span>](chatmessage.md) | <span data-ttu-id="311a0-124">Получение одного из каналов сообщения с одним корневым сеансом.</span><span class="sxs-lookup"><span data-stu-id="311a0-124">Get a single root chat message from a channel.</span></span>|
|[<span data-ttu-id="311a0-125">Создание объекта chatMessage в канале</span><span class="sxs-lookup"><span data-stu-id="311a0-125">Create chatMessage in a channel</span></span>](../api/channel-post-messages.md) | [<span data-ttu-id="311a0-126">chatMessage</span><span class="sxs-lookup"><span data-stu-id="311a0-126">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="311a0-127">Создайте новое сообщение разговора верхнего уровня в канале.</span><span class="sxs-lookup"><span data-stu-id="311a0-127">Create a new top-level chat message in a channel.</span></span>|
|<span data-ttu-id="311a0-128">**Ответы на сообщения канала**</span><span class="sxs-lookup"><span data-stu-id="311a0-128">**Channel message replies**</span></span>| | |
|[<span data-ttu-id="311a0-129">Перечисление ответов на chatMessage</span><span class="sxs-lookup"><span data-stu-id="311a0-129">List replies to a chatMessage</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="311a0-130">Коллекция [chatMessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="311a0-130">[chatMessage](chatmessage.md) collection</span></span>| <span data-ttu-id="311a0-131">Список всех ответов на сообщение чата в канале.</span><span class="sxs-lookup"><span data-stu-id="311a0-131">List of all replies to a chat message in channel.</span></span>|
|[<span data-ttu-id="311a0-132">Получение ответа на chatMessage</span><span class="sxs-lookup"><span data-stu-id="311a0-132">Get a reply to a chatMessage</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="311a0-133">chatMessage</span><span class="sxs-lookup"><span data-stu-id="311a0-133">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="311a0-134">Получение одного ответа на сообщение чата в канале.</span><span class="sxs-lookup"><span data-stu-id="311a0-134">Get a single reply to a chat message in a channel.</span></span>|
|[<span data-ttu-id="311a0-135">Ответ на chatMessage в канале</span><span class="sxs-lookup"><span data-stu-id="311a0-135">Reply to a chatMessage in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="311a0-136">chatMessage</span><span class="sxs-lookup"><span data-stu-id="311a0-136">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="311a0-137">Ответ на существующее сообщение чата в канале.</span><span class="sxs-lookup"><span data-stu-id="311a0-137">Reply to an existing chat message in a channel.</span></span>|
|<span data-ttu-id="311a0-138">**1:1 и сообщения группового чата**</span><span class="sxs-lookup"><span data-stu-id="311a0-138">**1:1 and group chat messages**</span></span>| | |
|[<span data-ttu-id="311a0-139">Создание chatMessage в чате</span><span class="sxs-lookup"><span data-stu-id="311a0-139">Create chatMessage in a chat</span></span>](../api/chat-post-messages.md) | [<span data-ttu-id="311a0-140">chatMessage</span><span class="sxs-lookup"><span data-stu-id="311a0-140">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="311a0-141">Отправка сообщения чата в существующей беседе 1:1 или группе чата.</span><span class="sxs-lookup"><span data-stu-id="311a0-141">Send a chat message in an existing 1:1 or group chat conversation.</span></span>|
|[<span data-ttu-id="311a0-142">Перечисление chatMessages в чате</span><span class="sxs-lookup"><span data-stu-id="311a0-142">List chatMessages in a chat</span></span>](../api/chatmessage-list.md)  | [<span data-ttu-id="311a0-143">chatMessage</span><span class="sxs-lookup"><span data-stu-id="311a0-143">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="311a0-144">Перечисление сообщений чата в 1:1 или группе чата.</span><span class="sxs-lookup"><span data-stu-id="311a0-144">List chat messages in a 1:1 or group chat.</span></span> |
|[<span data-ttu-id="311a0-145">Создание подписки для новых сообщений чата</span><span class="sxs-lookup"><span data-stu-id="311a0-145">Create subscription for new chat messages</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="311a0-146">subscription</span><span class="sxs-lookup"><span data-stu-id="311a0-146">subscription</span></span>](subscription.md) | <span data-ttu-id="311a0-147">Прослушивание новых и измененных сообщений чата и реакции на них.</span><span class="sxs-lookup"><span data-stu-id="311a0-147">Listen for new and edited chat messages, and reactions to them.</span></span> |
|[<span data-ttu-id="311a0-148">Получение chatMessage в чате</span><span class="sxs-lookup"><span data-stu-id="311a0-148">Get chatMessage in chat</span></span>](../api/chatmessage-get.md)  | [<span data-ttu-id="311a0-149">chatMessage</span><span class="sxs-lookup"><span data-stu-id="311a0-149">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="311a0-150">Получение одного сообщения чата в чате.</span><span class="sxs-lookup"><span data-stu-id="311a0-150">Get a single chat message in a chat.</span></span> |
|<span data-ttu-id="311a0-151">**Размещенный контент**</span><span class="sxs-lookup"><span data-stu-id="311a0-151">**Hosted content**</span></span>| | |
|[<span data-ttu-id="311a0-152">Перечисление всех размещенных контента</span><span class="sxs-lookup"><span data-stu-id="311a0-152">List all hosted content</span></span>](../api/chatmessage-list-chatmessagehostedcontents.md) | <span data-ttu-id="311a0-153">Коллекция [чатмессажехостедконтент](../resources/chatmessagehostedcontent.md)</span><span class="sxs-lookup"><span data-stu-id="311a0-153">[chatMessageHostedContent](../resources/chatmessagehostedcontent.md) collection</span></span>| <span data-ttu-id="311a0-154">Получение всего размещенного содержимого в сообщении чата.</span><span class="sxs-lookup"><span data-stu-id="311a0-154">Get all hosted content in a chat message.</span></span>|
|[<span data-ttu-id="311a0-155">Получение размещенного контента</span><span class="sxs-lookup"><span data-stu-id="311a0-155">Get hosted content</span></span>](../api/chatmessagehostedcontent-get.md) | [<span data-ttu-id="311a0-156">чатмессажехостедконтент</span><span class="sxs-lookup"><span data-stu-id="311a0-156">chatMessageHostedContent</span></span>](../resources/chatmessagehostedcontent.md) | <span data-ttu-id="311a0-157">Получение размещенного контента из сообщения чата.</span><span class="sxs-lookup"><span data-stu-id="311a0-157">Get hosted content from a chat message.</span></span>|

## <a name="properties"></a><span data-ttu-id="311a0-158">Свойства</span><span class="sxs-lookup"><span data-stu-id="311a0-158">Properties</span></span>

| <span data-ttu-id="311a0-159">Свойство</span><span class="sxs-lookup"><span data-stu-id="311a0-159">Property</span></span>   | <span data-ttu-id="311a0-160">Тип</span><span class="sxs-lookup"><span data-stu-id="311a0-160">Type</span></span> |<span data-ttu-id="311a0-161">Описание</span><span class="sxs-lookup"><span data-stu-id="311a0-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="311a0-162">id</span><span class="sxs-lookup"><span data-stu-id="311a0-162">id</span></span>|<span data-ttu-id="311a0-163">String</span><span class="sxs-lookup"><span data-stu-id="311a0-163">String</span></span>| <span data-ttu-id="311a0-164">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="311a0-164">Read-only.</span></span> <span data-ttu-id="311a0-165">Уникальный идентификатор сообщения.</span><span class="sxs-lookup"><span data-stu-id="311a0-165">Unique Id of the message.</span></span>|
|<span data-ttu-id="311a0-166">replyToId</span><span class="sxs-lookup"><span data-stu-id="311a0-166">replyToId</span></span>| <span data-ttu-id="311a0-167">string</span><span class="sxs-lookup"><span data-stu-id="311a0-167">string</span></span> | <span data-ttu-id="311a0-168">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="311a0-168">Read-only.</span></span> <span data-ttu-id="311a0-169">Идентификатор родительского сообщения чата или сообщения корневого сеанса беседы в цепочке.</span><span class="sxs-lookup"><span data-stu-id="311a0-169">Id of the parent chat message or root chat message of the thread.</span></span> <span data-ttu-id="311a0-170">(Применяется только к сообщениям чата в каналах без чатов)</span><span class="sxs-lookup"><span data-stu-id="311a0-170">(Only applies to chat messages in channels not chats)</span></span> |
|<span data-ttu-id="311a0-171">from</span><span class="sxs-lookup"><span data-stu-id="311a0-171">from</span></span>|[<span data-ttu-id="311a0-172">identitySet</span><span class="sxs-lookup"><span data-stu-id="311a0-172">identitySet</span></span>](identityset.md)| <span data-ttu-id="311a0-173">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="311a0-173">Read only.</span></span> <span data-ttu-id="311a0-174">Сведения об отправителе сообщения чата.</span><span class="sxs-lookup"><span data-stu-id="311a0-174">Details of the sender of the chat message.</span></span>|
|<span data-ttu-id="311a0-175">etag</span><span class="sxs-lookup"><span data-stu-id="311a0-175">etag</span></span>| <span data-ttu-id="311a0-176">string</span><span class="sxs-lookup"><span data-stu-id="311a0-176">string</span></span> | <span data-ttu-id="311a0-177">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="311a0-177">Read-only.</span></span> <span data-ttu-id="311a0-178">Номер версии сообщения чата.</span><span class="sxs-lookup"><span data-stu-id="311a0-178">Version number of the chat message.</span></span> |
|<span data-ttu-id="311a0-179">messageType</span><span class="sxs-lookup"><span data-stu-id="311a0-179">messageType</span></span>|<span data-ttu-id="311a0-180">чатмессажетипе</span><span class="sxs-lookup"><span data-stu-id="311a0-180">chatMessageType</span></span>|<span data-ttu-id="311a0-181">Тип сообщения чата.</span><span class="sxs-lookup"><span data-stu-id="311a0-181">The type of chat message.</span></span> <span data-ttu-id="311a0-182">Возможные значения: `message`.</span><span class="sxs-lookup"><span data-stu-id="311a0-182">The possible values are: `message`.</span></span>|
|<span data-ttu-id="311a0-183">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="311a0-183">createdDateTime</span></span>|<span data-ttu-id="311a0-184">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="311a0-184">dateTimeOffset</span></span>|<span data-ttu-id="311a0-185">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="311a0-185">Read only.</span></span> <span data-ttu-id="311a0-186">Метка времени создания сообщения чата.</span><span class="sxs-lookup"><span data-stu-id="311a0-186">Timestamp of when the chat message was created.</span></span>|
|<span data-ttu-id="311a0-187">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="311a0-187">lastModifiedDateTime</span></span>|<span data-ttu-id="311a0-188">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="311a0-188">dateTimeOffset</span></span>|<span data-ttu-id="311a0-189">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="311a0-189">Read only.</span></span> <span data-ttu-id="311a0-190">Метка времени создания или изменения сообщения чата, в том числе когда выполняется ответ (если он является корневым сообщением в канале) или добавляется или удаляется реакция.</span><span class="sxs-lookup"><span data-stu-id="311a0-190">Timestamp of when the chat message is created or edited, including when a reply is made (if it's a root chat message in a channel) or a reaction is added or removed.</span></span> |
|<span data-ttu-id="311a0-191">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="311a0-191">deletedDateTime</span></span>|<span data-ttu-id="311a0-192">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="311a0-192">dateTimeOffset</span></span>|<span data-ttu-id="311a0-193">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="311a0-193">Read only.</span></span> <span data-ttu-id="311a0-194">Временная метка, в которой сообщение чата удалено, или значение null, если оно не удалено.</span><span class="sxs-lookup"><span data-stu-id="311a0-194">Timestamp at which the chat message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="311a0-195">subject</span><span class="sxs-lookup"><span data-stu-id="311a0-195">subject</span></span>|<span data-ttu-id="311a0-196">string</span><span class="sxs-lookup"><span data-stu-id="311a0-196">string</span></span>| <span data-ttu-id="311a0-197">Тема сообщения чата в виде открытого текста.</span><span class="sxs-lookup"><span data-stu-id="311a0-197">The subject of the chat message, in plaintext.</span></span>|
|<span data-ttu-id="311a0-198">body</span><span class="sxs-lookup"><span data-stu-id="311a0-198">body</span></span>|[<span data-ttu-id="311a0-199">itemBody</span><span class="sxs-lookup"><span data-stu-id="311a0-199">itemBody</span></span>](itembody.md)|<span data-ttu-id="311a0-200">Представление содержимого сообщения чата в формате обычного текста или в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="311a0-200">Plaintext/HTML representation of the content of the chat message.</span></span> <span data-ttu-id="311a0-201">Представление определяется параметром contentType в тексте.</span><span class="sxs-lookup"><span data-stu-id="311a0-201">Representation is specified by the contentType inside the body.</span></span> <span data-ttu-id="311a0-202">Если сообщение чата содержит [чатмессажементион](chatmessagemention.md), содержимое всегда находится в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="311a0-202">The content is always in HTML if the chat message contains a [chatMessageMention](chatmessagemention.md).</span></span> |
|<span data-ttu-id="311a0-203">summary</span><span class="sxs-lookup"><span data-stu-id="311a0-203">summary</span></span>|<span data-ttu-id="311a0-204">string</span><span class="sxs-lookup"><span data-stu-id="311a0-204">string</span></span>| <span data-ttu-id="311a0-205">Сводный текст сообщения чата, которое можно использовать для push-уведомлений и сводных представлений, а также для обратного просмотра.</span><span class="sxs-lookup"><span data-stu-id="311a0-205">Summary text of the chat message that could be used for push notifications and summary views or fall back views.</span></span> <span data-ttu-id="311a0-206">Применяется только к сообщениям разговора по каналу, а не к сообщениям в чате.</span><span class="sxs-lookup"><span data-stu-id="311a0-206">Only applies to channel chat messages, not chat messages in a chat.</span></span> |
|<span data-ttu-id="311a0-207">attachments</span><span class="sxs-lookup"><span data-stu-id="311a0-207">attachments</span></span>|<span data-ttu-id="311a0-208">Коллекция [chatMessageAttachment](chatmessageattachment.md)</span><span class="sxs-lookup"><span data-stu-id="311a0-208">[chatMessageAttachment](chatmessageattachment.md) collection</span></span> |<span data-ttu-id="311a0-209">Вложенные файлы.</span><span class="sxs-lookup"><span data-stu-id="311a0-209">Attached files.</span></span> <span data-ttu-id="311a0-210">В настоящее время вложения доступны только для чтения. Отправка вложений не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="311a0-210">Attachments are currently read-only – sending attachments is not supported.</span></span> |
|<span data-ttu-id="311a0-211">mentions</span><span class="sxs-lookup"><span data-stu-id="311a0-211">mentions</span></span>|<span data-ttu-id="311a0-212">Коллекция [chatMessageMention](chatmessagemention.md)</span><span class="sxs-lookup"><span data-stu-id="311a0-212">[chatMessageMention](chatmessagemention.md) collection</span></span>| <span data-ttu-id="311a0-213">Список сущностей, упоминаемых в сообщении чата.</span><span class="sxs-lookup"><span data-stu-id="311a0-213">List of entities mentioned in the chat message.</span></span> <span data-ttu-id="311a0-214">В настоящее время поддерживаются значения user, bot, team и channel.</span><span class="sxs-lookup"><span data-stu-id="311a0-214">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="311a0-215">importance</span><span class="sxs-lookup"><span data-stu-id="311a0-215">importance</span></span>| <span data-ttu-id="311a0-216">чатмессажеимпортанце</span><span class="sxs-lookup"><span data-stu-id="311a0-216">chatMessageImportance</span></span> | <span data-ttu-id="311a0-217">Важность сообщения чата.</span><span class="sxs-lookup"><span data-stu-id="311a0-217">The importance of the chat message.</span></span> <span data-ttu-id="311a0-218">Допустимые значения: `normal`, `high`, `urgent`.</span><span class="sxs-lookup"><span data-stu-id="311a0-218">The possible values are: `normal`, `high`, `urgent`.</span></span>|
|<span data-ttu-id="311a0-219">reactions</span><span class="sxs-lookup"><span data-stu-id="311a0-219">reactions</span></span>| <span data-ttu-id="311a0-220">Коллекция [chatMessageReaction](chatmessagereaction.md)</span><span class="sxs-lookup"><span data-stu-id="311a0-220">[chatMessageReaction](chatmessagereaction.md) collection</span></span> | <span data-ttu-id="311a0-221">Реакции на это сообщение чата (например, например).</span><span class="sxs-lookup"><span data-stu-id="311a0-221">Reactions for this chat message (for example, Like).</span></span>|
|<span data-ttu-id="311a0-222">языковые стандарты</span><span class="sxs-lookup"><span data-stu-id="311a0-222">locale</span></span>|<span data-ttu-id="311a0-223">string</span><span class="sxs-lookup"><span data-stu-id="311a0-223">string</span></span>|<span data-ttu-id="311a0-224">Язык сообщения чата, заданное клиентом.</span><span class="sxs-lookup"><span data-stu-id="311a0-224">Locale of the chat message set by the client.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="311a0-225">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="311a0-225">JSON representation</span></span>

<span data-ttu-id="311a0-226">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="311a0-226">The following is a JSON representation of the resource.</span></span>

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
