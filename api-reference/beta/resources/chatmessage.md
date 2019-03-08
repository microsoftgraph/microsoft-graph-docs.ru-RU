---
title: Тип ресурса chatMessage
description: Представляет отдельное сообщение чата в объекте channel или chat. Сообщение может быть корневым или частью беседы, определяемой свойством **replyToId** в сообщении.
localization_priority: Priority
ms.openlocfilehash: f61668d8c3892482043dd7531a6699974a964527
ms.sourcegitcommit: d1a9e7c8e1376a99c5a5416257889ec113613a77
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/07/2019
ms.locfileid: "30458661"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="3b8d5-104">Тип ресурса chatMessage</span><span class="sxs-lookup"><span data-stu-id="3b8d5-104">chatMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b8d5-105">Представляет отдельное сообщение чата в объекте [channel](channel.md) или chat.</span><span class="sxs-lookup"><span data-stu-id="3b8d5-105">Represents an individual chat message within a [channel](channel.md) or chat entity.</span></span> <span data-ttu-id="3b8d5-106">Сообщение может быть корневым или частью беседы, определяемой свойством **replyToId** в сообщении.</span><span class="sxs-lookup"><span data-stu-id="3b8d5-106">The message can be an root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>

## <a name="methods"></a><span data-ttu-id="3b8d5-107">Методы</span><span class="sxs-lookup"><span data-stu-id="3b8d5-107">Methods</span></span>

| <span data-ttu-id="3b8d5-108">Метод</span><span class="sxs-lookup"><span data-stu-id="3b8d5-108">Method</span></span>       | <span data-ttu-id="3b8d5-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3b8d5-109">Return Type</span></span>  |<span data-ttu-id="3b8d5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3b8d5-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3b8d5-111">Перечисление сообщений в канале</span><span class="sxs-lookup"><span data-stu-id="3b8d5-111">List Channel messages</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="3b8d5-112">Коллекция [chatmessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="3b8d5-112">[chatmessage](chatmessage.md) collection</span></span> | <span data-ttu-id="3b8d5-113">Получение списка всех корневых сообщений в канале.</span><span class="sxs-lookup"><span data-stu-id="3b8d5-113">Get the list of all root messages in a channel.</span></span>|
|[<span data-ttu-id="3b8d5-114">Получение сообщения в канале</span><span class="sxs-lookup"><span data-stu-id="3b8d5-114">Get Channel message</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="3b8d5-115">chatmessage</span><span class="sxs-lookup"><span data-stu-id="3b8d5-115">chatmessage</span></span>](chatmessage.md) | <span data-ttu-id="3b8d5-116">Получение одного корневого сообщения из канала.</span><span class="sxs-lookup"><span data-stu-id="3b8d5-116">Get a single root message from a channel.</span></span>|
|[<span data-ttu-id="3b8d5-117">Перечисление ответов на сообщение</span><span class="sxs-lookup"><span data-stu-id="3b8d5-117">List replies to a message</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="3b8d5-118">Коллекция [chatmessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="3b8d5-118">[chatmessage](chatmessage.md) collection</span></span>| <span data-ttu-id="3b8d5-119">Получение списка всех ответов на сообщение в канале.</span><span class="sxs-lookup"><span data-stu-id="3b8d5-119">Get the list of all replies to a message in channel.</span></span>|
|[<span data-ttu-id="3b8d5-120">Получение ответа на сообщение</span><span class="sxs-lookup"><span data-stu-id="3b8d5-120">Get a reply to a message</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="3b8d5-121">chatmessage</span><span class="sxs-lookup"><span data-stu-id="3b8d5-121">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="3b8d5-122">Получение одного ответа на сообщение в канале.</span><span class="sxs-lookup"><span data-stu-id="3b8d5-122">Get a single reply to a message in a channel.</span></span>|
|<span data-ttu-id="3b8d5-123">[Отправка сообщения в канал](../api/channel-post-chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="3b8d5-123">Use [Create a message in a channel](../api/channel-post-chatmessage.md) instead.</span></span> | [<span data-ttu-id="3b8d5-124">chatmessage</span><span class="sxs-lookup"><span data-stu-id="3b8d5-124">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="3b8d5-125">Создание сообщения верхнего уровня в канале.</span><span class="sxs-lookup"><span data-stu-id="3b8d5-125">Use Create a message in a channel instead.</span></span>|
|<span data-ttu-id="3b8d5-126">[Ответ на сообщение в канале](../api/channel-post-messagereply.md)</span><span class="sxs-lookup"><span data-stu-id="3b8d5-126">Introduced the [Reply to a message in a channel](../api/channel-post-messagereply.md) API.</span></span> | [<span data-ttu-id="3b8d5-127">chatmessage</span><span class="sxs-lookup"><span data-stu-id="3b8d5-127">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="3b8d5-128">Ответ на существующее сообщение в канале.</span><span class="sxs-lookup"><span data-stu-id="3b8d5-128">Reply to an existing message in a channel.</span></span>|


## <a name="properties"></a><span data-ttu-id="3b8d5-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="3b8d5-129">Properties</span></span>
| <span data-ttu-id="3b8d5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3b8d5-130">Property</span></span>     | <span data-ttu-id="3b8d5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3b8d5-131">Type</span></span>   |<span data-ttu-id="3b8d5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3b8d5-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3b8d5-133">id</span><span class="sxs-lookup"><span data-stu-id="3b8d5-133">id</span></span>|<span data-ttu-id="3b8d5-134">String</span><span class="sxs-lookup"><span data-stu-id="3b8d5-134">String</span></span>| <span data-ttu-id="3b8d5-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3b8d5-135">Read-only.</span></span> <span data-ttu-id="3b8d5-136">Уникальный идентификатор сообщения.</span><span class="sxs-lookup"><span data-stu-id="3b8d5-136">Unique ID of the message.</span></span>|
|<span data-ttu-id="3b8d5-137">replyToId</span><span class="sxs-lookup"><span data-stu-id="3b8d5-137">replyToId</span></span>| <span data-ttu-id="3b8d5-138">string</span><span class="sxs-lookup"><span data-stu-id="3b8d5-138">string</span></span> | <span data-ttu-id="3b8d5-139">Идентификатор родительского или корневого сообщения беседы</span><span class="sxs-lookup"><span data-stu-id="3b8d5-139">Id of the parent message/root message of the thread</span></span> |
|<span data-ttu-id="3b8d5-140">from</span><span class="sxs-lookup"><span data-stu-id="3b8d5-140">from</span></span>|[<span data-ttu-id="3b8d5-141">identitySet</span><span class="sxs-lookup"><span data-stu-id="3b8d5-141">identitySet</span></span>](identityset.md)| <span data-ttu-id="3b8d5-142">Сведения об отправителе сообщения</span><span class="sxs-lookup"><span data-stu-id="3b8d5-142">Details of the sender of the message</span></span>|
|<span data-ttu-id="3b8d5-143">etag</span><span class="sxs-lookup"><span data-stu-id="3b8d5-143">etag</span></span>| <span data-ttu-id="3b8d5-144">string</span><span class="sxs-lookup"><span data-stu-id="3b8d5-144">string</span></span> | <span data-ttu-id="3b8d5-145">Номер версии сообщения</span><span class="sxs-lookup"><span data-stu-id="3b8d5-145">Version number of the message</span></span> |
|<span data-ttu-id="3b8d5-146">messageType</span><span class="sxs-lookup"><span data-stu-id="3b8d5-146">messageType</span></span>|<span data-ttu-id="3b8d5-147">String</span><span class="sxs-lookup"><span data-stu-id="3b8d5-147">String</span></span>|<span data-ttu-id="3b8d5-148">Тип сообщения. Поддерживаемые в настоящее время значения: message, chatEvent, Typing</span><span class="sxs-lookup"><span data-stu-id="3b8d5-148">The type of message, current supported values are: message, chatEvent, Typing</span></span>|
|<span data-ttu-id="3b8d5-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3b8d5-149">createdDateTime</span></span>|<span data-ttu-id="3b8d5-150">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b8d5-150">dateTimeOffset</span></span>|<span data-ttu-id="3b8d5-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3b8d5-151">Read only.</span></span> <span data-ttu-id="3b8d5-152">Метка времени создания сообщения</span><span class="sxs-lookup"><span data-stu-id="3b8d5-152">Timestamp of when the message was created</span></span>|
|<span data-ttu-id="3b8d5-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3b8d5-153">lastModifiedDateTime</span></span>|<span data-ttu-id="3b8d5-154">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b8d5-154">dateTimeOffset</span></span>|<span data-ttu-id="3b8d5-155">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3b8d5-155">Read only.</span></span> <span data-ttu-id="3b8d5-156">Метка времени изменения или обновления сообщения</span><span class="sxs-lookup"><span data-stu-id="3b8d5-156">Timestamp of when the message was edited/updated</span></span>|
|<span data-ttu-id="3b8d5-157">deleted</span><span class="sxs-lookup"><span data-stu-id="3b8d5-157">deleted</span></span>|<span data-ttu-id="3b8d5-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b8d5-158">Boolean</span></span>|<span data-ttu-id="3b8d5-159">Указывает, удалено ли сообщение с возможностью восстановления</span><span class="sxs-lookup"><span data-stu-id="3b8d5-159">Indicates whether a message has been soft deleted</span></span>|
|<span data-ttu-id="3b8d5-160">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="3b8d5-160">deletedDateTime</span></span>|<span data-ttu-id="3b8d5-161">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b8d5-161">dateTimeOffset</span></span>|<span data-ttu-id="3b8d5-162">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3b8d5-162">Read only.</span></span> <span data-ttu-id="3b8d5-163">Метка времени удаления сообщения</span><span class="sxs-lookup"><span data-stu-id="3b8d5-163">Timestamp at which the message was deleted</span></span> |
|<span data-ttu-id="3b8d5-164">subject</span><span class="sxs-lookup"><span data-stu-id="3b8d5-164">subject</span></span>|<span data-ttu-id="3b8d5-165">string</span><span class="sxs-lookup"><span data-stu-id="3b8d5-165">string</span></span>|<span data-ttu-id="3b8d5-166">Строка темы сообщения.</span><span class="sxs-lookup"><span data-stu-id="3b8d5-166">Message subject line.</span></span> <span data-ttu-id="3b8d5-167">Необязательное</span><span class="sxs-lookup"><span data-stu-id="3b8d5-167">Optional</span></span>|
|<span data-ttu-id="3b8d5-168">body</span><span class="sxs-lookup"><span data-stu-id="3b8d5-168">body</span></span>|[<span data-ttu-id="3b8d5-169">itemBody</span><span class="sxs-lookup"><span data-stu-id="3b8d5-169">itemBody</span></span>](itembody.md)|<span data-ttu-id="3b8d5-170">Представление содержимого сообщения в формате Plaintext/HTML.</span><span class="sxs-lookup"><span data-stu-id="3b8d5-170">Plaintext/HTML representation of the content of the message.</span></span> <span data-ttu-id="3b8d5-171">Возвращает неформатированный текст по умолчанию. Приложение может выбрать формат HTML в составе параметров запроса</span><span class="sxs-lookup"><span data-stu-id="3b8d5-171">Returns plain text by default, application can choose HTML as part of a query param</span></span>|
|<span data-ttu-id="3b8d5-172">summary</span><span class="sxs-lookup"><span data-stu-id="3b8d5-172">summary</span></span>|<span data-ttu-id="3b8d5-173">string</span><span class="sxs-lookup"><span data-stu-id="3b8d5-173">string</span></span>|<span data-ttu-id="3b8d5-174">Сводный текст сообщения, который можно использовать для push-уведомлений и представлений сводки или резервных представлений</span><span class="sxs-lookup"><span data-stu-id="3b8d5-174">Summary text of the message that could be used for push notifications and summary views or fall back views</span></span>|
|<span data-ttu-id="3b8d5-175">mentions</span><span class="sxs-lookup"><span data-stu-id="3b8d5-175">mentions</span></span>|<span data-ttu-id="3b8d5-176">Коллекция [chatMessageMention](chatmention.md)</span><span class="sxs-lookup"><span data-stu-id="3b8d5-176">[chatMessageMention](chatmention.md) collection</span></span>| <span data-ttu-id="3b8d5-177">Список сущностей, упомянутых в сообщении.</span><span class="sxs-lookup"><span data-stu-id="3b8d5-177">List of entities mentioned in the message.</span></span> <span data-ttu-id="3b8d5-178">Поддерживаемые в настоящее время: user, bot, team, channel</span><span class="sxs-lookup"><span data-stu-id="3b8d5-178">Currently supports user, bot, team, channel</span></span>|
|<span data-ttu-id="3b8d5-179">importance</span><span class="sxs-lookup"><span data-stu-id="3b8d5-179">importance</span></span>| <span data-ttu-id="3b8d5-180">string</span><span class="sxs-lookup"><span data-stu-id="3b8d5-180">string</span></span> | <span data-ttu-id="3b8d5-181">Важность сообщения: высокая, низкая</span><span class="sxs-lookup"><span data-stu-id="3b8d5-181">The importance of the message: Normal, High</span></span>|
|<span data-ttu-id="3b8d5-182">reactions</span><span class="sxs-lookup"><span data-stu-id="3b8d5-182">reactions</span></span>| <span data-ttu-id="3b8d5-183">Коллекция [chatMessageReaction](chatreaction.md)</span><span class="sxs-lookup"><span data-stu-id="3b8d5-183">[chatMessageReaction](chatreaction.md) collection</span></span> | <span data-ttu-id="3b8d5-184">Реакции на сообщение (например, "Нравится")</span><span class="sxs-lookup"><span data-stu-id="3b8d5-184">Reactions for this message (for example, Like)</span></span>|
|<span data-ttu-id="3b8d5-185">locale</span><span class="sxs-lookup"><span data-stu-id="3b8d5-185">locale</span></span>|<span data-ttu-id="3b8d5-186">string</span><span class="sxs-lookup"><span data-stu-id="3b8d5-186">string</span></span>|<span data-ttu-id="3b8d5-187">Язык сообщения, установленный клиентом</span><span class="sxs-lookup"><span data-stu-id="3b8d5-187">Locale of the message set by the client</span></span>|
|<span data-ttu-id="3b8d5-188">attachments</span><span class="sxs-lookup"><span data-stu-id="3b8d5-188">attachments</span></span>|<span data-ttu-id="3b8d5-189">Коллекция [chatMessageAttachment](chatattachment.md)</span><span class="sxs-lookup"><span data-stu-id="3b8d5-189">[chatMessageAttachment](chatattachment.md) collection</span></span> |<span data-ttu-id="3b8d5-190">Вложенные файлы</span><span class="sxs-lookup"><span data-stu-id="3b8d5-190">Attached files</span></span>|


## <a name="json-representation"></a><span data-ttu-id="3b8d5-191">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3b8d5-191">JSON representation</span></span>

<span data-ttu-id="3b8d5-192">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3b8d5-192">The following is a JSON representation of the resource.</span></span>

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
  "isDeleted": "boolean",
  "deletedDateTime": "string (timestamp)",
  "subject": "string",
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "summary": "string",
  "attachments": [{"@odata.type": "microsoft.graph.chatMessageAttachment"}],
  "mentions": [{"@odata.type": "microsoft.graph.chatMessageMention"}],
  "importance": "string",
  "reactions": [{"@odata.type": "microsoft.graph.chatMessageReaction"}],
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
  "suppressions": [
    "Error: /api-reference/beta/resources/chatmessage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
