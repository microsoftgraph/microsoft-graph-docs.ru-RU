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
# <a name="chatmessage-resource-type"></a>Тип ресурса chatMessage

Пространство имен: microsoft.graph

Представляет отдельное сообщение чата в [беседе](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true)по [каналу](./channel.md) или (в бета-версии). Сообщение чата может быть корневым сообщением чата или частью ответа, которое определяется свойством **реплитоид** в сообщении чата.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|**Сообщения канала**| | |
|[Создание объекта chatMessage в канале](../api/channel-post-messages.md) | [chatMessage](#chatmessage-resource-type)| Создайте новое сообщение разговора верхнего уровня в канале.|
|[Обновление chatMessage](../api/chatmessage-update.md)|[chatMessage](chatmessage.md)| Обновление свойства **полицивиолатион** сообщения чата.|
|**Ответы на сообщения канала**| | |
|[Ответ на chatMessage в канале](../api/channel-post-messagereply.md) | [chatMessage](#chatmessage-resource-type)| Ответ на существующее сообщение чата в канале.|

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|id|String| Только для чтения. Уникальный идентификатор сообщения.|
|replyToId| string | Только для чтения. Идентификатор родительского сообщения чата или сообщения корневого сеанса беседы в цепочке. (Применяется только к сообщениям чата в каналах без чатов) |
|from|[identitySet](identityset.md)| Только для чтения. Сведения об отправителе сообщения чата.|
|etag| string | Только для чтения. Номер версии сообщения чата. |
|messageType|string|Тип сообщения чата. Возможные значения: `message` .|
|createdDateTime|dateTimeOffset|Только для чтения. Метка времени создания сообщения чата.|
|lastModifiedDateTime|dateTimeOffset|Только для чтения. Временная метка при создании сообщения чата (первоначальный параметр) или редактировании, в том числе при добавлении или удалении реакции. |
|ластедитеддатетиме|dateTimeOffset|Только для чтения. Временная метка при внесении изменений в сообщение чата. Запускает в пользовательском интерфейсе Microsoft Teams флаг "отредактирован". Если не выполняется никаких изменений, значение — `null` .|
|deletedDateTime|dateTimeOffset|Только для чтения. Временная метка, в которой сообщение чата удалено, или значение null, если оно не удалено. |
|subject|string| Тема сообщения чата в виде открытого текста.|
|body|[itemBody](itembody.md)|Представление содержимого сообщения чата в формате обычного текста или в формате HTML. Представление определяется параметром contentType в тексте. Если сообщение чата содержит [чатмессажементион](chatmessagemention.md), содержимое всегда находится в формате HTML. |
|summary|string| Сводный текст сообщения чата, которое можно использовать для push-уведомлений и сводных представлений, а также для обратного просмотра. Применяется только к сообщениям разговора по каналу, а не к сообщениям в чате. |
|attachments|Коллекция [chatMessageAttachment](chatmessageattachment.md) |Вложенные файлы. В настоящее время вложения доступны только для чтения. Отправка вложений не поддерживается. |
|mentions|Коллекция [chatMessageMention](chatmessagemention.md)| Список сущностей, упоминаемых в сообщении чата. В настоящее время поддерживаются значения user, bot, team и channel.|
|importance| string | Важность сообщения чата. Допустимые значения: `normal`, `high`, `urgent`.|
| полицивиолатион | [чатмессажеполицивиолатион](../resources/chatmessagepolicyviolation.md) |Определяет свойства нарушения политики, заданные с помощью приложения предотвращения потери данных (DLP).|
|языковые стандарты|string|Язык сообщения чата, заданное клиентом.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

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
