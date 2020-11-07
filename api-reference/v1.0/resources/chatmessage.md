---
title: Тип ресурса chatMessage
description: Представляет отдельное сообщение чата в объекте channel или chat. Сообщение чата может быть корневым сообщением чата или частью потока, определенного свойством **реплитоид** в сообщении чата.
doc_type: resourcePageType
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 16bcd870ba8d4b97b5951fefab538eb6b6669635
ms.sourcegitcommit: 22d99624036ceaeb1b612538d5196faaa743881f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2020
ms.locfileid: "48932579"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="d00c1-104">Тип ресурса chatMessage</span><span class="sxs-lookup"><span data-stu-id="d00c1-104">chatMessage resource type</span></span>

<span data-ttu-id="d00c1-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d00c1-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d00c1-106">Представляет отдельное сообщение чата в [беседе](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true)по [каналу](./channel.md) или (в бета-версии).</span><span class="sxs-lookup"><span data-stu-id="d00c1-106">Represents an individual chat message within a [channel](./channel.md) or (in beta) [chat](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true).</span></span> <span data-ttu-id="d00c1-107">Сообщение чата может быть корневым сообщением чата или частью ответа, которое определяется свойством **реплитоид** в сообщении чата.</span><span class="sxs-lookup"><span data-stu-id="d00c1-107">The chat message can be a root chat message or part of a reply thread that is defined by the **replyToId** property in the chat message.</span></span>

## <a name="methods"></a><span data-ttu-id="d00c1-108">Методы</span><span class="sxs-lookup"><span data-stu-id="d00c1-108">Methods</span></span>

| <span data-ttu-id="d00c1-109">Метод</span><span class="sxs-lookup"><span data-stu-id="d00c1-109">Method</span></span>       | <span data-ttu-id="d00c1-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d00c1-110">Return Type</span></span>  |<span data-ttu-id="d00c1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d00c1-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d00c1-112">**Сообщения канала**</span><span class="sxs-lookup"><span data-stu-id="d00c1-112">**Channel messages**</span></span>| | |
|[<span data-ttu-id="d00c1-113">Список chatMessage Channel</span><span class="sxs-lookup"><span data-stu-id="d00c1-113">List channel chatMessage</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="d00c1-114">Коллекция [chatMessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="d00c1-114">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="d00c1-115">Список всех корневых сообщений чата в канале.</span><span class="sxs-lookup"><span data-stu-id="d00c1-115">List of all root chat messages in a channel.</span></span>|
|[<span data-ttu-id="d00c1-116">Получение chatMessages в разностном канале</span><span class="sxs-lookup"><span data-stu-id="d00c1-116">Get chatMessages in a channel delta</span></span>](../api/chatmessage-delta.md)  | [<span data-ttu-id="d00c1-117">chatMessage</span><span class="sxs-lookup"><span data-stu-id="d00c1-117">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="d00c1-118">Получение добавочных сообщений чата в канале.</span><span class="sxs-lookup"><span data-stu-id="d00c1-118">Get incremental chat messages in a channel.</span></span> |
|[<span data-ttu-id="d00c1-119">Создание подписки для сообщений о новых каналах</span><span class="sxs-lookup"><span data-stu-id="d00c1-119">Create subscription for new channel messages</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="d00c1-120">subscription</span><span class="sxs-lookup"><span data-stu-id="d00c1-120">subscription</span></span>](subscription.md) | <span data-ttu-id="d00c1-121">Прослушивать новые и измененные сообщения каналов и реакции на них.</span><span class="sxs-lookup"><span data-stu-id="d00c1-121">Listen for new and edited channel messages, and reactions to them.</span></span> |
|[<span data-ttu-id="d00c1-122">Получение chatMessage Channel</span><span class="sxs-lookup"><span data-stu-id="d00c1-122">Get channel chatMessage</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="d00c1-123">chatMessage</span><span class="sxs-lookup"><span data-stu-id="d00c1-123">chatMessage</span></span>](chatmessage.md) | <span data-ttu-id="d00c1-124">Получение одного из каналов сообщения с одним корневым сеансом.</span><span class="sxs-lookup"><span data-stu-id="d00c1-124">Get a single root chat message from a channel.</span></span>|
|[<span data-ttu-id="d00c1-125">Создание объекта chatMessage в канале</span><span class="sxs-lookup"><span data-stu-id="d00c1-125">Create chatMessage in a channel</span></span>](../api/channel-post-message.md) | [<span data-ttu-id="d00c1-126">chatMessage</span><span class="sxs-lookup"><span data-stu-id="d00c1-126">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="d00c1-127">Отправка сообщения в канал.</span><span class="sxs-lookup"><span data-stu-id="d00c1-127">Send a message to a channel.</span></span> |
|[<span data-ttu-id="d00c1-128">Обновление chatMessage</span><span class="sxs-lookup"><span data-stu-id="d00c1-128">Update chatMessage</span></span>](../api/chatmessage-update.md)|[<span data-ttu-id="d00c1-129">chatMessage</span><span class="sxs-lookup"><span data-stu-id="d00c1-129">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="d00c1-130">Обновление свойства **полицивиолатион** сообщения чата.</span><span class="sxs-lookup"><span data-stu-id="d00c1-130">Update the **policyViolation** property of a chat message.</span></span>|
|<span data-ttu-id="d00c1-131">**Ответы на сообщения канала**</span><span class="sxs-lookup"><span data-stu-id="d00c1-131">**Channel message replies**</span></span>| | |
|[<span data-ttu-id="d00c1-132">Перечисление ответов на chatMessage</span><span class="sxs-lookup"><span data-stu-id="d00c1-132">List replies to a chatMessage</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="d00c1-133">Коллекция [chatMessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="d00c1-133">[chatMessage](chatmessage.md) collection</span></span>| <span data-ttu-id="d00c1-134">Список всех ответов на сообщение чата в канале.</span><span class="sxs-lookup"><span data-stu-id="d00c1-134">List of all replies to a chat message in channel.</span></span>|
|[<span data-ttu-id="d00c1-135">Получение ответа на chatMessage</span><span class="sxs-lookup"><span data-stu-id="d00c1-135">Get a reply to a chatMessage</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="d00c1-136">chatMessage</span><span class="sxs-lookup"><span data-stu-id="d00c1-136">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="d00c1-137">Получение одного ответа на сообщение чата в канале.</span><span class="sxs-lookup"><span data-stu-id="d00c1-137">Get a single reply to a chat message in a channel.</span></span>|
|[<span data-ttu-id="d00c1-138">Ответ на chatMessage в канале</span><span class="sxs-lookup"><span data-stu-id="d00c1-138">Reply to a chatMessage in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="d00c1-139">chatMessage</span><span class="sxs-lookup"><span data-stu-id="d00c1-139">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="d00c1-140">Ответ на существующее сообщение чата в канале.</span><span class="sxs-lookup"><span data-stu-id="d00c1-140">Reply to an existing chat message in a channel.</span></span>|
|[<span data-ttu-id="d00c1-141">Обновление chatMessage</span><span class="sxs-lookup"><span data-stu-id="d00c1-141">Update chatMessage</span></span>](../api/chatmessage-update.md)|[<span data-ttu-id="d00c1-142">chatMessage</span><span class="sxs-lookup"><span data-stu-id="d00c1-142">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="d00c1-143">Обновление свойства **полицивиолатион** сообщения чата.</span><span class="sxs-lookup"><span data-stu-id="d00c1-143">Update the **policyViolation** property of a chat message.</span></span>|

## <a name="properties"></a><span data-ttu-id="d00c1-144">Свойства</span><span class="sxs-lookup"><span data-stu-id="d00c1-144">Properties</span></span>

| <span data-ttu-id="d00c1-145">Свойство</span><span class="sxs-lookup"><span data-stu-id="d00c1-145">Property</span></span>   | <span data-ttu-id="d00c1-146">Тип</span><span class="sxs-lookup"><span data-stu-id="d00c1-146">Type</span></span> |<span data-ttu-id="d00c1-147">Описание</span><span class="sxs-lookup"><span data-stu-id="d00c1-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d00c1-148">id</span><span class="sxs-lookup"><span data-stu-id="d00c1-148">id</span></span>|<span data-ttu-id="d00c1-149">String</span><span class="sxs-lookup"><span data-stu-id="d00c1-149">String</span></span>| <span data-ttu-id="d00c1-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d00c1-150">Read-only.</span></span> <span data-ttu-id="d00c1-151">Уникальный идентификатор сообщения.</span><span class="sxs-lookup"><span data-stu-id="d00c1-151">Unique Id of the message.</span></span>|
|<span data-ttu-id="d00c1-152">replyToId</span><span class="sxs-lookup"><span data-stu-id="d00c1-152">replyToId</span></span>| <span data-ttu-id="d00c1-153">string</span><span class="sxs-lookup"><span data-stu-id="d00c1-153">string</span></span> | <span data-ttu-id="d00c1-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d00c1-154">Read-only.</span></span> <span data-ttu-id="d00c1-155">Идентификатор родительского сообщения чата или сообщения корневого сеанса беседы в цепочке.</span><span class="sxs-lookup"><span data-stu-id="d00c1-155">Id of the parent chat message or root chat message of the thread.</span></span> <span data-ttu-id="d00c1-156">(Применяется только к сообщениям чата в каналах без чатов)</span><span class="sxs-lookup"><span data-stu-id="d00c1-156">(Only applies to chat messages in channels not chats)</span></span> |
|<span data-ttu-id="d00c1-157">from</span><span class="sxs-lookup"><span data-stu-id="d00c1-157">from</span></span>|[<span data-ttu-id="d00c1-158">identitySet</span><span class="sxs-lookup"><span data-stu-id="d00c1-158">identitySet</span></span>](identityset.md)| <span data-ttu-id="d00c1-159">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d00c1-159">Read only.</span></span> <span data-ttu-id="d00c1-160">Сведения об отправителе сообщения чата.</span><span class="sxs-lookup"><span data-stu-id="d00c1-160">Details of the sender of the chat message.</span></span>|
|<span data-ttu-id="d00c1-161">etag</span><span class="sxs-lookup"><span data-stu-id="d00c1-161">etag</span></span>| <span data-ttu-id="d00c1-162">string</span><span class="sxs-lookup"><span data-stu-id="d00c1-162">string</span></span> | <span data-ttu-id="d00c1-163">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d00c1-163">Read-only.</span></span> <span data-ttu-id="d00c1-164">Номер версии сообщения чата.</span><span class="sxs-lookup"><span data-stu-id="d00c1-164">Version number of the chat message.</span></span> |
|<span data-ttu-id="d00c1-165">messageType</span><span class="sxs-lookup"><span data-stu-id="d00c1-165">messageType</span></span>|<span data-ttu-id="d00c1-166">string</span><span class="sxs-lookup"><span data-stu-id="d00c1-166">string</span></span>|<span data-ttu-id="d00c1-167">Тип сообщения чата.</span><span class="sxs-lookup"><span data-stu-id="d00c1-167">The type of chat message.</span></span> <span data-ttu-id="d00c1-168">Возможные значения: `message` .</span><span class="sxs-lookup"><span data-stu-id="d00c1-168">The possible values are: `message`.</span></span>|
|<span data-ttu-id="d00c1-169">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d00c1-169">createdDateTime</span></span>|<span data-ttu-id="d00c1-170">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d00c1-170">dateTimeOffset</span></span>|<span data-ttu-id="d00c1-171">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d00c1-171">Read only.</span></span> <span data-ttu-id="d00c1-172">Метка времени создания сообщения чата.</span><span class="sxs-lookup"><span data-stu-id="d00c1-172">Timestamp of when the chat message was created.</span></span>|
|<span data-ttu-id="d00c1-173">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d00c1-173">lastModifiedDateTime</span></span>|<span data-ttu-id="d00c1-174">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d00c1-174">dateTimeOffset</span></span>|<span data-ttu-id="d00c1-175">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d00c1-175">Read only.</span></span> <span data-ttu-id="d00c1-176">Временная метка при создании сообщения чата (первоначальный параметр) или редактировании, в том числе при добавлении или удалении реакции.</span><span class="sxs-lookup"><span data-stu-id="d00c1-176">Timestamp when the chat message is created (initial setting) or edited, including when a reaction is added or removed.</span></span> |
|<span data-ttu-id="d00c1-177">ластедитеддатетиме</span><span class="sxs-lookup"><span data-stu-id="d00c1-177">lastEditedDateTime</span></span>|<span data-ttu-id="d00c1-178">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d00c1-178">dateTimeOffset</span></span>|<span data-ttu-id="d00c1-179">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d00c1-179">Read only.</span></span> <span data-ttu-id="d00c1-180">Временная метка при внесении изменений в сообщение чата.</span><span class="sxs-lookup"><span data-stu-id="d00c1-180">Timestamp when edits to the chat message were made.</span></span> <span data-ttu-id="d00c1-181">Запускает в пользовательском интерфейсе Microsoft Teams флаг "отредактирован".</span><span class="sxs-lookup"><span data-stu-id="d00c1-181">Triggers an "Edited" flag in the Microsoft Teams UI.</span></span> <span data-ttu-id="d00c1-182">Если не выполняется никаких изменений, значение — `null` .</span><span class="sxs-lookup"><span data-stu-id="d00c1-182">If no edits are made the value is `null`.</span></span>|
|<span data-ttu-id="d00c1-183">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="d00c1-183">deletedDateTime</span></span>|<span data-ttu-id="d00c1-184">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d00c1-184">dateTimeOffset</span></span>|<span data-ttu-id="d00c1-185">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d00c1-185">Read only.</span></span> <span data-ttu-id="d00c1-186">Временная метка, в которой сообщение чата удалено, или значение null, если оно не удалено.</span><span class="sxs-lookup"><span data-stu-id="d00c1-186">Timestamp at which the chat message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="d00c1-187">subject</span><span class="sxs-lookup"><span data-stu-id="d00c1-187">subject</span></span>|<span data-ttu-id="d00c1-188">string</span><span class="sxs-lookup"><span data-stu-id="d00c1-188">string</span></span>| <span data-ttu-id="d00c1-189">Тема сообщения чата в виде открытого текста.</span><span class="sxs-lookup"><span data-stu-id="d00c1-189">The subject of the chat message, in plaintext.</span></span>|
|<span data-ttu-id="d00c1-190">body</span><span class="sxs-lookup"><span data-stu-id="d00c1-190">body</span></span>|[<span data-ttu-id="d00c1-191">itemBody</span><span class="sxs-lookup"><span data-stu-id="d00c1-191">itemBody</span></span>](itembody.md)|<span data-ttu-id="d00c1-192">Представление содержимого сообщения чата в формате обычного текста или в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="d00c1-192">Plaintext/HTML representation of the content of the chat message.</span></span> <span data-ttu-id="d00c1-193">Представление определяется параметром contentType в тексте.</span><span class="sxs-lookup"><span data-stu-id="d00c1-193">Representation is specified by the contentType inside the body.</span></span> <span data-ttu-id="d00c1-194">Если сообщение чата содержит [чатмессажементион](chatmessagemention.md), содержимое всегда находится в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="d00c1-194">The content is always in HTML if the chat message contains a [chatMessageMention](chatmessagemention.md).</span></span> |
|<span data-ttu-id="d00c1-195">summary</span><span class="sxs-lookup"><span data-stu-id="d00c1-195">summary</span></span>|<span data-ttu-id="d00c1-196">string</span><span class="sxs-lookup"><span data-stu-id="d00c1-196">string</span></span>| <span data-ttu-id="d00c1-197">Сводный текст сообщения чата, которое можно использовать для push-уведомлений и сводных представлений, а также для обратного просмотра.</span><span class="sxs-lookup"><span data-stu-id="d00c1-197">Summary text of the chat message that could be used for push notifications and summary views or fall back views.</span></span> <span data-ttu-id="d00c1-198">Применяется только к сообщениям разговора по каналу, а не к сообщениям в чате.</span><span class="sxs-lookup"><span data-stu-id="d00c1-198">Only applies to channel chat messages, not chat messages in a chat.</span></span> |
|<span data-ttu-id="d00c1-199">attachments</span><span class="sxs-lookup"><span data-stu-id="d00c1-199">attachments</span></span>|<span data-ttu-id="d00c1-200">Коллекция [chatMessageAttachment](chatmessageattachment.md)</span><span class="sxs-lookup"><span data-stu-id="d00c1-200">[chatMessageAttachment](chatmessageattachment.md) collection</span></span> |<span data-ttu-id="d00c1-201">Вложенные файлы.</span><span class="sxs-lookup"><span data-stu-id="d00c1-201">Attached files.</span></span> <span data-ttu-id="d00c1-202">В настоящее время вложения доступны только для чтения. Отправка вложений не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d00c1-202">Attachments are currently read-only – sending attachments is not supported.</span></span> |
|<span data-ttu-id="d00c1-203">mentions</span><span class="sxs-lookup"><span data-stu-id="d00c1-203">mentions</span></span>|<span data-ttu-id="d00c1-204">Коллекция [chatMessageMention](chatmessagemention.md)</span><span class="sxs-lookup"><span data-stu-id="d00c1-204">[chatMessageMention](chatmessagemention.md) collection</span></span>| <span data-ttu-id="d00c1-205">Список сущностей, упоминаемых в сообщении чата.</span><span class="sxs-lookup"><span data-stu-id="d00c1-205">List of entities mentioned in the chat message.</span></span> <span data-ttu-id="d00c1-206">В настоящее время поддерживаются значения user, bot, team и channel.</span><span class="sxs-lookup"><span data-stu-id="d00c1-206">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="d00c1-207">importance</span><span class="sxs-lookup"><span data-stu-id="d00c1-207">importance</span></span>| <span data-ttu-id="d00c1-208">string</span><span class="sxs-lookup"><span data-stu-id="d00c1-208">string</span></span> | <span data-ttu-id="d00c1-209">Важность сообщения чата.</span><span class="sxs-lookup"><span data-stu-id="d00c1-209">The importance of the chat message.</span></span> <span data-ttu-id="d00c1-210">Допустимые значения: `normal`, `high`, `urgent`.</span><span class="sxs-lookup"><span data-stu-id="d00c1-210">The possible values are: `normal`, `high`, `urgent`.</span></span>|
| <span data-ttu-id="d00c1-211">полицивиолатион</span><span class="sxs-lookup"><span data-stu-id="d00c1-211">policyViolation</span></span> | [<span data-ttu-id="d00c1-212">чатмессажеполицивиолатион</span><span class="sxs-lookup"><span data-stu-id="d00c1-212">chatMessagePolicyViolation</span></span>](../resources/chatmessagepolicyviolation.md) |<span data-ttu-id="d00c1-213">Определяет свойства нарушения политики, заданные с помощью приложения предотвращения потери данных (DLP).</span><span class="sxs-lookup"><span data-stu-id="d00c1-213">Defines the properties of a policy violation set by a data loss prevention (DLP) application.</span></span>|
|<span data-ttu-id="d00c1-214">языковые стандарты</span><span class="sxs-lookup"><span data-stu-id="d00c1-214">locale</span></span>|<span data-ttu-id="d00c1-215">string</span><span class="sxs-lookup"><span data-stu-id="d00c1-215">string</span></span>|<span data-ttu-id="d00c1-216">Язык сообщения чата, заданное клиентом.</span><span class="sxs-lookup"><span data-stu-id="d00c1-216">Locale of the chat message set by the client.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d00c1-217">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d00c1-217">JSON representation</span></span>

<span data-ttu-id="d00c1-218">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d00c1-218">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "deleted",
    "deletedDateTime",
    "attachments",
    "importance",
    "mentions",
    "subject",
    "summary",
    "policyViolation",
    "locale"
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
  "policyViolation": {"@odata.type": "microsoft.graph.chatMessagePolicyViolation"},
  "locale": "string"
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
