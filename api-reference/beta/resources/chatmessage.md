---
title: Тип ресурса chatMessage
description: Представляет отдельное сообщение чата в объекте channel или chat. Сообщение может быть корневым или частью беседы, определяемой свойством **replyToId** в сообщении.
localization_priority: Priority
ms.openlocfilehash: a74f422c6bf60e1293d8620b440152be77dacdc7
ms.sourcegitcommit: cd4bdb2c6754b1d5658e68909ea6c219466da6df
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/16/2019
ms.locfileid: "30644323"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="7f08d-104">Тип ресурса chatMessage</span><span class="sxs-lookup"><span data-stu-id="7f08d-104">chatMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f08d-105">Представляет отдельное сообщение чата в объекте [channel](channel.md) или chat.</span><span class="sxs-lookup"><span data-stu-id="7f08d-105">Represents an individual chat message within a [channel](channel.md) or chat entity.</span></span> <span data-ttu-id="7f08d-106">Сообщение может быть корневым или частью беседы, определяемой свойством **replyToId** в сообщении.</span><span class="sxs-lookup"><span data-stu-id="7f08d-106">The message can be an root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>

## <a name="methods"></a><span data-ttu-id="7f08d-107">Методы</span><span class="sxs-lookup"><span data-stu-id="7f08d-107">Methods</span></span>

| <span data-ttu-id="7f08d-108">Метод</span><span class="sxs-lookup"><span data-stu-id="7f08d-108">Method</span></span>       | <span data-ttu-id="7f08d-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7f08d-109">Return Type</span></span>  |<span data-ttu-id="7f08d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7f08d-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7f08d-111">Перечисление сообщений в канале</span><span class="sxs-lookup"><span data-stu-id="7f08d-111">List Channel messages</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="7f08d-112">Коллекция [chatmessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="7f08d-112">[chatmessage](chatmessage.md) collection</span></span> | <span data-ttu-id="7f08d-113">Получение списка всех корневых сообщений в канале.</span><span class="sxs-lookup"><span data-stu-id="7f08d-113">Get the list of all root messages in a channel.</span></span>|
|[<span data-ttu-id="7f08d-114">Получение сообщения в канале</span><span class="sxs-lookup"><span data-stu-id="7f08d-114">Get Channel message</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="7f08d-115">chatmessage</span><span class="sxs-lookup"><span data-stu-id="7f08d-115">chatmessage</span></span>](chatmessage.md) | <span data-ttu-id="7f08d-116">Получение одного корневого сообщения из канала.</span><span class="sxs-lookup"><span data-stu-id="7f08d-116">Get a single root message from a channel.</span></span>|
|[<span data-ttu-id="7f08d-117">Перечисление ответов на сообщение</span><span class="sxs-lookup"><span data-stu-id="7f08d-117">List replies to a message</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="7f08d-118">Коллекция [chatmessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="7f08d-118">[chatmessage](chatmessage.md) collection</span></span>| <span data-ttu-id="7f08d-119">Получение списка всех ответов на сообщение в канале.</span><span class="sxs-lookup"><span data-stu-id="7f08d-119">Get the list of all replies to a message in channel.</span></span>|
|[<span data-ttu-id="7f08d-120">Получение ответа на сообщение</span><span class="sxs-lookup"><span data-stu-id="7f08d-120">Get a reply to a message</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="7f08d-121">chatmessage</span><span class="sxs-lookup"><span data-stu-id="7f08d-121">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="7f08d-122">Получение одного ответа на сообщение в канале.</span><span class="sxs-lookup"><span data-stu-id="7f08d-122">Get a single reply to a message in a channel.</span></span>|
|[<span data-ttu-id="7f08d-123">Отправка сообщения в канал</span><span class="sxs-lookup"><span data-stu-id="7f08d-123">Send a message in a channel</span></span>](../api/channel-post-chatmessage.md) | [<span data-ttu-id="7f08d-124">chatmessage</span><span class="sxs-lookup"><span data-stu-id="7f08d-124">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="7f08d-125">Создание сообщения верхнего уровня в канале.</span><span class="sxs-lookup"><span data-stu-id="7f08d-125">Create a new top-level message in a channel.</span></span>|
|[<span data-ttu-id="7f08d-126">Ответ на сообщение в канале</span><span class="sxs-lookup"><span data-stu-id="7f08d-126">Reply to a message in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="7f08d-127">chatmessage</span><span class="sxs-lookup"><span data-stu-id="7f08d-127">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="7f08d-128">Ответ на существующее сообщение в канале.</span><span class="sxs-lookup"><span data-stu-id="7f08d-128">Reply to an existing message in a channel.</span></span>|


## <a name="properties"></a><span data-ttu-id="7f08d-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="7f08d-129">Properties</span></span>
| <span data-ttu-id="7f08d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7f08d-130">Property</span></span>     | <span data-ttu-id="7f08d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7f08d-131">Type</span></span>   |<span data-ttu-id="7f08d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7f08d-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7f08d-133">id</span><span class="sxs-lookup"><span data-stu-id="7f08d-133">id</span></span>|<span data-ttu-id="7f08d-134">String</span><span class="sxs-lookup"><span data-stu-id="7f08d-134">String</span></span>| <span data-ttu-id="7f08d-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7f08d-135">Read-only.</span></span> <span data-ttu-id="7f08d-136">Уникальный идентификатор сообщения.</span><span class="sxs-lookup"><span data-stu-id="7f08d-136">Unique ID of the message.</span></span>|
|<span data-ttu-id="7f08d-137">replyToId</span><span class="sxs-lookup"><span data-stu-id="7f08d-137">replyToId</span></span>| <span data-ttu-id="7f08d-138">string</span><span class="sxs-lookup"><span data-stu-id="7f08d-138">string</span></span> | <span data-ttu-id="7f08d-139">Идентификатор родительского или корневого сообщения беседы.</span><span class="sxs-lookup"><span data-stu-id="7f08d-139">Id of the parent message/root message of the thread</span></span> |
|<span data-ttu-id="7f08d-140">from</span><span class="sxs-lookup"><span data-stu-id="7f08d-140">from</span></span>|[<span data-ttu-id="7f08d-141">identitySet</span><span class="sxs-lookup"><span data-stu-id="7f08d-141">identitySet</span></span>](identityset.md)| <span data-ttu-id="7f08d-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7f08d-142">Read only.</span></span> <span data-ttu-id="7f08d-143">Подробные сведения об отправителе сообщения.</span><span class="sxs-lookup"><span data-stu-id="7f08d-143">Details of the sender of the message</span></span>|
|<span data-ttu-id="7f08d-144">etag</span><span class="sxs-lookup"><span data-stu-id="7f08d-144">etag</span></span>| <span data-ttu-id="7f08d-145">строка</span><span class="sxs-lookup"><span data-stu-id="7f08d-145">string</span></span> | <span data-ttu-id="7f08d-146">Номер версии сообщения.</span><span class="sxs-lookup"><span data-stu-id="7f08d-146">Version number of the message</span></span> |
|<span data-ttu-id="7f08d-147">messageType</span><span class="sxs-lookup"><span data-stu-id="7f08d-147">messageType</span></span>|<span data-ttu-id="7f08d-148">Строка</span><span class="sxs-lookup"><span data-stu-id="7f08d-148">String</span></span>|<span data-ttu-id="7f08d-149">Тип сообщения. В настоящее время поддерживаются следующие значения: message, chatEvent, Typing.</span><span class="sxs-lookup"><span data-stu-id="7f08d-149">The type of message, current supported values are: message, chatEvent, Typing</span></span>|
|<span data-ttu-id="7f08d-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7f08d-150">createdDateTime</span></span>|<span data-ttu-id="7f08d-151">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f08d-151">dateTimeOffset</span></span>|<span data-ttu-id="7f08d-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7f08d-152">Read only.</span></span> <span data-ttu-id="7f08d-153">Метка времени создания сообщения.</span><span class="sxs-lookup"><span data-stu-id="7f08d-153">Timestamp of when the message was created</span></span>|
|<span data-ttu-id="7f08d-154">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7f08d-154">lastModifiedDateTime</span></span>|<span data-ttu-id="7f08d-155">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f08d-155">dateTimeOffset</span></span>|<span data-ttu-id="7f08d-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7f08d-156">Read only.</span></span> <span data-ttu-id="7f08d-157">Метка времени изменения или обновления сообщения.</span><span class="sxs-lookup"><span data-stu-id="7f08d-157">Timestamp of when the message was edited/updated</span></span>|
|<span data-ttu-id="7f08d-158">deleted</span><span class="sxs-lookup"><span data-stu-id="7f08d-158">deleted</span></span>|<span data-ttu-id="7f08d-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f08d-159">Boolean</span></span>|<span data-ttu-id="7f08d-160">Указывает, было ли сообщение обратимо удалено.</span><span class="sxs-lookup"><span data-stu-id="7f08d-160">Indicates whether a message has been soft deleted</span></span>|
|<span data-ttu-id="7f08d-161">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="7f08d-161">deletedDateTime</span></span>|<span data-ttu-id="7f08d-162">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f08d-162">dateTimeOffset</span></span>|<span data-ttu-id="7f08d-163">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7f08d-163">Read only.</span></span> <span data-ttu-id="7f08d-164">Метка времени удаления сообщения.</span><span class="sxs-lookup"><span data-stu-id="7f08d-164">Timestamp at which the message was deleted</span></span> |
|<span data-ttu-id="7f08d-165">subject</span><span class="sxs-lookup"><span data-stu-id="7f08d-165">subject</span></span>|<span data-ttu-id="7f08d-166">string</span><span class="sxs-lookup"><span data-stu-id="7f08d-166">string</span></span>|<span data-ttu-id="7f08d-167">Строка темы сообщения.</span><span class="sxs-lookup"><span data-stu-id="7f08d-167">Message subject line.</span></span> <span data-ttu-id="7f08d-168">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="7f08d-168">Optional.</span></span>|
|<span data-ttu-id="7f08d-169">body</span><span class="sxs-lookup"><span data-stu-id="7f08d-169">body</span></span>|[<span data-ttu-id="7f08d-170">itemBody</span><span class="sxs-lookup"><span data-stu-id="7f08d-170">itemBody</span></span>](itembody.md)|<span data-ttu-id="7f08d-171">Представление содержимого сообщения в формате Plaintext/HTML.</span><span class="sxs-lookup"><span data-stu-id="7f08d-171">Plaintext/HTML representation of the content of the message.</span></span> <span data-ttu-id="7f08d-172">Возвращает неформатированный текст по умолчанию. Приложение может выбрать формат HTML в составе параметров запроса</span><span class="sxs-lookup"><span data-stu-id="7f08d-172">Returns plain text by default, application can choose HTML as part of a query param</span></span>|
|<span data-ttu-id="7f08d-173">summary</span><span class="sxs-lookup"><span data-stu-id="7f08d-173">summary</span></span>|<span data-ttu-id="7f08d-174">string</span><span class="sxs-lookup"><span data-stu-id="7f08d-174">string</span></span>|<span data-ttu-id="7f08d-175">Сводный текст сообщения, который можно использовать для push-уведомлений и представлений сводки или резервных представлений</span><span class="sxs-lookup"><span data-stu-id="7f08d-175">Summary text of the message that could be used for push notifications and summary views or fall back views</span></span>|
|<span data-ttu-id="7f08d-176">mentions</span><span class="sxs-lookup"><span data-stu-id="7f08d-176">mentions</span></span>|<span data-ttu-id="7f08d-177">Коллекция [chatMessageMention](chatmention.md)</span><span class="sxs-lookup"><span data-stu-id="7f08d-177">[chatMessageMention](chatmention.md) collection</span></span>| <span data-ttu-id="7f08d-178">Список сущностей, упомянутых в сообщении.</span><span class="sxs-lookup"><span data-stu-id="7f08d-178">List of entities mentioned in the message.</span></span> <span data-ttu-id="7f08d-179">В настоящее время поддерживаются значения user, bot, team и channel.</span><span class="sxs-lookup"><span data-stu-id="7f08d-179">Currently supports user, bot, team, channel</span></span>|
|<span data-ttu-id="7f08d-180">importance</span><span class="sxs-lookup"><span data-stu-id="7f08d-180">importance</span></span>| <span data-ttu-id="7f08d-181">строка</span><span class="sxs-lookup"><span data-stu-id="7f08d-181">string</span></span> | <span data-ttu-id="7f08d-182">Важность сообщения: Normal, High.</span><span class="sxs-lookup"><span data-stu-id="7f08d-182">The importance of the message: Normal, High</span></span>|
|<span data-ttu-id="7f08d-183">reactions</span><span class="sxs-lookup"><span data-stu-id="7f08d-183">reactions</span></span>| <span data-ttu-id="7f08d-184">Коллекция [chatMessageReaction](chatreaction.md)</span><span class="sxs-lookup"><span data-stu-id="7f08d-184">[chatMessageReaction](chatreaction.md) collection</span></span> | <span data-ttu-id="7f08d-185">Реакции на сообщение (например, "Нравится")</span><span class="sxs-lookup"><span data-stu-id="7f08d-185">Reactions for this message (for example, Like)</span></span>|
|<span data-ttu-id="7f08d-186">locale</span><span class="sxs-lookup"><span data-stu-id="7f08d-186">locale</span></span>|<span data-ttu-id="7f08d-187">string</span><span class="sxs-lookup"><span data-stu-id="7f08d-187">string</span></span>|<span data-ttu-id="7f08d-188">Язык сообщения, установленный клиентом</span><span class="sxs-lookup"><span data-stu-id="7f08d-188">Locale of the message set by the client</span></span>|
|<span data-ttu-id="7f08d-189">attachments</span><span class="sxs-lookup"><span data-stu-id="7f08d-189">attachments</span></span>|<span data-ttu-id="7f08d-190">Коллекция [chatMessageAttachment](chatattachment.md)</span><span class="sxs-lookup"><span data-stu-id="7f08d-190">[chatMessageAttachment](chatattachment.md) collection</span></span> |<span data-ttu-id="7f08d-191">Вложенные файлы.</span><span class="sxs-lookup"><span data-stu-id="7f08d-191">Attached files</span></span> <span data-ttu-id="7f08d-192">В настоящее время вложения доступны только для чтения. Отправка вложений не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f08d-192">Attachments are currently read-only – sending attachments is not supported.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="7f08d-193">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7f08d-193">JSON representation</span></span>

<span data-ttu-id="7f08d-194">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7f08d-194">The following is a JSON representation of the resource.</span></span>

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
