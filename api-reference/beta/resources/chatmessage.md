---
title: Тип ресурса chatMessage
description: Представляет отдельное сообщение чата в объекте channel или chat. Сообщение чата может быть корневым сообщением чата или частью потока, определенного свойством **реплитоид** в сообщении чата.
doc_type: resourcePageType
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: a29afea30f0ea1d75f5c7ce1a0713976f10cc298
ms.sourcegitcommit: cca4f96414aededa03bb45e07e19bb20b7327563
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/30/2019
ms.locfileid: "36677123"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="fb53a-104">Тип ресурса chatMessage</span><span class="sxs-lookup"><span data-stu-id="fb53a-104">chatMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb53a-105">Представляет отдельное сообщение чата в [канале](channel.md) или [чате](chat.md).</span><span class="sxs-lookup"><span data-stu-id="fb53a-105">Represents an individual chat message within a [channel](channel.md) or [chat](chat.md).</span></span> <span data-ttu-id="fb53a-106">Сообщение чата может быть корневым сообщением чата или частью ответа, которое определяется свойством **реплитоид** в сообщении чата.</span><span class="sxs-lookup"><span data-stu-id="fb53a-106">The chat message can be a root chat message or part of a reply thread that is defined by the **replyToId** property in the chat message.</span></span>

## <a name="methods"></a><span data-ttu-id="fb53a-107">Методы</span><span class="sxs-lookup"><span data-stu-id="fb53a-107">Methods</span></span>

| <span data-ttu-id="fb53a-108">Метод</span><span class="sxs-lookup"><span data-stu-id="fb53a-108">Method</span></span>       | <span data-ttu-id="fb53a-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fb53a-109">Return Type</span></span>  |<span data-ttu-id="fb53a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="fb53a-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fb53a-111">Список chatMessage Channel</span><span class="sxs-lookup"><span data-stu-id="fb53a-111">List channel chatMessage</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="fb53a-112">Коллекция [chatMessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="fb53a-112">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="fb53a-113">Список всех корневых сообщений чата в канале.</span><span class="sxs-lookup"><span data-stu-id="fb53a-113">List of all root chat messages in a channel.</span></span>|
|[<span data-ttu-id="fb53a-114">Получение chatMessages в разностном канале</span><span class="sxs-lookup"><span data-stu-id="fb53a-114">Get chatMessages in a channel delta</span></span>](../api/chatmessage-delta.md)  | [<span data-ttu-id="fb53a-115">chatMessage</span><span class="sxs-lookup"><span data-stu-id="fb53a-115">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="fb53a-116">Получение добавочных сообщений чата в канале.</span><span class="sxs-lookup"><span data-stu-id="fb53a-116">Get incremental chat messages in a channel.</span></span> |
|[<span data-ttu-id="fb53a-117">Получение chatMessage Channel</span><span class="sxs-lookup"><span data-stu-id="fb53a-117">Get channel chatMessage</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="fb53a-118">chatMessage</span><span class="sxs-lookup"><span data-stu-id="fb53a-118">chatMessage</span></span>](chatmessage.md) | <span data-ttu-id="fb53a-119">Получение одного из каналов сообщения с одним корневым сеансом.</span><span class="sxs-lookup"><span data-stu-id="fb53a-119">Get a single root chat message from a channel.</span></span>|
|[<span data-ttu-id="fb53a-120">Перечисление ответов на chatMessage</span><span class="sxs-lookup"><span data-stu-id="fb53a-120">List replies to a chatMessage</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="fb53a-121">Коллекция [chatMessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="fb53a-121">[chatMessage](chatmessage.md) collection</span></span>| <span data-ttu-id="fb53a-122">Список всех ответов на сообщение чата в канале.</span><span class="sxs-lookup"><span data-stu-id="fb53a-122">List of all replies to a chat message in channel.</span></span>|
|[<span data-ttu-id="fb53a-123">Получение ответа на chatMessage</span><span class="sxs-lookup"><span data-stu-id="fb53a-123">Get a reply to a chatMessage</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="fb53a-124">chatMessage</span><span class="sxs-lookup"><span data-stu-id="fb53a-124">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="fb53a-125">Получение одного ответа на сообщение чата в канале.</span><span class="sxs-lookup"><span data-stu-id="fb53a-125">Get a single reply to a chat message in a channel.</span></span>|
|[<span data-ttu-id="fb53a-126">Создание chatMessage в канале</span><span class="sxs-lookup"><span data-stu-id="fb53a-126">Create chatMessage in a channel</span></span>](../api/channel-post-messages.md) | [<span data-ttu-id="fb53a-127">chatMessage</span><span class="sxs-lookup"><span data-stu-id="fb53a-127">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="fb53a-128">Создайте новое сообщение разговора верхнего уровня в канале.</span><span class="sxs-lookup"><span data-stu-id="fb53a-128">Create a new top-level chat message in a channel.</span></span>|
|[<span data-ttu-id="fb53a-129">Ответ на chatMessage в канале</span><span class="sxs-lookup"><span data-stu-id="fb53a-129">Reply to a chatMessage in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="fb53a-130">chatMessage</span><span class="sxs-lookup"><span data-stu-id="fb53a-130">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="fb53a-131">Ответ на существующее сообщение чата в канале.</span><span class="sxs-lookup"><span data-stu-id="fb53a-131">Reply to an existing chat message in a channel.</span></span>|
|[<span data-ttu-id="fb53a-132">Создание chatMessage в чате</span><span class="sxs-lookup"><span data-stu-id="fb53a-132">Create chatMessage in a chat</span></span>](../api/chat-post-messages.md) | [<span data-ttu-id="fb53a-133">chatMessage</span><span class="sxs-lookup"><span data-stu-id="fb53a-133">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="fb53a-134">Отправка сообщения чата в существующей беседе 1:1 или группе чата.</span><span class="sxs-lookup"><span data-stu-id="fb53a-134">Send a chat message in an existing 1:1 or group chat conversation.</span></span>|
|[<span data-ttu-id="fb53a-135">Перечисление chatMessages в чате</span><span class="sxs-lookup"><span data-stu-id="fb53a-135">List chatMessages in a chat</span></span>](../api/chatmessage-list.md)  | [<span data-ttu-id="fb53a-136">chatMessage</span><span class="sxs-lookup"><span data-stu-id="fb53a-136">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="fb53a-137">Перечисление сообщений чата в 1:1 или группе чата.</span><span class="sxs-lookup"><span data-stu-id="fb53a-137">List chat messages in a 1:1 or group chat.</span></span> |
|[<span data-ttu-id="fb53a-138">Получение chatMessage в чате</span><span class="sxs-lookup"><span data-stu-id="fb53a-138">Get chatMessage in chat</span></span>](../api/chatmessage-get.md)  | [<span data-ttu-id="fb53a-139">chatMessage</span><span class="sxs-lookup"><span data-stu-id="fb53a-139">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="fb53a-140">Получение одного сообщения чата в чате.</span><span class="sxs-lookup"><span data-stu-id="fb53a-140">Get a single chat message in a chat.</span></span> |
|[<span data-ttu-id="fb53a-141">Перечисление всех размещенных изображений</span><span class="sxs-lookup"><span data-stu-id="fb53a-141">List all hosted images</span></span>](../api/chatmessagehostedimage-list-hostedimages.md) | <span data-ttu-id="fb53a-142">Коллекция [хостедимаже](../resources/chatmessagehostedimage.md)</span><span class="sxs-lookup"><span data-stu-id="fb53a-142">[hostedImage](../resources/chatmessagehostedimage.md) collection</span></span>| <span data-ttu-id="fb53a-143">Получение всех размещенных изображений в сообщении чата.</span><span class="sxs-lookup"><span data-stu-id="fb53a-143">Get all hosted images in a chat message.</span></span>|
|[<span data-ttu-id="fb53a-144">Получение размещенного изображения</span><span class="sxs-lookup"><span data-stu-id="fb53a-144">Get hosted image</span></span>](../api/chatmessagehostedimage-get.md) | [<span data-ttu-id="fb53a-145">хостедимаже</span><span class="sxs-lookup"><span data-stu-id="fb53a-145">hostedImage</span></span>](../resources/chatmessagehostedimage.md) | <span data-ttu-id="fb53a-146">Получение размещенного изображения из сообщения чата.</span><span class="sxs-lookup"><span data-stu-id="fb53a-146">Get a hosted image from a chat message.</span></span>|
|[<span data-ttu-id="fb53a-147">Получение байтов размещенного изображения</span><span class="sxs-lookup"><span data-stu-id="fb53a-147">Get hosted image bytes</span></span>](../api/chatmessagehostedimage-getbytes.md) | <span data-ttu-id="fb53a-148">данные двоичных изображений</span><span class="sxs-lookup"><span data-stu-id="fb53a-148">binary image data</span></span> | <span data-ttu-id="fb53a-149">Получение двоичных данных изображения на размещенном изображении из сообщения чата.</span><span class="sxs-lookup"><span data-stu-id="fb53a-149">Get binary image data of a hosted image from a chat message.</span></span>|

## <a name="properties"></a><span data-ttu-id="fb53a-150">Свойства</span><span class="sxs-lookup"><span data-stu-id="fb53a-150">Properties</span></span>

| <span data-ttu-id="fb53a-151">Свойство</span><span class="sxs-lookup"><span data-stu-id="fb53a-151">Property</span></span>   | <span data-ttu-id="fb53a-152">Тип</span><span class="sxs-lookup"><span data-stu-id="fb53a-152">Type</span></span> |<span data-ttu-id="fb53a-153">Описание</span><span class="sxs-lookup"><span data-stu-id="fb53a-153">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fb53a-154">id</span><span class="sxs-lookup"><span data-stu-id="fb53a-154">id</span></span>|<span data-ttu-id="fb53a-155">String</span><span class="sxs-lookup"><span data-stu-id="fb53a-155">String</span></span>| <span data-ttu-id="fb53a-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fb53a-156">Read-only.</span></span> <span data-ttu-id="fb53a-157">Уникальный идентификатор сообщения.</span><span class="sxs-lookup"><span data-stu-id="fb53a-157">Unique Id of the message.</span></span>|
|<span data-ttu-id="fb53a-158">replyToId</span><span class="sxs-lookup"><span data-stu-id="fb53a-158">replyToId</span></span>| <span data-ttu-id="fb53a-159">string</span><span class="sxs-lookup"><span data-stu-id="fb53a-159">string</span></span> | <span data-ttu-id="fb53a-160">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fb53a-160">Read-only.</span></span> <span data-ttu-id="fb53a-161">Идентификатор родительского сообщения чата или сообщения корневого сеанса беседы в цепочке.</span><span class="sxs-lookup"><span data-stu-id="fb53a-161">Id of the parent chat message or root chat message of the thread.</span></span> <span data-ttu-id="fb53a-162">(Применяется только к сообщениям чата в каналах без чатов)</span><span class="sxs-lookup"><span data-stu-id="fb53a-162">(Only applies to chat messages in channels not chats)</span></span> |
|<span data-ttu-id="fb53a-163">from</span><span class="sxs-lookup"><span data-stu-id="fb53a-163">from</span></span>|[<span data-ttu-id="fb53a-164">identitySet</span><span class="sxs-lookup"><span data-stu-id="fb53a-164">identitySet</span></span>](identityset.md)| <span data-ttu-id="fb53a-165">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fb53a-165">Read only.</span></span> <span data-ttu-id="fb53a-166">Сведения об отправителе сообщения чата.</span><span class="sxs-lookup"><span data-stu-id="fb53a-166">Details of the sender of the chat message.</span></span>|
|<span data-ttu-id="fb53a-167">etag</span><span class="sxs-lookup"><span data-stu-id="fb53a-167">etag</span></span>| <span data-ttu-id="fb53a-168">string</span><span class="sxs-lookup"><span data-stu-id="fb53a-168">string</span></span> | <span data-ttu-id="fb53a-169">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fb53a-169">Read-only.</span></span> <span data-ttu-id="fb53a-170">Номер версии сообщения чата.</span><span class="sxs-lookup"><span data-stu-id="fb53a-170">Version number of the chat message.</span></span> |
|<span data-ttu-id="fb53a-171">messageType</span><span class="sxs-lookup"><span data-stu-id="fb53a-171">messageType</span></span>|<span data-ttu-id="fb53a-172">чатмессажетипе</span><span class="sxs-lookup"><span data-stu-id="fb53a-172">chatMessageType</span></span>|<span data-ttu-id="fb53a-173">Тип сообщения чата.</span><span class="sxs-lookup"><span data-stu-id="fb53a-173">The type of chat message.</span></span> <span data-ttu-id="fb53a-174">Возможные значения: `message`.</span><span class="sxs-lookup"><span data-stu-id="fb53a-174">The possible values are: `message`.</span></span>|
|<span data-ttu-id="fb53a-175">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fb53a-175">createdDateTime</span></span>|<span data-ttu-id="fb53a-176">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb53a-176">dateTimeOffset</span></span>|<span data-ttu-id="fb53a-177">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fb53a-177">Read only.</span></span> <span data-ttu-id="fb53a-178">Метка времени создания сообщения чата.</span><span class="sxs-lookup"><span data-stu-id="fb53a-178">Timestamp of when the chat message was created.</span></span>|
|<span data-ttu-id="fb53a-179">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fb53a-179">lastModifiedDateTime</span></span>|<span data-ttu-id="fb53a-180">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb53a-180">dateTimeOffset</span></span>|<span data-ttu-id="fb53a-181">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fb53a-181">Read only.</span></span> <span data-ttu-id="fb53a-182">Метка времени создания или изменения сообщения чата, в том числе когда выполняется ответ (если он является корневым сообщением в канале) или добавляется или удаляется реакция.</span><span class="sxs-lookup"><span data-stu-id="fb53a-182">Timestamp of when the chat message is created or edited, including when a reply is made (if it's a root chat message in a channel) or a reaction is added or removed.</span></span> |
|<span data-ttu-id="fb53a-183">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="fb53a-183">deletedDateTime</span></span>|<span data-ttu-id="fb53a-184">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb53a-184">dateTimeOffset</span></span>|<span data-ttu-id="fb53a-185">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fb53a-185">Read only.</span></span> <span data-ttu-id="fb53a-186">Временная метка, в которой сообщение чата удалено, или значение null, если оно не удалено.</span><span class="sxs-lookup"><span data-stu-id="fb53a-186">Timestamp at which the chat message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="fb53a-187">subject</span><span class="sxs-lookup"><span data-stu-id="fb53a-187">subject</span></span>|<span data-ttu-id="fb53a-188">string</span><span class="sxs-lookup"><span data-stu-id="fb53a-188">string</span></span>| <span data-ttu-id="fb53a-189">Тема сообщения чата в виде открытого текста.</span><span class="sxs-lookup"><span data-stu-id="fb53a-189">The subject of the chat message, in plaintext.</span></span>|
|<span data-ttu-id="fb53a-190">body</span><span class="sxs-lookup"><span data-stu-id="fb53a-190">body</span></span>|[<span data-ttu-id="fb53a-191">itemBody</span><span class="sxs-lookup"><span data-stu-id="fb53a-191">itemBody</span></span>](itembody.md)|<span data-ttu-id="fb53a-192">Представление содержимого сообщения чата в формате обычного текста или в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="fb53a-192">Plaintext/HTML representation of the content of the chat message.</span></span> <span data-ttu-id="fb53a-193">Представление определяется параметром contentType в тексте.</span><span class="sxs-lookup"><span data-stu-id="fb53a-193">Representation is specified by the contentType inside the body.</span></span> <span data-ttu-id="fb53a-194">Если сообщение чата содержит [чатмессажементион](chatmessagemention.md), содержимое всегда находится в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="fb53a-194">The content is always in HTML if the chat message contains a [chatMessageMention](chatmessagemention.md).</span></span> |
|<span data-ttu-id="fb53a-195">summary</span><span class="sxs-lookup"><span data-stu-id="fb53a-195">summary</span></span>|<span data-ttu-id="fb53a-196">string</span><span class="sxs-lookup"><span data-stu-id="fb53a-196">string</span></span>| <span data-ttu-id="fb53a-197">Сводный текст сообщения чата, которое можно использовать для push-уведомлений и сводных представлений, а также для обратного просмотра.</span><span class="sxs-lookup"><span data-stu-id="fb53a-197">Summary text of the chat message that could be used for push notifications and summary views or fall back views.</span></span> <span data-ttu-id="fb53a-198">Применяется только к сообщениям разговора по каналу, а не к сообщениям в чате.</span><span class="sxs-lookup"><span data-stu-id="fb53a-198">Only applies to channel chat messages, not chat messages in a chat.</span></span> |
|<span data-ttu-id="fb53a-199">attachments</span><span class="sxs-lookup"><span data-stu-id="fb53a-199">attachments</span></span>|<span data-ttu-id="fb53a-200">Коллекция [chatMessageAttachment](chatmessageattachment.md)</span><span class="sxs-lookup"><span data-stu-id="fb53a-200">[chatMessageAttachment](chatmessageattachment.md) collection</span></span> |<span data-ttu-id="fb53a-201">Вложенные файлы.</span><span class="sxs-lookup"><span data-stu-id="fb53a-201">Attached files.</span></span> <span data-ttu-id="fb53a-202">В настоящее время вложения доступны только для чтения. Отправка вложений не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb53a-202">Attachments are currently read-only – sending attachments is not supported.</span></span> |
|<span data-ttu-id="fb53a-203">mentions</span><span class="sxs-lookup"><span data-stu-id="fb53a-203">mentions</span></span>|<span data-ttu-id="fb53a-204">Коллекция [chatMessageMention](chatmessagemention.md)</span><span class="sxs-lookup"><span data-stu-id="fb53a-204">[chatMessageMention](chatmessagemention.md) collection</span></span>| <span data-ttu-id="fb53a-205">Список сущностей, упоминаемых в сообщении чата.</span><span class="sxs-lookup"><span data-stu-id="fb53a-205">List of entities mentioned in the chat message.</span></span> <span data-ttu-id="fb53a-206">В настоящее время поддерживаются значения user, bot, team и channel.</span><span class="sxs-lookup"><span data-stu-id="fb53a-206">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="fb53a-207">importance</span><span class="sxs-lookup"><span data-stu-id="fb53a-207">importance</span></span>| <span data-ttu-id="fb53a-208">чатмессажеимпортанце</span><span class="sxs-lookup"><span data-stu-id="fb53a-208">chatMessageImportance</span></span> | <span data-ttu-id="fb53a-209">Важность сообщения чата.</span><span class="sxs-lookup"><span data-stu-id="fb53a-209">The importance of the chat message.</span></span> <span data-ttu-id="fb53a-210">Допустимые значения: `normal`, `high`, `urgent`.</span><span class="sxs-lookup"><span data-stu-id="fb53a-210">The possible values are: `normal`, `high`, `urgent`.</span></span>|
|<span data-ttu-id="fb53a-211">reactions</span><span class="sxs-lookup"><span data-stu-id="fb53a-211">reactions</span></span>| <span data-ttu-id="fb53a-212">Коллекция [chatMessageReaction](chatmessagereaction.md)</span><span class="sxs-lookup"><span data-stu-id="fb53a-212">[chatMessageReaction](chatmessagereaction.md) collection</span></span> | <span data-ttu-id="fb53a-213">Реакции на это сообщение чата (например, например).</span><span class="sxs-lookup"><span data-stu-id="fb53a-213">Reactions for this chat message (for example, Like).</span></span>|
|<span data-ttu-id="fb53a-214">языковые стандарты</span><span class="sxs-lookup"><span data-stu-id="fb53a-214">locale</span></span>|<span data-ttu-id="fb53a-215">string</span><span class="sxs-lookup"><span data-stu-id="fb53a-215">string</span></span>|<span data-ttu-id="fb53a-216">Язык сообщения чата, заданное клиентом.</span><span class="sxs-lookup"><span data-stu-id="fb53a-216">Locale of the chat message set by the client.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fb53a-217">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fb53a-217">JSON representation</span></span>

<span data-ttu-id="fb53a-218">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fb53a-218">The following is a JSON representation of the resource.</span></span>

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
