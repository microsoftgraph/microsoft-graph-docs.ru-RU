---
title: Тип ресурса chatMessage
description: Представляет сообщение адресу сущности канала или чата. Сообщение может быть корневой сообщение или частью поток, который определяется свойством **replyToId** в сообщении.
localization_priority: Priority
ms.openlocfilehash: ad381102f7e93a4dcccd7b68435d0687ed6b4837
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855995"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="fa056-104">Тип ресурса chatMessage</span><span class="sxs-lookup"><span data-stu-id="fa056-104">chatMessage resource type</span></span>

> <span data-ttu-id="fa056-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fa056-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fa056-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa056-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fa056-107">Представляет сообщение адресу сущности [канала](channel.md) или чата.</span><span class="sxs-lookup"><span data-stu-id="fa056-107">Represents an individual chat message within a [channel](channel.md) or chat entity.</span></span> <span data-ttu-id="fa056-108">Сообщение может быть корневой сообщение или частью поток, который определяется свойством **replyToId** в сообщении.</span><span class="sxs-lookup"><span data-stu-id="fa056-108">The message can be an root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>

## <a name="methods"></a><span data-ttu-id="fa056-109">Методы</span><span class="sxs-lookup"><span data-stu-id="fa056-109">Methods</span></span>

| <span data-ttu-id="fa056-110">Метод</span><span class="sxs-lookup"><span data-stu-id="fa056-110">Method</span></span>       | <span data-ttu-id="fa056-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fa056-111">Return Type</span></span>  |<span data-ttu-id="fa056-112">Описание</span><span class="sxs-lookup"><span data-stu-id="fa056-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fa056-113">Список сообщения</span><span class="sxs-lookup"><span data-stu-id="fa056-113">List Channel messages</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="fa056-114">[chatmessage](chatmessage.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="fa056-114">[chatmessage](chatmessage.md) collection</span></span> | <span data-ttu-id="fa056-115">Получение списка всех сообщений корневой в канал.</span><span class="sxs-lookup"><span data-stu-id="fa056-115">Get the list of all root messages in a channel.</span></span>|
|[<span data-ttu-id="fa056-116">Сообщение канала Get</span><span class="sxs-lookup"><span data-stu-id="fa056-116">Get Channel message</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="fa056-117">chatmessage</span><span class="sxs-lookup"><span data-stu-id="fa056-117">chatmessage</span></span>](chatmessage.md) | <span data-ttu-id="fa056-118">Сообщение один корневой из канала.</span><span class="sxs-lookup"><span data-stu-id="fa056-118">Get a single root message from a channel.</span></span>|
|[<span data-ttu-id="fa056-119">Список ответов на сообщение</span><span class="sxs-lookup"><span data-stu-id="fa056-119">List replies to a message</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="fa056-120">[chatmessage](chatmessage.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="fa056-120">[chatmessage](chatmessage.md) collection</span></span>| <span data-ttu-id="fa056-121">Получение списка всех ответов на сообщение в канала.</span><span class="sxs-lookup"><span data-stu-id="fa056-121">Get the list of all replies to a message in channel.</span></span>|
|[<span data-ttu-id="fa056-122">Получить ответ на сообщение</span><span class="sxs-lookup"><span data-stu-id="fa056-122">Get a reply to a message</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="fa056-123">chatmessage</span><span class="sxs-lookup"><span data-stu-id="fa056-123">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="fa056-124">Получите один ответ на сообщение в канале.</span><span class="sxs-lookup"><span data-stu-id="fa056-124">Get a single reply to a message in a channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="fa056-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="fa056-125">Properties</span></span>
| <span data-ttu-id="fa056-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="fa056-126">Property</span></span>     | <span data-ttu-id="fa056-127">Тип</span><span class="sxs-lookup"><span data-stu-id="fa056-127">Type</span></span>   |<span data-ttu-id="fa056-128">Описание</span><span class="sxs-lookup"><span data-stu-id="fa056-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fa056-129">id</span><span class="sxs-lookup"><span data-stu-id="fa056-129">id</span></span>|<span data-ttu-id="fa056-130">Строка</span><span class="sxs-lookup"><span data-stu-id="fa056-130">String</span></span>| <span data-ttu-id="fa056-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fa056-131">Read-only.</span></span> <span data-ttu-id="fa056-132">Уникальный идентификатор сообщения.</span><span class="sxs-lookup"><span data-stu-id="fa056-132">Unique ID of the message.</span></span>|
|<span data-ttu-id="fa056-133">replyToId</span><span class="sxs-lookup"><span data-stu-id="fa056-133">replyToId</span></span>| <span data-ttu-id="fa056-134">string</span><span class="sxs-lookup"><span data-stu-id="fa056-134">string</span></span> | <span data-ttu-id="fa056-135">Идентификатор сообщения message/root родительского потока</span><span class="sxs-lookup"><span data-stu-id="fa056-135">Id of the parent message/root message of the thread</span></span> |
|<span data-ttu-id="fa056-136">from</span><span class="sxs-lookup"><span data-stu-id="fa056-136">from</span></span>|[<span data-ttu-id="fa056-137">identitySet</span><span class="sxs-lookup"><span data-stu-id="fa056-137">identitySet</span></span>](identityset.md)| <span data-ttu-id="fa056-138">Сведения о отправитель сообщения</span><span class="sxs-lookup"><span data-stu-id="fa056-138">Details of the sender of the message</span></span>|
|<span data-ttu-id="fa056-139">etag</span><span class="sxs-lookup"><span data-stu-id="fa056-139">etag</span></span>| <span data-ttu-id="fa056-140">string</span><span class="sxs-lookup"><span data-stu-id="fa056-140">string</span></span> | <span data-ttu-id="fa056-141">Номер версии сообщения</span><span class="sxs-lookup"><span data-stu-id="fa056-141">Version number of the message</span></span> |
|<span data-ttu-id="fa056-142">messageType</span><span class="sxs-lookup"><span data-stu-id="fa056-142">messageType</span></span>|<span data-ttu-id="fa056-143">Строка</span><span class="sxs-lookup"><span data-stu-id="fa056-143">String</span></span>|<span data-ttu-id="fa056-144">Поддерживаемый тип сообщения текущего значения: сообщения, chatEvent, набор</span><span class="sxs-lookup"><span data-stu-id="fa056-144">The type of message, current supported values are: message, chatEvent, Typing</span></span>|
|<span data-ttu-id="fa056-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fa056-145">createdDateTime</span></span>|<span data-ttu-id="fa056-146">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa056-146">dateTimeOffset</span></span>|<span data-ttu-id="fa056-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fa056-147">Read only.</span></span> <span data-ttu-id="fa056-148">Метка времени создания сообщения</span><span class="sxs-lookup"><span data-stu-id="fa056-148">Timestamp of when the message was created</span></span>|
|<span data-ttu-id="fa056-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fa056-149">lastModifiedDateTime</span></span>|<span data-ttu-id="fa056-150">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa056-150">dateTimeOffset</span></span>|<span data-ttu-id="fa056-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fa056-151">Read only.</span></span> <span data-ttu-id="fa056-152">Когда сообщение было изменяется обновлено отметки времени</span><span class="sxs-lookup"><span data-stu-id="fa056-152">Timestamp of when the message was edited/updated</span></span>|
|<span data-ttu-id="fa056-153">isDeleted</span><span class="sxs-lookup"><span data-stu-id="fa056-153">isDeleted</span></span>|<span data-ttu-id="fa056-154">boolean</span><span class="sxs-lookup"><span data-stu-id="fa056-154">boolean</span></span>|<span data-ttu-id="fa056-155">Представляет Мягкая удаления сообщения</span><span class="sxs-lookup"><span data-stu-id="fa056-155">Represents if a message has been soft deleted</span></span>|
|<span data-ttu-id="fa056-156">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="fa056-156">deletedDateTime</span></span>|<span data-ttu-id="fa056-157">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa056-157">dateTimeOffset</span></span>|<span data-ttu-id="fa056-158">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fa056-158">Read only.</span></span> <span data-ttu-id="fa056-159">Метка времени, в котором оно было удалено</span><span class="sxs-lookup"><span data-stu-id="fa056-159">Timestamp at which the message was deleted</span></span> |
|<span data-ttu-id="fa056-160">subject</span><span class="sxs-lookup"><span data-stu-id="fa056-160">subject</span></span>|<span data-ttu-id="fa056-161">строка</span><span class="sxs-lookup"><span data-stu-id="fa056-161">string</span></span>|<span data-ttu-id="fa056-162">Строка темы сообщения.</span><span class="sxs-lookup"><span data-stu-id="fa056-162">Message subject line.</span></span> <span data-ttu-id="fa056-163">Необязательный</span><span class="sxs-lookup"><span data-stu-id="fa056-163">Optional</span></span>|
|<span data-ttu-id="fa056-164">body</span><span class="sxs-lookup"><span data-stu-id="fa056-164">body</span></span>|[<span data-ttu-id="fa056-165">itemBody</span><span class="sxs-lookup"><span data-stu-id="fa056-165">itemBody</span></span>](itembody.md)|<span data-ttu-id="fa056-166">Представление содержимое сообщения в обычный текст или HTML.</span><span class="sxs-lookup"><span data-stu-id="fa056-166">Plaintext/HTML representation of the content of the message.</span></span> <span data-ttu-id="fa056-167">Возвращает обычный текст по умолчанию, приложение может выбрать HTML в составе параметров запроса</span><span class="sxs-lookup"><span data-stu-id="fa056-167">Returns plain text by default, application can choose HTML as part of a query param</span></span>|
|<span data-ttu-id="fa056-168">Сводка</span><span class="sxs-lookup"><span data-stu-id="fa056-168">summary</span></span>|<span data-ttu-id="fa056-169">string</span><span class="sxs-lookup"><span data-stu-id="fa056-169">string</span></span>|<span data-ttu-id="fa056-170">Сводки текста сообщения, которое может использоваться для push-уведомлений и представлений сводок или попадающих обратная представлений</span><span class="sxs-lookup"><span data-stu-id="fa056-170">Summary text of the message that could be used for push notifications and summary views or fall back views</span></span>|
|<span data-ttu-id="fa056-171">упоминания</span><span class="sxs-lookup"><span data-stu-id="fa056-171">mentions</span></span>|<span data-ttu-id="fa056-172">[chatMessageMention](chatmention.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="fa056-172">[chatMessageMention](chatmention.md) collection</span></span>| <span data-ttu-id="fa056-173">Список сущностей, упомянутые в сообщении.</span><span class="sxs-lookup"><span data-stu-id="fa056-173">List of entities mentioned in the message.</span></span> <span data-ttu-id="fa056-174">В настоящее время поддерживает пользователя, программа-робот, группы, канала</span><span class="sxs-lookup"><span data-stu-id="fa056-174">Currently supports user, bot, team, channel</span></span>|
|<span data-ttu-id="fa056-175">importance</span><span class="sxs-lookup"><span data-stu-id="fa056-175">importance</span></span>| <span data-ttu-id="fa056-176">string</span><span class="sxs-lookup"><span data-stu-id="fa056-176">string</span></span> | <span data-ttu-id="fa056-177">Важность сообщения: обычный, высокая</span><span class="sxs-lookup"><span data-stu-id="fa056-177">The importance of the message: Normal, High</span></span>|
|<span data-ttu-id="fa056-178">реакции</span><span class="sxs-lookup"><span data-stu-id="fa056-178">reactions</span></span>| <span data-ttu-id="fa056-179">[chatMessageReaction](chatreaction.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="fa056-179">[chatMessageReaction](chatreaction.md) collection</span></span> | <span data-ttu-id="fa056-180">Реакции для данного сообщения (например, например)</span><span class="sxs-lookup"><span data-stu-id="fa056-180">Reactions for this message (for example, Like)</span></span>|
|<span data-ttu-id="fa056-181">locale</span><span class="sxs-lookup"><span data-stu-id="fa056-181">locale</span></span>|<span data-ttu-id="fa056-182">string</span><span class="sxs-lookup"><span data-stu-id="fa056-182">string</span></span>|<span data-ttu-id="fa056-183">Языковой стандарт сообщения, заданный клиентом</span><span class="sxs-lookup"><span data-stu-id="fa056-183">Locale of the message set by the client</span></span>|
|<span data-ttu-id="fa056-184">attachments</span><span class="sxs-lookup"><span data-stu-id="fa056-184">attachments</span></span>|<span data-ttu-id="fa056-185">[chatMessageAttachment](chatattachment.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="fa056-185">[chatMessageAttachment](chatattachment.md) collection</span></span> |<span data-ttu-id="fa056-186">Вложенные файлы</span><span class="sxs-lookup"><span data-stu-id="fa056-186">Attached files</span></span>|


## <a name="json-representation"></a><span data-ttu-id="fa056-187">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fa056-187">JSON representation</span></span>

<span data-ttu-id="fa056-188">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fa056-188">The following is a JSON representation of the resource.</span></span>

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
