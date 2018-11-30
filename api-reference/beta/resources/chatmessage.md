---
title: Тип ресурса chatMessage
description: Представляет сообщение адресу сущности канала или чата. Сообщение может быть корневой сообщение или частью поток, который определяется свойством **replyToId** в сообщении.
ms.openlocfilehash: 1fba27567d5a1c80a36a5758925ec427735504cf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074938"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="4042c-104">Тип ресурса chatMessage</span><span class="sxs-lookup"><span data-stu-id="4042c-104">chatMessage resource type</span></span>

> <span data-ttu-id="4042c-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4042c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4042c-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4042c-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4042c-107">Представляет сообщение адресу сущности [канала](channel.md) или чата.</span><span class="sxs-lookup"><span data-stu-id="4042c-107">Represents an individual chat message within a [channel](channel.md) or chat entity.</span></span> <span data-ttu-id="4042c-108">Сообщение может быть корневой сообщение или частью поток, который определяется свойством **replyToId** в сообщении.</span><span class="sxs-lookup"><span data-stu-id="4042c-108">The message can be an root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>

## <a name="methods"></a><span data-ttu-id="4042c-109">Методы</span><span class="sxs-lookup"><span data-stu-id="4042c-109">Methods</span></span>

| <span data-ttu-id="4042c-110">Метод</span><span class="sxs-lookup"><span data-stu-id="4042c-110">Method</span></span>       | <span data-ttu-id="4042c-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4042c-111">Return Type</span></span>  |<span data-ttu-id="4042c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="4042c-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4042c-113">Список сообщения</span><span class="sxs-lookup"><span data-stu-id="4042c-113">List Channel messages</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="4042c-114">[chatmessage](chatmessage.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="4042c-114">[chatmessage](chatmessage.md) collection</span></span> | <span data-ttu-id="4042c-115">Получение списка всех сообщений корневой в канал.</span><span class="sxs-lookup"><span data-stu-id="4042c-115">Get the list of all root messages in a channel.</span></span>|
|[<span data-ttu-id="4042c-116">Сообщение канала Get</span><span class="sxs-lookup"><span data-stu-id="4042c-116">Get Channel message</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="4042c-117">chatmessage</span><span class="sxs-lookup"><span data-stu-id="4042c-117">chatmessage</span></span>](chatmessage.md) | <span data-ttu-id="4042c-118">Сообщение один корневой из канала.</span><span class="sxs-lookup"><span data-stu-id="4042c-118">Get a single root message from a channel.</span></span>|
|[<span data-ttu-id="4042c-119">Список ответов на сообщение</span><span class="sxs-lookup"><span data-stu-id="4042c-119">List replies to a message</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="4042c-120">[chatmessage](chatmessage.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="4042c-120">[chatmessage](chatmessage.md) collection</span></span>| <span data-ttu-id="4042c-121">Получение списка всех ответов на сообщение в канала.</span><span class="sxs-lookup"><span data-stu-id="4042c-121">Get the list of all replies to a message in channel.</span></span>|
|[<span data-ttu-id="4042c-122">Получить ответ на сообщение</span><span class="sxs-lookup"><span data-stu-id="4042c-122">Get a reply to a message</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="4042c-123">chatmessage</span><span class="sxs-lookup"><span data-stu-id="4042c-123">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="4042c-124">Получите один ответ на сообщение в канале.</span><span class="sxs-lookup"><span data-stu-id="4042c-124">Get a single reply to a message in a channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="4042c-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="4042c-125">Properties</span></span>
| <span data-ttu-id="4042c-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="4042c-126">Property</span></span>     | <span data-ttu-id="4042c-127">Тип</span><span class="sxs-lookup"><span data-stu-id="4042c-127">Type</span></span>   |<span data-ttu-id="4042c-128">Описание</span><span class="sxs-lookup"><span data-stu-id="4042c-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4042c-129">id</span><span class="sxs-lookup"><span data-stu-id="4042c-129">id</span></span>|<span data-ttu-id="4042c-130">String</span><span class="sxs-lookup"><span data-stu-id="4042c-130">String</span></span>| <span data-ttu-id="4042c-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4042c-131">Read-only.</span></span> <span data-ttu-id="4042c-132">Уникальный идентификатор сообщения.</span><span class="sxs-lookup"><span data-stu-id="4042c-132">Unique ID of the message.</span></span>|
|<span data-ttu-id="4042c-133">replyToId</span><span class="sxs-lookup"><span data-stu-id="4042c-133">replyToId</span></span>| <span data-ttu-id="4042c-134">string</span><span class="sxs-lookup"><span data-stu-id="4042c-134">string</span></span> | <span data-ttu-id="4042c-135">Идентификатор сообщения message/root родительского потока</span><span class="sxs-lookup"><span data-stu-id="4042c-135">Id of the parent message/root message of the thread</span></span> |
|<span data-ttu-id="4042c-136">from</span><span class="sxs-lookup"><span data-stu-id="4042c-136">from</span></span>|[<span data-ttu-id="4042c-137">identitySet</span><span class="sxs-lookup"><span data-stu-id="4042c-137">identitySet</span></span>](identityset.md)| <span data-ttu-id="4042c-138">Сведения о отправитель сообщения</span><span class="sxs-lookup"><span data-stu-id="4042c-138">Details of the sender of the message</span></span>|
|<span data-ttu-id="4042c-139">etag</span><span class="sxs-lookup"><span data-stu-id="4042c-139">etag</span></span>| <span data-ttu-id="4042c-140">string</span><span class="sxs-lookup"><span data-stu-id="4042c-140">string</span></span> | <span data-ttu-id="4042c-141">Номер версии сообщения</span><span class="sxs-lookup"><span data-stu-id="4042c-141">Version number of the message</span></span> |
|<span data-ttu-id="4042c-142">messageType</span><span class="sxs-lookup"><span data-stu-id="4042c-142">messageType</span></span>|<span data-ttu-id="4042c-143">String</span><span class="sxs-lookup"><span data-stu-id="4042c-143">String</span></span>|<span data-ttu-id="4042c-144">Поддерживаемый тип сообщения текущего значения: сообщения, chatEvent, набор</span><span class="sxs-lookup"><span data-stu-id="4042c-144">The type of message, current supported values are: message, chatEvent, Typing</span></span>|
|<span data-ttu-id="4042c-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4042c-145">createdDateTime</span></span>|<span data-ttu-id="4042c-146">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4042c-146">dateTimeOffset</span></span>|<span data-ttu-id="4042c-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4042c-147">Read only.</span></span> <span data-ttu-id="4042c-148">Метка времени создания сообщения</span><span class="sxs-lookup"><span data-stu-id="4042c-148">Timestamp of when the message was created</span></span>|
|<span data-ttu-id="4042c-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4042c-149">lastModifiedDateTime</span></span>|<span data-ttu-id="4042c-150">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4042c-150">dateTimeOffset</span></span>|<span data-ttu-id="4042c-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4042c-151">Read only.</span></span> <span data-ttu-id="4042c-152">Когда сообщение было изменяется обновлено отметки времени</span><span class="sxs-lookup"><span data-stu-id="4042c-152">Timestamp of when the message was edited/updated</span></span>|
|<span data-ttu-id="4042c-153">isDeleted</span><span class="sxs-lookup"><span data-stu-id="4042c-153">isDeleted</span></span>|<span data-ttu-id="4042c-154">boolean</span><span class="sxs-lookup"><span data-stu-id="4042c-154">boolean</span></span>|<span data-ttu-id="4042c-155">Представляет Мягкая удаления сообщения</span><span class="sxs-lookup"><span data-stu-id="4042c-155">Represents if a message has been soft deleted</span></span>|
|<span data-ttu-id="4042c-156">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="4042c-156">deletedDateTime</span></span>|<span data-ttu-id="4042c-157">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4042c-157">dateTimeOffset</span></span>|<span data-ttu-id="4042c-158">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4042c-158">Read only.</span></span> <span data-ttu-id="4042c-159">Метка времени, в котором оно было удалено</span><span class="sxs-lookup"><span data-stu-id="4042c-159">Timestamp at which the message was deleted</span></span> |
|<span data-ttu-id="4042c-160">subject</span><span class="sxs-lookup"><span data-stu-id="4042c-160">subject</span></span>|<span data-ttu-id="4042c-161">строка</span><span class="sxs-lookup"><span data-stu-id="4042c-161">string</span></span>|<span data-ttu-id="4042c-162">Строка темы сообщения.</span><span class="sxs-lookup"><span data-stu-id="4042c-162">Message subject line.</span></span> <span data-ttu-id="4042c-163">Необязательный</span><span class="sxs-lookup"><span data-stu-id="4042c-163">Optional</span></span>|
|<span data-ttu-id="4042c-164">body</span><span class="sxs-lookup"><span data-stu-id="4042c-164">body</span></span>|[<span data-ttu-id="4042c-165">itemBody</span><span class="sxs-lookup"><span data-stu-id="4042c-165">itemBody</span></span>](itembody.md)|<span data-ttu-id="4042c-166">Представление содержимое сообщения в обычный текст или HTML.</span><span class="sxs-lookup"><span data-stu-id="4042c-166">Plaintext/HTML representation of the content of the message.</span></span> <span data-ttu-id="4042c-167">Возвращает обычный текст по умолчанию, приложение может выбрать HTML в составе параметров запроса</span><span class="sxs-lookup"><span data-stu-id="4042c-167">Returns plain text by default, application can choose HTML as part of a query param</span></span>|
|<span data-ttu-id="4042c-168">Сводка</span><span class="sxs-lookup"><span data-stu-id="4042c-168">summary</span></span>|<span data-ttu-id="4042c-169">string</span><span class="sxs-lookup"><span data-stu-id="4042c-169">string</span></span>|<span data-ttu-id="4042c-170">Сводки текста сообщения, которое может использоваться для push-уведомлений и представлений сводок или попадающих обратная представлений</span><span class="sxs-lookup"><span data-stu-id="4042c-170">Summary text of the message that could be used for push notifications and summary views or fall back views</span></span>|
|<span data-ttu-id="4042c-171">упоминания</span><span class="sxs-lookup"><span data-stu-id="4042c-171">mentions</span></span>|<span data-ttu-id="4042c-172">[chatMessageMention](chatmention.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="4042c-172">[chatMessageMention](chatmention.md) collection</span></span>| <span data-ttu-id="4042c-173">Список сущностей, упомянутые в сообщении.</span><span class="sxs-lookup"><span data-stu-id="4042c-173">List of entities mentioned in the message.</span></span> <span data-ttu-id="4042c-174">В настоящее время поддерживает пользователя, программа-робот, группы, канала</span><span class="sxs-lookup"><span data-stu-id="4042c-174">Currently supports user, bot, team, channel</span></span>|
|<span data-ttu-id="4042c-175">importance</span><span class="sxs-lookup"><span data-stu-id="4042c-175">importance</span></span>| <span data-ttu-id="4042c-176">string</span><span class="sxs-lookup"><span data-stu-id="4042c-176">string</span></span> | <span data-ttu-id="4042c-177">Важность сообщения: обычный, высокая</span><span class="sxs-lookup"><span data-stu-id="4042c-177">The importance of the message: Normal, High</span></span>|
|<span data-ttu-id="4042c-178">реакции</span><span class="sxs-lookup"><span data-stu-id="4042c-178">reactions</span></span>| <span data-ttu-id="4042c-179">[chatMessageReaction](chatreaction.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="4042c-179">[chatMessageReaction](chatreaction.md) collection</span></span> | <span data-ttu-id="4042c-180">Реакции для данного сообщения (например, например)</span><span class="sxs-lookup"><span data-stu-id="4042c-180">Reactions for this message (for example, Like)</span></span>|
|<span data-ttu-id="4042c-181">locale</span><span class="sxs-lookup"><span data-stu-id="4042c-181">locale</span></span>|<span data-ttu-id="4042c-182">string</span><span class="sxs-lookup"><span data-stu-id="4042c-182">string</span></span>|<span data-ttu-id="4042c-183">Языковой стандарт сообщения, заданный клиентом</span><span class="sxs-lookup"><span data-stu-id="4042c-183">Locale of the message set by the client</span></span>|
|<span data-ttu-id="4042c-184">attachments</span><span class="sxs-lookup"><span data-stu-id="4042c-184">attachments</span></span>|<span data-ttu-id="4042c-185">[chatMessageAttachment](chatattachment.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="4042c-185">[chatMessageAttachment](chatattachment.md) collection</span></span> |<span data-ttu-id="4042c-186">Вложенные файлы</span><span class="sxs-lookup"><span data-stu-id="4042c-186">Attached files</span></span>|


## <a name="json-representation"></a><span data-ttu-id="4042c-187">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4042c-187">JSON representation</span></span>

<span data-ttu-id="4042c-188">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4042c-188">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "isDeleted",
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
<!-- {
  "type": "#page.annotation",
  "description": "chat message resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
