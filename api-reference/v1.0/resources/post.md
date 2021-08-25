---
title: Тип ресурса Post
description: Представляет отдельный элемент Post в сущности conversationThread.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: f1af505f7c55ef46c855d92170679195bb390474
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/25/2021
ms.locfileid: "58513197"
---
# <a name="post-resource-type"></a>Тип ресурса Post

Пространство имен: microsoft.graph представляет отдельный элемент Post в [объекте conversationThread.](conversationthread.md)

Хотя явно создать экземпляр post невозможно, он будет создан в результате выполнения любого из указанных ниже действий.

- [Добавление ответа к существующей публикации](../api/post-reply.md). 
- [Добавление ответа к существующей цепочке](../api/conversationthread-reply.md). 
- [Создание цепочки в новой беседе](../api/group-post-threads.md).
- [Создание беседы](../api/group-post-conversations.md).

С помощью этого ресурса можно добавлять собственные данные к настраиваемым свойствам, применяя [расширения](/graph/extensibility-overview).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Вывод списка публикаций](../api/conversationthread-list-posts.md) | [post](post.md) |Получение публикаций из указанной цепочки. |
|[Получение публикации](../api/post-get.md) | [post](post.md) |Получение свойств и связей публикации в указанной цепочке.|
|[Ответ](../api/post-reply.md)|Нет|Ответ на публикацию и добавление новой публикации в указанную цепочку беседы группы.|
|[Переадресация](../api/post-forward.md)|Нет|Переадресация публикации получателю.|
|**Вложения**| | |
|[Список вложений](../api/post-list-attachments.md) |Коллекция [attachment](attachment.md) | Получает все вложения для экземпляра post.|
|[Добавление вложения](../api/post-post-attachments.md) |[attachment](attachment.md)| Добавление вложения в публикацию. |
|**Открытые расширения**| | |
|[Создание открытого расширения](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Создание открытого расширения и добавление настраиваемых свойств в новый или существующий экземпляр ресурса.|
|[Получение открытого расширения](../api/opentypeextension-get.md) |Коллекция [openTypeExtension](opentypeextension.md)| Получение объектов открытого расширения, которые определяются по имени или полному имени.|
|**Расширения схемы**| | |
|[Добавление значений расширений для схемы](/graph/extensibility-schema-groups) || Создание определения расширения схемы и его дальнейшее использование для добавления в ресурс введенных пользовательских данных.|
|**Расширенные свойства**| | |
|[Создание расширенного свойства с одним значением](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[post](post.md)  |Создание одного или нескольких расширенных свойств с одним значением в новой или существующей публикации.   |
|[Получение публикации с расширенным свойством с одним значением](../api/singlevaluelegacyextendedproperty-get.md)  | [post](post.md) | Получение публикаций, которые содержат расширенное свойство с одним значением, с помощью параметра `$expand` или `$filter`. |
|[Создание расширенного свойства с несколькими значениями](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [post](post.md) | Создание одного или нескольких расширенных свойств с несколькими значениями в новой или существующей публикации.  |
|[Получение публикации с расширенным свойством с несколькими значениями](../api/multivaluelegacyextendedproperty-get.md)  | [post](post.md) | Получение публикации, которая содержит расширенное свойство с несколькими значениями, с помощью параметра `$expand`. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|body|[itemBody](itembody.md)|Содержимое публикации. Это свойство используется по умолчанию. Это свойство может иметь значение null.|
|categories|Коллекция String|Категории, сопоставленные с публикацией.|
|changeKey|String|Указывает версию публикации. При каждом изменении публикации также меняется значение ChangeKey. Благодаря этому Exchange может применять изменения к правильной версии объекта.|
|conversationId|String|Уникальный идентификатор беседы. Только для чтения.|
|conversationThreadId|Строка|Уникальный идентификатор цепочки беседы. Только для чтения.|
|createdDateTime|DateTimeOffset|Указывает, когда была создана должность. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|from|[recipient](recipient.md)|Используется в сценариях делегированного доступа. Указывает, кто опубликовал сообщение от имени другого пользователя. Это свойство используется по умолчанию.|
|hasAttachments|Boolean|Указывает, есть ли в публикации хотя бы одно вложение. Это свойство используется по умолчанию.|
|id|String| Только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Указывает, когда сообщение было изменено в последний раз. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|newParticipants|Коллекция объектов [recipient](recipient.md)|Участники беседы, которые были добавлены в цепочку в рамках этой публикации.|
|receivedDateTime|DateTimeOffset|Указывает, когда сообщение было получено. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|sender|[recipient](recipient.md)|Содержит электронный адрес отправителя. Если получатель не указан, то в качестве значения Sender используется адрес пользователя, прошедшего проверку подлинности. Это свойство используется по умолчанию.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|attachments|Коллекция [Attachment](attachment.md)| Только для чтения. Допускается значение null. Поддерживает `$expand`.|
|extensions|Коллекция [Extension](extension.md)|Коллекция открытых расширений, определенных для столба. Только для чтения. Допускается значение null. Поддерживает `$expand`.|
|inReplyTo|[post](post.md)| Только для чтения. Поддерживает `$expand`.|
|multiValueExtendedProperties|Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| Коллекция расширенных свойств с несколькими значениями, определенных для публикации. Только для чтения. Допускается значение null.|
|singleValueExtendedProperties|Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| Коллекция расширенных свойств с одним значением, определенных для публикации. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже этот ресурс представлен в формате JSON.

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [
    "attachments",
    "inReplyTo",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "baseType": "microsoft.graph.outlookItem",
  "@odata.type": "microsoft.graph.post",
  "@odata.annotations": [
    {
      "property": "attachments",
      "capabilities": {
        "changeTracking": false,
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "extensions",
      "capabilities": {
        "changeTracking": false,
        "searchable": false
      }
    },
    {
      "property": "inReplyTo",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "insertable": false,
        "navigability": "single",
        "searchable": false,
        "updatable": false
      }
    }
  ]
}-->

```json
{
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "categories": ["string"],
  "changeKey": "string",
  "conversationId": "string",
  "conversationThreadId": "string",
  "createdDateTime": "String (timestamp)",
  "from": {"@odata.type": "microsoft.graph.recipient"},
  "hasAttachments": true,
  "id": "string (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "newParticipants": [{"@odata.type": "microsoft.graph.recipient"}],
  "receivedDateTime": "String (timestamp)",
  "sender": {"@odata.type": "microsoft.graph.recipient"}
}

```

## <a name="see-also"></a>См. также

- [Добавление пользовательских данных в ресурсы с помощью расширений](/graph/extensibility-overview)
- [Добавление пользовательских данных в ресурсы user с помощью открытых расширений](/graph/extensibility-open-users)
- [Добавление пользовательских данных в группы с помощью расширений схемы](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "post resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

