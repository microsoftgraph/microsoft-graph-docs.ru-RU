---
title: Тип ресурса chatMessage
description: Представляет отдельное сообщение чата в объекте channel или chat. Сообщение может быть корневым или частью беседы, определяемой свойством **replyToId** в сообщении.
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 893a7d09dba1ef376926c8ad7339e21a84cd83fa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543895"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="b9213-104">Тип ресурса chatMessage</span><span class="sxs-lookup"><span data-stu-id="b9213-104">chatMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9213-105">Представляет отдельное сообщение чата в объекте [channel](channel.md) или chat.</span><span class="sxs-lookup"><span data-stu-id="b9213-105">Represents an individual chat message within a [channel](channel.md) or chat entity.</span></span> <span data-ttu-id="b9213-106">Сообщение может быть корневым или частью беседы, определяемой свойством **replyToId** в сообщении.</span><span class="sxs-lookup"><span data-stu-id="b9213-106">The message can be an root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>

## <a name="methods"></a><span data-ttu-id="b9213-107">Методы</span><span class="sxs-lookup"><span data-stu-id="b9213-107">Methods</span></span>

| <span data-ttu-id="b9213-108">Метод</span><span class="sxs-lookup"><span data-stu-id="b9213-108">Method</span></span>       | <span data-ttu-id="b9213-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b9213-109">Return Type</span></span>  |<span data-ttu-id="b9213-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b9213-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b9213-111">Перечисление сообщений в канале</span><span class="sxs-lookup"><span data-stu-id="b9213-111">List Channel messages</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="b9213-112">Коллекция [chatmessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="b9213-112">[chatmessage](chatmessage.md) collection</span></span> | <span data-ttu-id="b9213-113">Получение списка всех корневых сообщений в канале.</span><span class="sxs-lookup"><span data-stu-id="b9213-113">Get the list of all root messages in a channel.</span></span>|
|[<span data-ttu-id="b9213-114">Получение сообщения в канале</span><span class="sxs-lookup"><span data-stu-id="b9213-114">Get Channel message</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="b9213-115">chatmessage</span><span class="sxs-lookup"><span data-stu-id="b9213-115">chatmessage</span></span>](chatmessage.md) | <span data-ttu-id="b9213-116">Получение одного корневого сообщения из канала.</span><span class="sxs-lookup"><span data-stu-id="b9213-116">Get a single root message from a channel.</span></span>|
|[<span data-ttu-id="b9213-117">Перечисление ответов на сообщение</span><span class="sxs-lookup"><span data-stu-id="b9213-117">List replies to a message</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="b9213-118">Коллекция [chatmessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="b9213-118">[chatmessage](chatmessage.md) collection</span></span>| <span data-ttu-id="b9213-119">Получение списка всех ответов на сообщение в канале.</span><span class="sxs-lookup"><span data-stu-id="b9213-119">Get the list of all replies to a message in channel.</span></span>|
|[<span data-ttu-id="b9213-120">Получение ответа на сообщение</span><span class="sxs-lookup"><span data-stu-id="b9213-120">Get a reply to a message</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="b9213-121">chatmessage</span><span class="sxs-lookup"><span data-stu-id="b9213-121">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="b9213-122">Получение одного ответа на сообщение в канале.</span><span class="sxs-lookup"><span data-stu-id="b9213-122">Get a single reply to a message in a channel.</span></span>|
|[<span data-ttu-id="b9213-123">Отправка сообщения в канал</span><span class="sxs-lookup"><span data-stu-id="b9213-123">Send a message in a channel</span></span>](../api/channel-post-chatmessage.md) | [<span data-ttu-id="b9213-124">chatmessage</span><span class="sxs-lookup"><span data-stu-id="b9213-124">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="b9213-125">Создание сообщения верхнего уровня в канале.</span><span class="sxs-lookup"><span data-stu-id="b9213-125">Create a new top-level message in a channel.</span></span>|
|[<span data-ttu-id="b9213-126">Ответ на сообщение в канале</span><span class="sxs-lookup"><span data-stu-id="b9213-126">Reply to a message in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="b9213-127">chatmessage</span><span class="sxs-lookup"><span data-stu-id="b9213-127">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="b9213-128">Ответ на существующее сообщение в канале.</span><span class="sxs-lookup"><span data-stu-id="b9213-128">Reply to an existing message in a channel.</span></span>|


## <a name="properties"></a><span data-ttu-id="b9213-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="b9213-129">Properties</span></span>
| <span data-ttu-id="b9213-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b9213-130">Property</span></span>     | <span data-ttu-id="b9213-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b9213-131">Type</span></span>   |<span data-ttu-id="b9213-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b9213-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b9213-133">id</span><span class="sxs-lookup"><span data-stu-id="b9213-133">id</span></span>|<span data-ttu-id="b9213-134">String</span><span class="sxs-lookup"><span data-stu-id="b9213-134">String</span></span>| <span data-ttu-id="b9213-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b9213-135">Read-only.</span></span> <span data-ttu-id="b9213-136">Уникальный идентификатор сообщения.</span><span class="sxs-lookup"><span data-stu-id="b9213-136">Unique ID of the message.</span></span>|
|<span data-ttu-id="b9213-137">replyToId</span><span class="sxs-lookup"><span data-stu-id="b9213-137">replyToId</span></span>| <span data-ttu-id="b9213-138">string</span><span class="sxs-lookup"><span data-stu-id="b9213-138">string</span></span> | <span data-ttu-id="b9213-139">Идентификатор родительского или корневого сообщения беседы.</span><span class="sxs-lookup"><span data-stu-id="b9213-139">Id of the parent message/root message of the thread.</span></span> |
|<span data-ttu-id="b9213-140">from</span><span class="sxs-lookup"><span data-stu-id="b9213-140">from</span></span>|[<span data-ttu-id="b9213-141">identitySet</span><span class="sxs-lookup"><span data-stu-id="b9213-141">identitySet</span></span>](identityset.md)| <span data-ttu-id="b9213-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b9213-142">Read only.</span></span> <span data-ttu-id="b9213-143">Подробные сведения об отправителе сообщения.</span><span class="sxs-lookup"><span data-stu-id="b9213-143">Details of the sender of the message.</span></span>|
|<span data-ttu-id="b9213-144">etag</span><span class="sxs-lookup"><span data-stu-id="b9213-144">etag</span></span>| <span data-ttu-id="b9213-145">строка</span><span class="sxs-lookup"><span data-stu-id="b9213-145">string</span></span> | <span data-ttu-id="b9213-146">Номер версии сообщения.</span><span class="sxs-lookup"><span data-stu-id="b9213-146">Version number of the message.</span></span> |
|<span data-ttu-id="b9213-147">messageType</span><span class="sxs-lookup"><span data-stu-id="b9213-147">messageType</span></span>|<span data-ttu-id="b9213-148">Строка</span><span class="sxs-lookup"><span data-stu-id="b9213-148">String</span></span>|<span data-ttu-id="b9213-149">Тип сообщения. В настоящее время поддерживаются следующие значения: message, chatEvent, Typing.</span><span class="sxs-lookup"><span data-stu-id="b9213-149">The type of message, current supported values are: message, chatEvent, Typing.</span></span>|
|<span data-ttu-id="b9213-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b9213-150">createdDateTime</span></span>|<span data-ttu-id="b9213-151">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9213-151">dateTimeOffset</span></span>|<span data-ttu-id="b9213-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b9213-152">Read only.</span></span> <span data-ttu-id="b9213-153">Метка времени создания сообщения.</span><span class="sxs-lookup"><span data-stu-id="b9213-153">Timestamp of when the message was created.</span></span>|
|<span data-ttu-id="b9213-154">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b9213-154">lastModifiedDateTime</span></span>|<span data-ttu-id="b9213-155">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9213-155">dateTimeOffset</span></span>|<span data-ttu-id="b9213-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b9213-156">Read only.</span></span> <span data-ttu-id="b9213-157">Метка времени изменения или обновления сообщения.</span><span class="sxs-lookup"><span data-stu-id="b9213-157">Timestamp of when the message was edited/updated.</span></span>|
|<span data-ttu-id="b9213-158">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="b9213-158">deletedDateTime</span></span>|<span data-ttu-id="b9213-159">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9213-159">dateTimeOffset</span></span>|<span data-ttu-id="b9213-160">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b9213-160">Read only.</span></span> <span data-ttu-id="b9213-161">Метка времени, в которое сообщение было удалено, или значение null, если сообщение не было удалено.</span><span class="sxs-lookup"><span data-stu-id="b9213-161">Timestamp at which the message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="b9213-162">subject</span><span class="sxs-lookup"><span data-stu-id="b9213-162">subject</span></span>|<span data-ttu-id="b9213-163">string</span><span class="sxs-lookup"><span data-stu-id="b9213-163">string</span></span>| <span data-ttu-id="b9213-164">Тема сообщения в формате обычного текста.</span><span class="sxs-lookup"><span data-stu-id="b9213-164">The subject of the message.</span></span>|
|<span data-ttu-id="b9213-165">body</span><span class="sxs-lookup"><span data-stu-id="b9213-165">body</span></span>|[<span data-ttu-id="b9213-166">itemBody</span><span class="sxs-lookup"><span data-stu-id="b9213-166">itemBody</span></span>](itembody.md)|<span data-ttu-id="b9213-167">Представление содержимого сообщения в формате Plaintext/HTML.</span><span class="sxs-lookup"><span data-stu-id="b9213-167">Plaintext/HTML representation of the content of the message.</span></span> <span data-ttu-id="b9213-168">По умолчанию содержимое представлено в формате обычного текста.</span><span class="sxs-lookup"><span data-stu-id="b9213-168">By default, the content is in plain text.</span></span> <span data-ttu-id="b9213-169">Приложение может выбрать формат HTML в составе параметров запроса.</span><span class="sxs-lookup"><span data-stu-id="b9213-169">Returns plain text by default, application can choose HTML as part of a query param</span></span> <span data-ttu-id="b9213-170">Содержимое представлено в формате HTML, если сообщение содержит ресурс [chatMessageMention](chatmessagemention.md).</span><span class="sxs-lookup"><span data-stu-id="b9213-170">The content is in HTML if the message contains a [chatMessageMention](chatmessagemention.md).</span></span> |
|<span data-ttu-id="b9213-171">summary</span><span class="sxs-lookup"><span data-stu-id="b9213-171">summary</span></span>|<span data-ttu-id="b9213-172">string</span><span class="sxs-lookup"><span data-stu-id="b9213-172">string</span></span>|<span data-ttu-id="b9213-173">Сводный текст сообщения, который можно использовать для push-уведомлений и представлений сводки или резервных представлений.</span><span class="sxs-lookup"><span data-stu-id="b9213-173">Summary text of the message that could be used for push notifications and summary views or fall back views</span></span>|
|<span data-ttu-id="b9213-174">attachments</span><span class="sxs-lookup"><span data-stu-id="b9213-174">attachments</span></span>|<span data-ttu-id="b9213-175">Коллекция [chatMessageAttachment](chatmessageattachment.md)</span><span class="sxs-lookup"><span data-stu-id="b9213-175">[chatMessageAttachment](chatmessageattachment.md) collection</span></span> |<span data-ttu-id="b9213-176">Вложенные файлы.</span><span class="sxs-lookup"><span data-stu-id="b9213-176">Attached files.</span></span> <span data-ttu-id="b9213-177">В настоящее время вложения доступны только для чтения. Отправка вложений не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9213-177">Attachments are currently read-only – sending attachments is not supported.</span></span> |
|<span data-ttu-id="b9213-178">mentions</span><span class="sxs-lookup"><span data-stu-id="b9213-178">mentions</span></span>|<span data-ttu-id="b9213-179">Коллекция [chatMessageMention](chatmessagemention.md)</span><span class="sxs-lookup"><span data-stu-id="b9213-179">[chatMessageMention](chatmessagemention.md) collection</span></span>| <span data-ttu-id="b9213-180">Список сущностей, упомянутых в сообщении.</span><span class="sxs-lookup"><span data-stu-id="b9213-180">List of entities mentioned in the message.</span></span> <span data-ttu-id="b9213-181">В настоящее время поддерживаются значения user, bot, team и channel.</span><span class="sxs-lookup"><span data-stu-id="b9213-181">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="b9213-182">importance</span><span class="sxs-lookup"><span data-stu-id="b9213-182">importance</span></span>| <span data-ttu-id="b9213-183">строка</span><span class="sxs-lookup"><span data-stu-id="b9213-183">string</span></span> | <span data-ttu-id="b9213-184">Важность сообщения: Normal, High.</span><span class="sxs-lookup"><span data-stu-id="b9213-184">The importance of the message: Normal, High.</span></span>|
|<span data-ttu-id="b9213-185">reactions</span><span class="sxs-lookup"><span data-stu-id="b9213-185">reactions</span></span>| <span data-ttu-id="b9213-186">Коллекция [chatMessageReaction](chatmessagereaction.md)</span><span class="sxs-lookup"><span data-stu-id="b9213-186">[chatMessageReaction](chatmessagereaction.md) collection</span></span> | <span data-ttu-id="b9213-187">Реакции на сообщение (например, "Нравится").</span><span class="sxs-lookup"><span data-stu-id="b9213-187">Reactions for this message (for example, Like)</span></span>|
|<span data-ttu-id="b9213-188">языковые стандарты</span><span class="sxs-lookup"><span data-stu-id="b9213-188">locale</span></span>|<span data-ttu-id="b9213-189">string</span><span class="sxs-lookup"><span data-stu-id="b9213-189">string</span></span>|<span data-ttu-id="b9213-190">Язык сообщения, установленный клиентом.</span><span class="sxs-lookup"><span data-stu-id="b9213-190">Locale of the message set by the client</span></span>|


## <a name="json-representation"></a><span data-ttu-id="b9213-191">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b9213-191">JSON representation</span></span>

<span data-ttu-id="b9213-192">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b9213-192">The following is a JSON representation of the resource.</span></span>

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
