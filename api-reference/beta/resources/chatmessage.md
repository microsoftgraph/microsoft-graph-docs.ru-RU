---
title: Тип ресурса chatMessage
description: Представляет отдельное сообщение чата в объекте channel или chat. Сообщение может быть корневым или частью беседы, определяемой свойством **replyToId** в сообщении.
localization_priority: Priority
ms.openlocfilehash: ef91281eff0cc61f992f659bd33debec03841bb4
ms.sourcegitcommit: a1f1e59ee568340bfabdb524e01cff7860bcc862
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/05/2019
ms.locfileid: "29735581"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="72b3f-104">Тип ресурса chatMessage</span><span class="sxs-lookup"><span data-stu-id="72b3f-104">chatMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72b3f-105">Представляет отдельное сообщение чата в объекте [channel](channel.md) или chat.</span><span class="sxs-lookup"><span data-stu-id="72b3f-105">Represents an individual chat message within a [channel](channel.md) or chat entity.</span></span> <span data-ttu-id="72b3f-106">Сообщение может быть корневым или частью беседы, определяемой свойством **replyToId** в сообщении.</span><span class="sxs-lookup"><span data-stu-id="72b3f-106">The message can be an root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>

## <a name="methods"></a><span data-ttu-id="72b3f-107">Методы</span><span class="sxs-lookup"><span data-stu-id="72b3f-107">Methods</span></span>

| <span data-ttu-id="72b3f-108">Метод</span><span class="sxs-lookup"><span data-stu-id="72b3f-108">Method</span></span>       | <span data-ttu-id="72b3f-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="72b3f-109">Return Type</span></span>  |<span data-ttu-id="72b3f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="72b3f-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="72b3f-111">Перечисление сообщений в канале</span><span class="sxs-lookup"><span data-stu-id="72b3f-111">List Channel messages</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="72b3f-112">Коллекция [chatmessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="72b3f-112">[chatmessage](chatmessage.md) collection</span></span> | <span data-ttu-id="72b3f-113">Получение списка всех корневых сообщений в канале.</span><span class="sxs-lookup"><span data-stu-id="72b3f-113">Get the list of all root messages in a channel.</span></span>|
|[<span data-ttu-id="72b3f-114">Получение сообщения в канале</span><span class="sxs-lookup"><span data-stu-id="72b3f-114">Get Channel message</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="72b3f-115">chatmessage</span><span class="sxs-lookup"><span data-stu-id="72b3f-115">chatmessage</span></span>](chatmessage.md) | <span data-ttu-id="72b3f-116">Получение одного корневого сообщения из канала.</span><span class="sxs-lookup"><span data-stu-id="72b3f-116">Get a single root message from a channel.</span></span>|
|[<span data-ttu-id="72b3f-117">Перечисление ответов на сообщение</span><span class="sxs-lookup"><span data-stu-id="72b3f-117">List replies to a message</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="72b3f-118">Коллекция [chatmessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="72b3f-118">[chatmessage](chatmessage.md) collection</span></span>| <span data-ttu-id="72b3f-119">Получение списка всех ответов на сообщение в канале.</span><span class="sxs-lookup"><span data-stu-id="72b3f-119">Get the list of all replies to a message in channel.</span></span>|
|[<span data-ttu-id="72b3f-120">Получение ответа на сообщение</span><span class="sxs-lookup"><span data-stu-id="72b3f-120">Get a reply to a message</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="72b3f-121">chatmessage</span><span class="sxs-lookup"><span data-stu-id="72b3f-121">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="72b3f-122">Получение одного ответа на сообщение в канале.</span><span class="sxs-lookup"><span data-stu-id="72b3f-122">Get a single reply to a message in a channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="72b3f-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="72b3f-123">Properties</span></span>
| <span data-ttu-id="72b3f-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="72b3f-124">Property</span></span>     | <span data-ttu-id="72b3f-125">Тип</span><span class="sxs-lookup"><span data-stu-id="72b3f-125">Type</span></span>   |<span data-ttu-id="72b3f-126">Описание</span><span class="sxs-lookup"><span data-stu-id="72b3f-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="72b3f-127">id</span><span class="sxs-lookup"><span data-stu-id="72b3f-127">id</span></span>|<span data-ttu-id="72b3f-128">String</span><span class="sxs-lookup"><span data-stu-id="72b3f-128">String</span></span>| <span data-ttu-id="72b3f-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="72b3f-129">Read-only.</span></span> <span data-ttu-id="72b3f-130">Уникальный идентификатор сообщения.</span><span class="sxs-lookup"><span data-stu-id="72b3f-130">Unique ID of the message.</span></span>|
|<span data-ttu-id="72b3f-131">replyToId</span><span class="sxs-lookup"><span data-stu-id="72b3f-131">replyToId</span></span>| <span data-ttu-id="72b3f-132">string</span><span class="sxs-lookup"><span data-stu-id="72b3f-132">string</span></span> | <span data-ttu-id="72b3f-133">Идентификатор родительского или корневого сообщения беседы</span><span class="sxs-lookup"><span data-stu-id="72b3f-133">Id of the parent message/root message of the thread</span></span> |
|<span data-ttu-id="72b3f-134">from</span><span class="sxs-lookup"><span data-stu-id="72b3f-134">from</span></span>|[<span data-ttu-id="72b3f-135">identitySet</span><span class="sxs-lookup"><span data-stu-id="72b3f-135">identitySet</span></span>](identityset.md)| <span data-ttu-id="72b3f-136">Сведения об отправителе сообщения</span><span class="sxs-lookup"><span data-stu-id="72b3f-136">Details of the sender of the message</span></span>|
|<span data-ttu-id="72b3f-137">etag</span><span class="sxs-lookup"><span data-stu-id="72b3f-137">etag</span></span>| <span data-ttu-id="72b3f-138">string</span><span class="sxs-lookup"><span data-stu-id="72b3f-138">string</span></span> | <span data-ttu-id="72b3f-139">Номер версии сообщения</span><span class="sxs-lookup"><span data-stu-id="72b3f-139">Version number of the message</span></span> |
|<span data-ttu-id="72b3f-140">messageType</span><span class="sxs-lookup"><span data-stu-id="72b3f-140">messageType</span></span>|<span data-ttu-id="72b3f-141">String</span><span class="sxs-lookup"><span data-stu-id="72b3f-141">String</span></span>|<span data-ttu-id="72b3f-142">Тип сообщения. Поддерживаемые в настоящее время значения: message, chatEvent, Typing</span><span class="sxs-lookup"><span data-stu-id="72b3f-142">The type of message, current supported values are: message, chatEvent, Typing</span></span>|
|<span data-ttu-id="72b3f-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="72b3f-143">createdDateTime</span></span>|<span data-ttu-id="72b3f-144">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72b3f-144">dateTimeOffset</span></span>|<span data-ttu-id="72b3f-145">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="72b3f-145">Read only.</span></span> <span data-ttu-id="72b3f-146">Метка времени создания сообщения</span><span class="sxs-lookup"><span data-stu-id="72b3f-146">Timestamp of when the message was created</span></span>|
|<span data-ttu-id="72b3f-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="72b3f-147">lastModifiedDateTime</span></span>|<span data-ttu-id="72b3f-148">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72b3f-148">dateTimeOffset</span></span>|<span data-ttu-id="72b3f-149">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="72b3f-149">Read only.</span></span> <span data-ttu-id="72b3f-150">Метка времени изменения или обновления сообщения</span><span class="sxs-lookup"><span data-stu-id="72b3f-150">Timestamp of when the message was edited/updated</span></span>|
|<span data-ttu-id="72b3f-151">deleted</span><span class="sxs-lookup"><span data-stu-id="72b3f-151">deleted</span></span>|<span data-ttu-id="72b3f-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="72b3f-152">Boolean</span></span>|<span data-ttu-id="72b3f-153">Указывает, удалено ли сообщение с возможностью восстановления</span><span class="sxs-lookup"><span data-stu-id="72b3f-153">Represents if a message has been soft deleted</span></span>|
|<span data-ttu-id="72b3f-154">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="72b3f-154">deletedDateTime</span></span>|<span data-ttu-id="72b3f-155">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72b3f-155">dateTimeOffset</span></span>|<span data-ttu-id="72b3f-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="72b3f-156">Read only.</span></span> <span data-ttu-id="72b3f-157">Метка времени удаления сообщения</span><span class="sxs-lookup"><span data-stu-id="72b3f-157">Timestamp at which the message was deleted</span></span> |
|<span data-ttu-id="72b3f-158">subject</span><span class="sxs-lookup"><span data-stu-id="72b3f-158">subject</span></span>|<span data-ttu-id="72b3f-159">string</span><span class="sxs-lookup"><span data-stu-id="72b3f-159">string</span></span>|<span data-ttu-id="72b3f-160">Строка темы сообщения.</span><span class="sxs-lookup"><span data-stu-id="72b3f-160">Message subject line.</span></span> <span data-ttu-id="72b3f-161">Необязательное</span><span class="sxs-lookup"><span data-stu-id="72b3f-161">Optional</span></span>|
|<span data-ttu-id="72b3f-162">body</span><span class="sxs-lookup"><span data-stu-id="72b3f-162">body</span></span>|[<span data-ttu-id="72b3f-163">itemBody</span><span class="sxs-lookup"><span data-stu-id="72b3f-163">itemBody</span></span>](itembody.md)|<span data-ttu-id="72b3f-164">Представление содержимого сообщения в формате Plaintext/HTML.</span><span class="sxs-lookup"><span data-stu-id="72b3f-164">Plaintext/HTML representation of the content of the message.</span></span> <span data-ttu-id="72b3f-165">Возвращает неформатированный текст по умолчанию. Приложение может выбрать формат HTML в составе параметров запроса</span><span class="sxs-lookup"><span data-stu-id="72b3f-165">Returns plain text by default, application can choose HTML as part of a query param</span></span>|
|<span data-ttu-id="72b3f-166">summary</span><span class="sxs-lookup"><span data-stu-id="72b3f-166">summary</span></span>|<span data-ttu-id="72b3f-167">string</span><span class="sxs-lookup"><span data-stu-id="72b3f-167">string</span></span>|<span data-ttu-id="72b3f-168">Сводный текст сообщения, который можно использовать для push-уведомлений и представлений сводки или резервных представлений</span><span class="sxs-lookup"><span data-stu-id="72b3f-168">Summary text of the message that could be used for push notifications and summary views or fall back views</span></span>|
|<span data-ttu-id="72b3f-169">mentions</span><span class="sxs-lookup"><span data-stu-id="72b3f-169">mentions</span></span>|<span data-ttu-id="72b3f-170">Коллекция [chatMessageMention](chatmention.md)</span><span class="sxs-lookup"><span data-stu-id="72b3f-170">[chatMessageMention](chatmention.md) collection</span></span>| <span data-ttu-id="72b3f-171">Список сущностей, упомянутых в сообщении.</span><span class="sxs-lookup"><span data-stu-id="72b3f-171">List of entities mentioned in the message.</span></span> <span data-ttu-id="72b3f-172">Поддерживаемые в настоящее время: user, bot, team, channel</span><span class="sxs-lookup"><span data-stu-id="72b3f-172">Currently supports user, bot, team, channel</span></span>|
|<span data-ttu-id="72b3f-173">importance</span><span class="sxs-lookup"><span data-stu-id="72b3f-173">importance</span></span>| <span data-ttu-id="72b3f-174">string</span><span class="sxs-lookup"><span data-stu-id="72b3f-174">string</span></span> | <span data-ttu-id="72b3f-175">Важность сообщения: высокая, низкая</span><span class="sxs-lookup"><span data-stu-id="72b3f-175">The importance of the message: Normal, High</span></span>|
|<span data-ttu-id="72b3f-176">reactions</span><span class="sxs-lookup"><span data-stu-id="72b3f-176">reactions</span></span>| <span data-ttu-id="72b3f-177">Коллекция [chatMessageReaction](chatreaction.md)</span><span class="sxs-lookup"><span data-stu-id="72b3f-177">[chatMessageReaction](chatreaction.md) collection</span></span> | <span data-ttu-id="72b3f-178">Реакции на сообщение (например, "Нравится")</span><span class="sxs-lookup"><span data-stu-id="72b3f-178">Reactions for this message (for example, Like)</span></span>|
|<span data-ttu-id="72b3f-179">locale</span><span class="sxs-lookup"><span data-stu-id="72b3f-179">locale</span></span>|<span data-ttu-id="72b3f-180">string</span><span class="sxs-lookup"><span data-stu-id="72b3f-180">string</span></span>|<span data-ttu-id="72b3f-181">Язык сообщения, установленный клиентом</span><span class="sxs-lookup"><span data-stu-id="72b3f-181">Locale of the message set by the client</span></span>|
|<span data-ttu-id="72b3f-182">attachments</span><span class="sxs-lookup"><span data-stu-id="72b3f-182">attachments</span></span>|<span data-ttu-id="72b3f-183">Коллекция [chatMessageAttachment](chatattachment.md)</span><span class="sxs-lookup"><span data-stu-id="72b3f-183">[chatMessageAttachment](chatattachment.md) collection</span></span> |<span data-ttu-id="72b3f-184">Вложенные файлы</span><span class="sxs-lookup"><span data-stu-id="72b3f-184">Attached files</span></span>|


## <a name="json-representation"></a><span data-ttu-id="72b3f-185">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="72b3f-185">JSON representation</span></span>

<span data-ttu-id="72b3f-186">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="72b3f-186">The following is a JSON representation of the resource.</span></span>

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
