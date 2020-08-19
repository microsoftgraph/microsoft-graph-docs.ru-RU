---
title: Тип ресурса chatMessage
description: Представляет отдельное сообщение чата в объекте channel или chat. Сообщение чата может быть корневым сообщением чата или частью потока, определенного свойством **реплитоид** в сообщении чата.
doc_type: resourcePageType
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 2b5c06b8b664c10483c8d4a6767a981f1a5551be
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812346"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="7c2b8-104">Тип ресурса chatMessage</span><span class="sxs-lookup"><span data-stu-id="7c2b8-104">chatMessage resource type</span></span>

<span data-ttu-id="7c2b8-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c2b8-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7c2b8-106">Представляет отдельное сообщение чата в [беседе](/graph/api/resources/chat?view=graph-rest-beta)по [каналу](./channel.md) или (в бета-версии).</span><span class="sxs-lookup"><span data-stu-id="7c2b8-106">Represents an individual chat message within a [channel](./channel.md) or (in beta) [chat](/graph/api/resources/chat?view=graph-rest-beta).</span></span> <span data-ttu-id="7c2b8-107">Сообщение чата может быть корневым сообщением чата или частью ответа, которое определяется свойством **реплитоид** в сообщении чата.</span><span class="sxs-lookup"><span data-stu-id="7c2b8-107">The chat message can be a root chat message or part of a reply thread that is defined by the **replyToId** property in the chat message.</span></span>

## <a name="methods"></a><span data-ttu-id="7c2b8-108">Методы</span><span class="sxs-lookup"><span data-stu-id="7c2b8-108">Methods</span></span>

| <span data-ttu-id="7c2b8-109">Метод</span><span class="sxs-lookup"><span data-stu-id="7c2b8-109">Method</span></span>       | <span data-ttu-id="7c2b8-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7c2b8-110">Return Type</span></span>  |<span data-ttu-id="7c2b8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7c2b8-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7c2b8-112">**Сообщения канала**</span><span class="sxs-lookup"><span data-stu-id="7c2b8-112">**Channel messages**</span></span>| | |
|[<span data-ttu-id="7c2b8-113">Создание объекта chatMessage в канале</span><span class="sxs-lookup"><span data-stu-id="7c2b8-113">Create chatMessage in a channel</span></span>](../api/channel-post-messages.md) | [<span data-ttu-id="7c2b8-114">chatMessage</span><span class="sxs-lookup"><span data-stu-id="7c2b8-114">chatMessage</span></span>](#chatmessage-resource-type)| <span data-ttu-id="7c2b8-115">Создайте новое сообщение разговора верхнего уровня в канале.</span><span class="sxs-lookup"><span data-stu-id="7c2b8-115">Create a new top-level chat message in a channel.</span></span>|
|<span data-ttu-id="7c2b8-116">**Ответы на сообщения канала**</span><span class="sxs-lookup"><span data-stu-id="7c2b8-116">**Channel message replies**</span></span>| | |
|[<span data-ttu-id="7c2b8-117">Ответ на chatMessage в канале</span><span class="sxs-lookup"><span data-stu-id="7c2b8-117">Reply to a chatMessage in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="7c2b8-118">chatMessage</span><span class="sxs-lookup"><span data-stu-id="7c2b8-118">chatMessage</span></span>](#chatmessage-resource-type)| <span data-ttu-id="7c2b8-119">Ответ на существующее сообщение чата в канале.</span><span class="sxs-lookup"><span data-stu-id="7c2b8-119">Reply to an existing chat message in a channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="7c2b8-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="7c2b8-120">Properties</span></span>

| <span data-ttu-id="7c2b8-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="7c2b8-121">Property</span></span>   | <span data-ttu-id="7c2b8-122">Тип</span><span class="sxs-lookup"><span data-stu-id="7c2b8-122">Type</span></span> |<span data-ttu-id="7c2b8-123">Описание</span><span class="sxs-lookup"><span data-stu-id="7c2b8-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7c2b8-124">id</span><span class="sxs-lookup"><span data-stu-id="7c2b8-124">id</span></span>|<span data-ttu-id="7c2b8-125">String</span><span class="sxs-lookup"><span data-stu-id="7c2b8-125">String</span></span>| <span data-ttu-id="7c2b8-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7c2b8-126">Read-only.</span></span> <span data-ttu-id="7c2b8-127">Уникальный идентификатор сообщения.</span><span class="sxs-lookup"><span data-stu-id="7c2b8-127">Unique Id of the message.</span></span>|
|<span data-ttu-id="7c2b8-128">replyToId</span><span class="sxs-lookup"><span data-stu-id="7c2b8-128">replyToId</span></span>| <span data-ttu-id="7c2b8-129">string</span><span class="sxs-lookup"><span data-stu-id="7c2b8-129">string</span></span> | <span data-ttu-id="7c2b8-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7c2b8-130">Read-only.</span></span> <span data-ttu-id="7c2b8-131">Идентификатор родительского сообщения чата или сообщения корневого сеанса беседы в цепочке.</span><span class="sxs-lookup"><span data-stu-id="7c2b8-131">Id of the parent chat message or root chat message of the thread.</span></span> <span data-ttu-id="7c2b8-132">(Применяется только к сообщениям чата в каналах без чатов)</span><span class="sxs-lookup"><span data-stu-id="7c2b8-132">(Only applies to chat messages in channels not chats)</span></span> |
|<span data-ttu-id="7c2b8-133">from</span><span class="sxs-lookup"><span data-stu-id="7c2b8-133">from</span></span>|[<span data-ttu-id="7c2b8-134">identitySet</span><span class="sxs-lookup"><span data-stu-id="7c2b8-134">identitySet</span></span>](identityset.md)| <span data-ttu-id="7c2b8-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7c2b8-135">Read only.</span></span> <span data-ttu-id="7c2b8-136">Сведения об отправителе сообщения чата.</span><span class="sxs-lookup"><span data-stu-id="7c2b8-136">Details of the sender of the chat message.</span></span>|
|<span data-ttu-id="7c2b8-137">etag</span><span class="sxs-lookup"><span data-stu-id="7c2b8-137">etag</span></span>| <span data-ttu-id="7c2b8-138">string</span><span class="sxs-lookup"><span data-stu-id="7c2b8-138">string</span></span> | <span data-ttu-id="7c2b8-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7c2b8-139">Read-only.</span></span> <span data-ttu-id="7c2b8-140">Номер версии сообщения чата.</span><span class="sxs-lookup"><span data-stu-id="7c2b8-140">Version number of the chat message.</span></span> |
|<span data-ttu-id="7c2b8-141">messageType</span><span class="sxs-lookup"><span data-stu-id="7c2b8-141">messageType</span></span>|<span data-ttu-id="7c2b8-142">string</span><span class="sxs-lookup"><span data-stu-id="7c2b8-142">string</span></span>|<span data-ttu-id="7c2b8-143">Тип сообщения чата.</span><span class="sxs-lookup"><span data-stu-id="7c2b8-143">The type of chat message.</span></span> <span data-ttu-id="7c2b8-144">Возможные значения: `message` .</span><span class="sxs-lookup"><span data-stu-id="7c2b8-144">The possible values are: `message`.</span></span>|
|<span data-ttu-id="7c2b8-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7c2b8-145">createdDateTime</span></span>|<span data-ttu-id="7c2b8-146">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c2b8-146">dateTimeOffset</span></span>|<span data-ttu-id="7c2b8-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7c2b8-147">Read only.</span></span> <span data-ttu-id="7c2b8-148">Метка времени создания сообщения чата.</span><span class="sxs-lookup"><span data-stu-id="7c2b8-148">Timestamp of when the chat message was created.</span></span>|
|<span data-ttu-id="7c2b8-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7c2b8-149">lastModifiedDateTime</span></span>|<span data-ttu-id="7c2b8-150">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c2b8-150">dateTimeOffset</span></span>|<span data-ttu-id="7c2b8-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7c2b8-151">Read only.</span></span> <span data-ttu-id="7c2b8-152">Метка времени создания или изменения сообщения чата, в том числе когда выполняется ответ (если он является корневым сообщением в канале) или добавляется или удаляется реакция.</span><span class="sxs-lookup"><span data-stu-id="7c2b8-152">Timestamp of when the chat message is created or edited, including when a reply is made (if it's a root chat message in a channel) or a reaction is added or removed.</span></span> |
|<span data-ttu-id="7c2b8-153">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="7c2b8-153">deletedDateTime</span></span>|<span data-ttu-id="7c2b8-154">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c2b8-154">dateTimeOffset</span></span>|<span data-ttu-id="7c2b8-155">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7c2b8-155">Read only.</span></span> <span data-ttu-id="7c2b8-156">Временная метка, в которой сообщение чата удалено, или значение null, если оно не удалено.</span><span class="sxs-lookup"><span data-stu-id="7c2b8-156">Timestamp at which the chat message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="7c2b8-157">subject</span><span class="sxs-lookup"><span data-stu-id="7c2b8-157">subject</span></span>|<span data-ttu-id="7c2b8-158">string</span><span class="sxs-lookup"><span data-stu-id="7c2b8-158">string</span></span>| <span data-ttu-id="7c2b8-159">Тема сообщения чата в виде открытого текста.</span><span class="sxs-lookup"><span data-stu-id="7c2b8-159">The subject of the chat message, in plaintext.</span></span>|
|<span data-ttu-id="7c2b8-160">body</span><span class="sxs-lookup"><span data-stu-id="7c2b8-160">body</span></span>|[<span data-ttu-id="7c2b8-161">itemBody</span><span class="sxs-lookup"><span data-stu-id="7c2b8-161">itemBody</span></span>](itembody.md)|<span data-ttu-id="7c2b8-162">Представление содержимого сообщения чата в формате обычного текста или в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="7c2b8-162">Plaintext/HTML representation of the content of the chat message.</span></span> <span data-ttu-id="7c2b8-163">Представление определяется параметром contentType в тексте.</span><span class="sxs-lookup"><span data-stu-id="7c2b8-163">Representation is specified by the contentType inside the body.</span></span> <span data-ttu-id="7c2b8-164">Если сообщение чата содержит [чатмессажементион](chatmessagemention.md), содержимое всегда находится в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="7c2b8-164">The content is always in HTML if the chat message contains a [chatMessageMention](chatmessagemention.md).</span></span> |
|<span data-ttu-id="7c2b8-165">summary</span><span class="sxs-lookup"><span data-stu-id="7c2b8-165">summary</span></span>|<span data-ttu-id="7c2b8-166">string</span><span class="sxs-lookup"><span data-stu-id="7c2b8-166">string</span></span>| <span data-ttu-id="7c2b8-167">Сводный текст сообщения чата, которое можно использовать для push-уведомлений и сводных представлений, а также для обратного просмотра.</span><span class="sxs-lookup"><span data-stu-id="7c2b8-167">Summary text of the chat message that could be used for push notifications and summary views or fall back views.</span></span> <span data-ttu-id="7c2b8-168">Применяется только к сообщениям разговора по каналу, а не к сообщениям в чате.</span><span class="sxs-lookup"><span data-stu-id="7c2b8-168">Only applies to channel chat messages, not chat messages in a chat.</span></span> |
|<span data-ttu-id="7c2b8-169">attachments</span><span class="sxs-lookup"><span data-stu-id="7c2b8-169">attachments</span></span>|<span data-ttu-id="7c2b8-170">Коллекция [chatMessageAttachment](chatmessageattachment.md)</span><span class="sxs-lookup"><span data-stu-id="7c2b8-170">[chatMessageAttachment](chatmessageattachment.md) collection</span></span> |<span data-ttu-id="7c2b8-171">Вложенные файлы.</span><span class="sxs-lookup"><span data-stu-id="7c2b8-171">Attached files.</span></span> <span data-ttu-id="7c2b8-172">В настоящее время вложения доступны только для чтения. Отправка вложений не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c2b8-172">Attachments are currently read-only – sending attachments is not supported.</span></span> |
|<span data-ttu-id="7c2b8-173">mentions</span><span class="sxs-lookup"><span data-stu-id="7c2b8-173">mentions</span></span>|<span data-ttu-id="7c2b8-174">Коллекция [chatMessageMention](chatmessagemention.md)</span><span class="sxs-lookup"><span data-stu-id="7c2b8-174">[chatMessageMention](chatmessagemention.md) collection</span></span>| <span data-ttu-id="7c2b8-175">Список сущностей, упоминаемых в сообщении чата.</span><span class="sxs-lookup"><span data-stu-id="7c2b8-175">List of entities mentioned in the chat message.</span></span> <span data-ttu-id="7c2b8-176">В настоящее время поддерживаются значения user, bot, team и channel.</span><span class="sxs-lookup"><span data-stu-id="7c2b8-176">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="7c2b8-177">importance</span><span class="sxs-lookup"><span data-stu-id="7c2b8-177">importance</span></span>| <span data-ttu-id="7c2b8-178">string</span><span class="sxs-lookup"><span data-stu-id="7c2b8-178">string</span></span> | <span data-ttu-id="7c2b8-179">Важность сообщения чата.</span><span class="sxs-lookup"><span data-stu-id="7c2b8-179">The importance of the chat message.</span></span> <span data-ttu-id="7c2b8-180">Допустимые значения: `normal`, `high`, `urgent`.</span><span class="sxs-lookup"><span data-stu-id="7c2b8-180">The possible values are: `normal`, `high`, `urgent`.</span></span>|
|<span data-ttu-id="7c2b8-181">языковые стандарты</span><span class="sxs-lookup"><span data-stu-id="7c2b8-181">locale</span></span>|<span data-ttu-id="7c2b8-182">string</span><span class="sxs-lookup"><span data-stu-id="7c2b8-182">string</span></span>|<span data-ttu-id="7c2b8-183">Язык сообщения чата, заданное клиентом.</span><span class="sxs-lookup"><span data-stu-id="7c2b8-183">Locale of the chat message set by the client.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7c2b8-184">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7c2b8-184">JSON representation</span></span>

<span data-ttu-id="7c2b8-185">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7c2b8-185">The following is a JSON representation of the resource.</span></span>

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
