---
title: Тип ресурса chatMessage
description: Представляет отдельное сообщение чата в объекте channel или chat. Сообщение чата может быть корневым сообщением чата или частью потока, определенного свойством **реплитоид** в сообщении чата.
doc_type: resourcePageType
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: af025ad2484757626fec08d9131a870cb345e492
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223214"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="60187-104">Тип ресурса chatMessage</span><span class="sxs-lookup"><span data-stu-id="60187-104">chatMessage resource type</span></span>

<span data-ttu-id="60187-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60187-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="60187-106">Представляет отдельное сообщение чата в [беседе](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true)по [каналу](./channel.md) или (в бета-версии).</span><span class="sxs-lookup"><span data-stu-id="60187-106">Represents an individual chat message within a [channel](./channel.md) or (in beta) [chat](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true).</span></span> <span data-ttu-id="60187-107">Сообщение чата может быть корневым сообщением чата или частью ответа, которое определяется свойством **реплитоид** в сообщении чата.</span><span class="sxs-lookup"><span data-stu-id="60187-107">The chat message can be a root chat message or part of a reply thread that is defined by the **replyToId** property in the chat message.</span></span>

## <a name="methods"></a><span data-ttu-id="60187-108">Методы</span><span class="sxs-lookup"><span data-stu-id="60187-108">Methods</span></span>

| <span data-ttu-id="60187-109">Метод</span><span class="sxs-lookup"><span data-stu-id="60187-109">Method</span></span>       | <span data-ttu-id="60187-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="60187-110">Return Type</span></span>  |<span data-ttu-id="60187-111">Описание</span><span class="sxs-lookup"><span data-stu-id="60187-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="60187-112">**Сообщения канала**</span><span class="sxs-lookup"><span data-stu-id="60187-112">**Channel messages**</span></span>| | |
|[<span data-ttu-id="60187-113">Создание объекта chatMessage в канале</span><span class="sxs-lookup"><span data-stu-id="60187-113">Create chatMessage in a channel</span></span>](../api/channel-post-messages.md) | [<span data-ttu-id="60187-114">chatMessage</span><span class="sxs-lookup"><span data-stu-id="60187-114">chatMessage</span></span>](#chatmessage-resource-type)| <span data-ttu-id="60187-115">Создайте новое сообщение разговора верхнего уровня в канале.</span><span class="sxs-lookup"><span data-stu-id="60187-115">Create a new top-level chat message in a channel.</span></span>|
|[<span data-ttu-id="60187-116">Обновление chatMessage</span><span class="sxs-lookup"><span data-stu-id="60187-116">Update chatMessage</span></span>](../api/chatmessage-update.md)|[<span data-ttu-id="60187-117">chatMessage</span><span class="sxs-lookup"><span data-stu-id="60187-117">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="60187-118">Обновление свойства **полицивиолатион** сообщения чата.</span><span class="sxs-lookup"><span data-stu-id="60187-118">Update the **policyViolation** property of a chat message.</span></span>|
|<span data-ttu-id="60187-119">**Ответы на сообщения канала**</span><span class="sxs-lookup"><span data-stu-id="60187-119">**Channel message replies**</span></span>| | |
|[<span data-ttu-id="60187-120">Ответ на chatMessage в канале</span><span class="sxs-lookup"><span data-stu-id="60187-120">Reply to a chatMessage in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="60187-121">chatMessage</span><span class="sxs-lookup"><span data-stu-id="60187-121">chatMessage</span></span>](#chatmessage-resource-type)| <span data-ttu-id="60187-122">Ответ на существующее сообщение чата в канале.</span><span class="sxs-lookup"><span data-stu-id="60187-122">Reply to an existing chat message in a channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="60187-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="60187-123">Properties</span></span>

| <span data-ttu-id="60187-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="60187-124">Property</span></span>   | <span data-ttu-id="60187-125">Тип</span><span class="sxs-lookup"><span data-stu-id="60187-125">Type</span></span> |<span data-ttu-id="60187-126">Описание</span><span class="sxs-lookup"><span data-stu-id="60187-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="60187-127">id</span><span class="sxs-lookup"><span data-stu-id="60187-127">id</span></span>|<span data-ttu-id="60187-128">String</span><span class="sxs-lookup"><span data-stu-id="60187-128">String</span></span>| <span data-ttu-id="60187-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="60187-129">Read-only.</span></span> <span data-ttu-id="60187-130">Уникальный идентификатор сообщения.</span><span class="sxs-lookup"><span data-stu-id="60187-130">Unique Id of the message.</span></span>|
|<span data-ttu-id="60187-131">replyToId</span><span class="sxs-lookup"><span data-stu-id="60187-131">replyToId</span></span>| <span data-ttu-id="60187-132">string</span><span class="sxs-lookup"><span data-stu-id="60187-132">string</span></span> | <span data-ttu-id="60187-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="60187-133">Read-only.</span></span> <span data-ttu-id="60187-134">Идентификатор родительского сообщения чата или сообщения корневого сеанса беседы в цепочке.</span><span class="sxs-lookup"><span data-stu-id="60187-134">Id of the parent chat message or root chat message of the thread.</span></span> <span data-ttu-id="60187-135">(Применяется только к сообщениям чата в каналах без чатов)</span><span class="sxs-lookup"><span data-stu-id="60187-135">(Only applies to chat messages in channels not chats)</span></span> |
|<span data-ttu-id="60187-136">from</span><span class="sxs-lookup"><span data-stu-id="60187-136">from</span></span>|[<span data-ttu-id="60187-137">identitySet</span><span class="sxs-lookup"><span data-stu-id="60187-137">identitySet</span></span>](identityset.md)| <span data-ttu-id="60187-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="60187-138">Read only.</span></span> <span data-ttu-id="60187-139">Сведения об отправителе сообщения чата.</span><span class="sxs-lookup"><span data-stu-id="60187-139">Details of the sender of the chat message.</span></span>|
|<span data-ttu-id="60187-140">etag</span><span class="sxs-lookup"><span data-stu-id="60187-140">etag</span></span>| <span data-ttu-id="60187-141">string</span><span class="sxs-lookup"><span data-stu-id="60187-141">string</span></span> | <span data-ttu-id="60187-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="60187-142">Read-only.</span></span> <span data-ttu-id="60187-143">Номер версии сообщения чата.</span><span class="sxs-lookup"><span data-stu-id="60187-143">Version number of the chat message.</span></span> |
|<span data-ttu-id="60187-144">messageType</span><span class="sxs-lookup"><span data-stu-id="60187-144">messageType</span></span>|<span data-ttu-id="60187-145">string</span><span class="sxs-lookup"><span data-stu-id="60187-145">string</span></span>|<span data-ttu-id="60187-146">Тип сообщения чата.</span><span class="sxs-lookup"><span data-stu-id="60187-146">The type of chat message.</span></span> <span data-ttu-id="60187-147">Возможные значения: `message` .</span><span class="sxs-lookup"><span data-stu-id="60187-147">The possible values are: `message`.</span></span>|
|<span data-ttu-id="60187-148">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="60187-148">createdDateTime</span></span>|<span data-ttu-id="60187-149">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="60187-149">dateTimeOffset</span></span>|<span data-ttu-id="60187-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="60187-150">Read only.</span></span> <span data-ttu-id="60187-151">Метка времени создания сообщения чата.</span><span class="sxs-lookup"><span data-stu-id="60187-151">Timestamp of when the chat message was created.</span></span>|
|<span data-ttu-id="60187-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="60187-152">lastModifiedDateTime</span></span>|<span data-ttu-id="60187-153">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="60187-153">dateTimeOffset</span></span>|<span data-ttu-id="60187-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="60187-154">Read only.</span></span> <span data-ttu-id="60187-155">Временная метка при создании сообщения чата (первоначальный параметр) или редактировании, в том числе при добавлении или удалении реакции.</span><span class="sxs-lookup"><span data-stu-id="60187-155">Timestamp when the chat message is created (initial setting) or edited, including when a reaction is added or removed.</span></span> |
|<span data-ttu-id="60187-156">ластедитеддатетиме</span><span class="sxs-lookup"><span data-stu-id="60187-156">lastEditedDateTime</span></span>|<span data-ttu-id="60187-157">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="60187-157">dateTimeOffset</span></span>|<span data-ttu-id="60187-158">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="60187-158">Read only.</span></span> <span data-ttu-id="60187-159">Временная метка при внесении изменений в сообщение чата.</span><span class="sxs-lookup"><span data-stu-id="60187-159">Timestamp when edits to the chat message were made.</span></span> <span data-ttu-id="60187-160">Запускает в пользовательском интерфейсе Microsoft Teams флаг "отредактирован".</span><span class="sxs-lookup"><span data-stu-id="60187-160">Triggers an "Edited" flag in the Microsoft Teams UI.</span></span> <span data-ttu-id="60187-161">Если не выполняется никаких изменений, значение — `null` .</span><span class="sxs-lookup"><span data-stu-id="60187-161">If no edits are made the value is `null`.</span></span>|
|<span data-ttu-id="60187-162">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="60187-162">deletedDateTime</span></span>|<span data-ttu-id="60187-163">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="60187-163">dateTimeOffset</span></span>|<span data-ttu-id="60187-164">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="60187-164">Read only.</span></span> <span data-ttu-id="60187-165">Временная метка, в которой сообщение чата удалено, или значение null, если оно не удалено.</span><span class="sxs-lookup"><span data-stu-id="60187-165">Timestamp at which the chat message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="60187-166">subject</span><span class="sxs-lookup"><span data-stu-id="60187-166">subject</span></span>|<span data-ttu-id="60187-167">string</span><span class="sxs-lookup"><span data-stu-id="60187-167">string</span></span>| <span data-ttu-id="60187-168">Тема сообщения чата в виде открытого текста.</span><span class="sxs-lookup"><span data-stu-id="60187-168">The subject of the chat message, in plaintext.</span></span>|
|<span data-ttu-id="60187-169">body</span><span class="sxs-lookup"><span data-stu-id="60187-169">body</span></span>|[<span data-ttu-id="60187-170">itemBody</span><span class="sxs-lookup"><span data-stu-id="60187-170">itemBody</span></span>](itembody.md)|<span data-ttu-id="60187-171">Представление содержимого сообщения чата в формате обычного текста или в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="60187-171">Plaintext/HTML representation of the content of the chat message.</span></span> <span data-ttu-id="60187-172">Представление определяется параметром contentType в тексте.</span><span class="sxs-lookup"><span data-stu-id="60187-172">Representation is specified by the contentType inside the body.</span></span> <span data-ttu-id="60187-173">Если сообщение чата содержит [чатмессажементион](chatmessagemention.md), содержимое всегда находится в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="60187-173">The content is always in HTML if the chat message contains a [chatMessageMention](chatmessagemention.md).</span></span> |
|<span data-ttu-id="60187-174">summary</span><span class="sxs-lookup"><span data-stu-id="60187-174">summary</span></span>|<span data-ttu-id="60187-175">string</span><span class="sxs-lookup"><span data-stu-id="60187-175">string</span></span>| <span data-ttu-id="60187-176">Сводный текст сообщения чата, которое можно использовать для push-уведомлений и сводных представлений, а также для обратного просмотра.</span><span class="sxs-lookup"><span data-stu-id="60187-176">Summary text of the chat message that could be used for push notifications and summary views or fall back views.</span></span> <span data-ttu-id="60187-177">Применяется только к сообщениям разговора по каналу, а не к сообщениям в чате.</span><span class="sxs-lookup"><span data-stu-id="60187-177">Only applies to channel chat messages, not chat messages in a chat.</span></span> |
|<span data-ttu-id="60187-178">attachments</span><span class="sxs-lookup"><span data-stu-id="60187-178">attachments</span></span>|<span data-ttu-id="60187-179">Коллекция [chatMessageAttachment](chatmessageattachment.md)</span><span class="sxs-lookup"><span data-stu-id="60187-179">[chatMessageAttachment](chatmessageattachment.md) collection</span></span> |<span data-ttu-id="60187-180">Вложенные файлы.</span><span class="sxs-lookup"><span data-stu-id="60187-180">Attached files.</span></span> <span data-ttu-id="60187-181">В настоящее время вложения доступны только для чтения. Отправка вложений не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60187-181">Attachments are currently read-only – sending attachments is not supported.</span></span> |
|<span data-ttu-id="60187-182">mentions</span><span class="sxs-lookup"><span data-stu-id="60187-182">mentions</span></span>|<span data-ttu-id="60187-183">Коллекция [chatMessageMention](chatmessagemention.md)</span><span class="sxs-lookup"><span data-stu-id="60187-183">[chatMessageMention](chatmessagemention.md) collection</span></span>| <span data-ttu-id="60187-184">Список сущностей, упоминаемых в сообщении чата.</span><span class="sxs-lookup"><span data-stu-id="60187-184">List of entities mentioned in the chat message.</span></span> <span data-ttu-id="60187-185">В настоящее время поддерживаются значения user, bot, team и channel.</span><span class="sxs-lookup"><span data-stu-id="60187-185">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="60187-186">importance</span><span class="sxs-lookup"><span data-stu-id="60187-186">importance</span></span>| <span data-ttu-id="60187-187">string</span><span class="sxs-lookup"><span data-stu-id="60187-187">string</span></span> | <span data-ttu-id="60187-188">Важность сообщения чата.</span><span class="sxs-lookup"><span data-stu-id="60187-188">The importance of the chat message.</span></span> <span data-ttu-id="60187-189">Допустимые значения: `normal`, `high`, `urgent`.</span><span class="sxs-lookup"><span data-stu-id="60187-189">The possible values are: `normal`, `high`, `urgent`.</span></span>|
| <span data-ttu-id="60187-190">полицивиолатион</span><span class="sxs-lookup"><span data-stu-id="60187-190">policyViolation</span></span> | [<span data-ttu-id="60187-191">чатмессажеполицивиолатион</span><span class="sxs-lookup"><span data-stu-id="60187-191">chatMessagePolicyViolation</span></span>](../resources/chatmessagepolicyviolation.md) |<span data-ttu-id="60187-192">Определяет свойства нарушения политики, заданные с помощью приложения предотвращения потери данных (DLP).</span><span class="sxs-lookup"><span data-stu-id="60187-192">Defines the properties of a policy violation set by a data loss prevention (DLP) application.</span></span>|
|<span data-ttu-id="60187-193">языковые стандарты</span><span class="sxs-lookup"><span data-stu-id="60187-193">locale</span></span>|<span data-ttu-id="60187-194">string</span><span class="sxs-lookup"><span data-stu-id="60187-194">string</span></span>|<span data-ttu-id="60187-195">Язык сообщения чата, заданное клиентом.</span><span class="sxs-lookup"><span data-stu-id="60187-195">Locale of the chat message set by the client.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="60187-196">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="60187-196">JSON representation</span></span>

<span data-ttu-id="60187-197">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="60187-197">The following is a JSON representation of the resource.</span></span>

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
